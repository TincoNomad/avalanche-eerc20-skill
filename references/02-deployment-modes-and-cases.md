# Standalone vs Converter: Decision Guide

## Standalone Mode

Use it when:
- the token is born private from the first mint,
- you optionally want to hide total supply,
- the product is designed as a private market from the start.

Examples:
- confidential enterprise payments,
- regulated financial assets with privacy by default,
- private game economies on L1.

## Converter Mode

Use it when:
- you already have an ERC-20 in production,
- you need wrap/unwrap to alternate between public and private,
- you want compatibility with existing public liquidity.

Examples:
- sensitive governance with optional privacy,
- bridge between public pools and private operations,
- gradual transition from ERC-20 to eERC.

## Quick Rule

- **New token + privacy by design** -> Standalone.
- **Existing token + incremental privacy** -> Converter.
