# XDV Consensus

Version: 0.1.0
Status: active
Language: Dust Programming Language (DPL)

## Specification Alignment

Primary specification: XDV-042 in `xdv-spec`.

Implemented focus for this milestone:

1. Deterministic reconciliation engine.
2. PHI-assisted and K fallback consensus modes.
3. Replay-equivalent decision validation.

## Modules

- `src/consensus_contracts.ds`
  Contract constants and deterministic validation rules.

- `src/consensus_reconcile.ds`
  Deterministic reconciliation and tie-breaking engine.

- `src/consensus_phi_mode.ds`
  PHI-assisted consensus activation/decision path.

- `src/consensus_k_fallback.ds`
  Deterministic K-based fallback path when PHI coherence fails.

- `src/consensus_replay.ds`
  Replay-equivalence token generation and verification.

- `src/consensus_tests.ds`
  XDV-042 behavior tests for reconcile/mode/replay semantics.

- `src/main.ds`
  Bootstrap/startup/smoke/self-test entrypoints.

## Build

```bash
dust check xdv-consensus/src
```

## Test

```bash
dust check xdv-consensus/src/consensus_tests.ds
dust check xdv-consensus/tests/consensus_replay_e2e.ds
```

## Notes

- Consensus tie-breaking is deterministic and replay-stable.
- PHI path never bypasses deterministic final reconciliation.
- K fallback preserves ordering invariants after PHI instability.
- Replay checks validate equivalent decision records from equivalent inputs.
