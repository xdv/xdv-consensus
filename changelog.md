# Changelog

## 0.1.1 - XDV-042 Core Implementation

- Implemented deterministic consensus contracts in `src/consensus_contracts.ds`.
- Implemented deterministic reconciliation engine in `src/consensus_reconcile.ds`.
- Implemented PHI-assisted consensus mode in `src/consensus_phi_mode.ds`.
- Implemented deterministic K fallback mode in `src/consensus_k_fallback.ds`.
- Implemented replay-equivalence checks in `src/consensus_replay.ds`.
- Added XDV-042 behavior tests in `src/consensus_tests.ds`.
- Added aggregate test entrypoint `tests/consensus_replay_e2e.ds`.
- Updated README and docs for active implementation status.

## 0.1.0 - Initial Skeleton

- Created project scaffold for XDV Consensus.
- Added State.toml, README.md, and docs/test placeholders.
- Imported LICENSE from xdv-os/LICENSE.
