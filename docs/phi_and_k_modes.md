# PHI and K Modes

Implemented across:

- `src/consensus_phi_mode.ds`
- `src/consensus_k_fallback.ds`

## PHI-Assisted Mode

- deterministic activation preflight
- capability/threshold checks
- quorum validation
- deterministic final reconciliation

## K Fallback Mode

Fallback is triggered deterministically when PHI path is unavailable or unstable.

- coherence instability
- envelope misalignment
- node desync
- network partition
- provider failure

Fallback preserves deterministic ordering and decision semantics.
