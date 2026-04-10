# Replay Equivalence

Implemented in `src/consensus_replay.ds`.

## Objective

Consensus decisions must be replay-equivalent for equivalent inputs.

## Mechanism

- construct deterministic decision records
- rebuild records from replay input
- compare for exact equivalence

## Key APIs

- `decision_record_token(...)`
- `replay_equivalent(...)`
- `rebuild_and_compare(...)`
- `consensus_round_replay_check(...)`
