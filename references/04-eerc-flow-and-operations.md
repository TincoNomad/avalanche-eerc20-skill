# Functional Flow of a Private Transfer

## Simplified Sequence

1. Wallet/backend prepares the private transaction.
2. The amount is encrypted (ElGamal over BabyJubJub).
3. zk proof is generated to demonstrate validity (sufficient balance, correct rules).
4. The verifier contract validates the proof.
5. Encrypted balances are updated in contract.
6. If applicable, authorized auditors can inspect with selective decryption.

## What the Public Network Sees

- A transaction occurred.
- No transferred amounts are visible.
- No balances in clear text are visible.

## What You Must Define in Your Product

- Who authorizes audits.
- What events trigger regulatory review.
- How permissions are revoked/rotated.
- What data must remain public for UX or compliance.
