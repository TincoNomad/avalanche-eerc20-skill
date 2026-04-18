# Cryptography and eERC Components

## Cryptographic Stack

- `zk-SNARKs` (Groth16 in official implementation): proves validity without revealing data.
- `ElGamal` over `BabyJubJub`: encrypts balances and amounts.
- `Poseidon`: efficient hash for ZK circuits and on-chain verifications.
- `Homomorphic properties`: allow updating encrypted balances without decrypting.

## Main On-Chain Components

- `Registrar Contract`
  - manages authorized auditors,
  - administers access keys/permissions.
- `EncryptedUserBalances` / `encryptedERC`
  - persists encrypted balances,
  - updates state after valid proofs.
- `AuditorManager` (if applicable in your stack)
  - controls audit permission lifecycle.
- `Proof Verifier`
  - validates zk proofs in contract.

## Privacy with Compliance

eERC is not total opacity:
- maintains public confidentiality of sensitive data,
- allows selective decryption by authorized actors,
- supports permission revocation/rotation without redesigning the entire system.
