# Context: Current Standards and Why They Fall Short

## Foundation on Avalanche (EVM)

- `ERC-20`: fungible, high interoperability, no native privacy.
- `ERC-721`: unique NFTs, public ownership.
- `ERC-1155`: multi-asset and batch transfers, but also public.

## Structural Problem

In all three traditional standards:
- balances visible publicly,
- transfer amounts public,
- ownership history and activity traceable.

This is useful for open auditability, but limits adoption in:
- regulated finance,
- enterprise with trade secrets,
- cases with personal/sensitive data.

## Business Impact and Compliance

- No native selective disclosure for regulators.
- No built-in compliance controls by standard.
- Teams must build custom layers, increasing cost, risk, and complexity.

## Signal That You Should Migrate to eERC

Consider eERC if you need at least one:
- hide amounts or balances in production,
- maintain privacy without losing regulatory oversight,
- avoid exposure of strategies, payroll, or treasury.
