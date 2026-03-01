# XDV Consensus Tests

Deterministic tests and fixtures for `xdv-consensus`.

## Covered Behaviors

- deterministic reconciliation engine
- PHI-assisted consensus activation and decision path
- deterministic K fallback when PHI coherence is unstable
- replay-equivalent decision reconstruction

## Entrypoints

- `xdv-consensus/src/consensus_tests.ds`
- `xdv-consensus/tests/consensus_replay_e2e.ds`

## Run

```bash
dust check xdv-consensus/src
dust check xdv-consensus/tests/consensus_replay_e2e.ds
```
