# Operational Deploy (Converter) on Avalanche

## Prerequisites

- Node/Hardhat environment set up.
- Avalanche RPC (Fuji for testing).
- Private keys for test accounts in `.env`.
- Dependencies installed (`npm install`).

## Recommended Execution Flow

1. Initialize converter contract/base.
2. Deploy core contracts.
3. Register users.
4. Configure auditor.
5. Obtain test funds/tokens.
6. Execute `deposit` to convert ERC-20 -> eERC.
7. Execute private `transfer` between registered accounts.
8. Execute `withdraw` to convert eERC -> ERC-20.
9. Verify balances before and after each operation.

## Practical Warnings

- `.env` and key configuration is critical for zk scripts.
- Account changes (`WALLET_NUMBER`) must be carefully controlled.
- In production, add secret management, key rotation, and robust access controls.

## Note on Proving Systems

- `Groth16` is the default in official eERC implementations.
- Switching to `PLONK` or `Halo2` requires modifying circuits, regenerating verifiers, and redeploying.
