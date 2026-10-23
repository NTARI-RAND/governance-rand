# Phase 1 Conformance Report

2026-10-22 · Calvin Secrest

## Summary

Phase 1 is complete: 12 of the 23 implementation-bound invariants in the Janus registry now have executable tests, which is the most Phase 1 can reach. The other 11 cannot be tested until missing code is built, so they move to Phase 2's build list.

- **Registry:** 30 invariants. 3 are document-bound and 27 are delegated: 23 implementation-bound and 4 instrument-bound.
- **Score:** 12 of 23 implementation invariants bound. 15 of 27 delegated invariants remain self-attested.
- **How to check:** `python jfa-conformance-suite.py --bindings ../Cloudy ../sohocloud-protocol` in the Janus repo.
- **Bylaws note:** under §9.15, "bound" means a test exists and runs in its repo's CI. It is not a claim that the delegated invariant passes.

## What's done

Twelve invariants are bound, across 6 merged pull requests in two repos. Each test is named `TestInvariant_<ID>_<Name>` so Janus can find it, and each was checked by planting violations to confirm it fails for the right reason.

| Invariant | Repo and test file | Merged in | Named residual |
| --- | --- | --- | --- |
| L1 | Cloudy `internal/economy` | Cloudy #19 | — |
| L8 | Cloudy `internal/covenant` | Cloudy #19 | — |
| L6 | Cloudy `internal/record` | Cloudy #20 | — |
| L7 | Cloudy `internal/record` | Cloudy #20 | — |
| L2 | Cloudy `internal/economy` | Cloudy #22 | Host-qualified route patterns are not read (none exist today) |
| L3 | Cloudy `internal/economy` | Cloudy #22 | — |
| L9 | Cloudy `internal/economy` | Cloudy #22 | Standing scan is per-function; the import wall and steward quorum back it |
| REC-witness-minimum | Cloudy `internal/record` | Cloudy #24 | — |
| COV-adjudicators | Cloudy `internal/consumerapi` | Cloudy #24 | Witness half untestable until witness adjudication exists |
| COV-operators-adjudicate | Cloudy `internal/dispute` | Cloudy #24 | A roster member ruling on its own case is COV-operator-dispute-witnesses (instrument) |
| P-lean-code | sohocloud-protocol `conformance_test.go` | protocol #10 | A workflow's effect can't be proven from its text |
| SUB-no-inbound-requirement | sohocloud-protocol `no_inbound_test.go` | protocol #11 | Cloudy's node agent doesn't run the loop yet; real NAT is Phase 2; address synonyms left to review |

Supporting work: Janus #22 added the `--bindings` report that counts these tests.

## What's left and why

Eleven implementation invariants stay unbound because the code they would test does not exist yet; none is blocked by a missing test idea. Four more are instrument-bound and are met by the governing documents, not by code.

| Invariant | Status | Waiting on |
| --- | --- | --- |
| REC-six-holders | Partly provable | Witnesses and the public chain; the two prosumers and the operator can be shown today |
| L4 | Blocked | Cross-community exchange |
| REC-truth-not-currency | Blocked | Cross-community exchange |
| L5 | Blocked | Public chain and transport offers |
| L11 | Blocked | Transport offers |
| L12 | Blocked | Public chain |
| REC-public-chain | Blocked | Public chain |
| REC-witness-draw | Blocked | Public chain and witness draw |
| REC-witness-work | Blocked | Witness draw as paid substrate work |
| COV-witness-adjudication | Blocked | Witness draw |
| SUB-redundant-execution | Blocked | Redundant execution on two or more hosts |

Instrument-bound (no code test applies): P-cost-of-leaving, L10, COV-operator-dispute-witnesses, GOV-prosumer-membership.

## Phase 2 build list

Seven pieces have to be built before the remaining tests can be written. The public chain unblocks the most (4 invariants), so it is the natural first build. Who builds each piece, and in what order, is still open.

| Build | Today | Unblocks |
| --- | --- | --- |
| Public chain | `sohocloud-protocol/anchor` is a labeled stub | L12, REC-public-chain, L5, REC-witness-draw |
| Witness draw as paid substrate work | Not built | REC-witness-work, REC-witness-draw, COV-witness-adjudication, witness half of COV-adjudicators |
| Transport offers (fee escrow, attestation) | Not found in any repo | L5, L11 |
| Cross-community exchange | Not built | L4, REC-truth-not-currency |
| Redundant execution on 2+ hosts | Not built | SUB-redundant-execution |
| Covenant trust gate | No spend path consults standing | Cloudy's covenant rule that reputation gates whether a member transacts on trust |
| Node agent → coordinator loop in Cloudy | Agent has no network code | A live SUB-no-inbound-requirement test on a real node |

## How Phase 2 starts

Phase 2 can start now with a small multi-node test cluster and two live tests; everything else waits on the build list.

1. **Set up the cluster:** at least one operator platform, two coordinator-facing nodes, and machines on separate networks, one behind a home router (NAT or CGNAT).
2. **Live REC-witness-minimum:** run a platform with fewer than two independent witnesses and confirm it labels itself unfederated; add a second witness and confirm the label changes.
3. **Live SUB-no-inbound-requirement:** run a node behind a real home router with no open ports, change its address mid-run, and confirm it still registers, heartbeats, polls and reports. This needs the Cloudy agent → coordinator loop first.
4. **Add chaos and faults as builds land:** dropped connections, a witness going offline, a coordinator restart.

Phase 3 (CI, public badge and report) follows once Phase 2's live tests run in CI.

## Deferred findings

Four findings stay open because none blocks Phase 2: the first three were set aside on 2026-10-15, and the Agrinet one arrived on 2026-10-21.

- [ ] **Janus `--bindings` counts tests that never run** (Jodson's bug report). A fix exists but was not submitted; Jodson may send his own.
- [ ] **Dispute Registry admits a ruling co-signed by a party on the roster.** Belongs to COV-operator-dispute-witnesses (instrument-bound, P1-001 §10.9).
- [ ] **Residual marker in `--bindings` output**, so a bound test with a named gap is visible as such.
- [ ] **Agrinet API keys in browser code** (reviewer, 2026-10-21): `VITE_API_KEY` and `NEXT_PUBLIC_API_KEY` are built into frontend code, so any production key is public. Outside the JFA suite, but a live security issue.
