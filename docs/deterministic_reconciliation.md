# Deterministic Reconciliation

Implemented in `src/consensus_reconcile.ds`.

## Engine Behavior

The reconciliation function is deterministic over:

- ordered proposal identifiers
- node identity ordering
- logical timestamp ordering
- alignment metadata thresholds

Tie-break sequence is stable and replay-safe.

## Key APIs

- `proposal_order_key(...)`
- `resolve_two(...)`
- `resolve_three(...)`
- `reconcile_decision(...)`
