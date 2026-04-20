# eERC Avalanche Skill

Skill for developing private eERC (Encrypted ERC) tokens on Avalanche with real privacy + auditability.

## What it solves?

- Privacy in balances and transfer amounts
- Compliance (KYC/AML) without exposing data publicly
- EVM compatibility while maintaining confidentiality

## Installation

### Windsurf (Recommended)
```bash
npx skills add TincoNomad/avalanche-eerc20-skill
```

### Other Platforms
The skills CLI automatically generates platform-specific files after installation. When you run `npx skills add`, it will ask which platforms you want to support and create the appropriate files (`.cursorrules`, `CLAUDE.md`, etc.) automatically.

The core content in `SKILL.md` and `references/` remains platform-agnostic and serves as the source for all generated platform files.

## Example Prompts

Once installed, mention any of these in your AI session:

- "I want to build a private token on Avalanche"
- "Should I use Standalone or Converter mode for my ERC-20?"
- "How do I migrate my public token to eERC?"
- "Explain how zk-SNARKs work with encrypted balances"
- "Set up selective auditing for compliance"

## Tech Stack

- **Cryptography**: zk-SNARKs (Groth16), ElGamal over BabyJubJub, Poseidon
- **Network**: Avalanche C-Chain, Fuji testnet, L1s
- **Standards**: eERC (Encrypted ERC), ERC-20 compatibility
- **Use Cases**: Private DeFi, regulated assets, confidential payroll

## Structure

- `SKILL.md` — Skill definition and workflow for the agent
- `references/` — Technical reference documentation
  - `01-context-standards-and-limits.md` — Why traditional ERCs fall short
  - `02-deployment-modes-and-cases.md` — Standalone vs Converter guide
  - `03-cryptography-and-components.md` — Cryptographic stack & components
  - `04-eerc-flow-and-operations.md` — Private transfer flow
  - `05-deploy-converter-step-by-step.md` — Operational deployment guide

## Requirements

- Any AI-powered IDE (Windsurf, Cursor, Claude Code, etc.)
- Basic knowledge of Solidity and EVM
- Avalanche Fuji testnet access (for testing)

## Contributing

Contributions are welcome! Here's how to help improve this skill:

### Reporting Issues
- Open a GitHub issue for bugs, unclear explanations, or missing topics
- Include specific prompts where the skill response could be better

### Adding Content
- Reference files in `references/` can be expanded with more examples
- New reference files should follow the numbered naming convention
- Keep content concise and actionable for agent workflows

### Improving Workflows
- `SKILL.md` defines the agent workflow — suggest improvements via PR
- Test changes in Windsurf before submitting

### Code Contributions
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/your-improvement`)
3. Make your changes
4. Test with real prompts in Windsurf
5. Submit a pull request with description of changes

## Version

**v1.0.0** — Core eERC workflow and documentation


## Status

✅ Ready for use — all references completed.
