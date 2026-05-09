# shielded-docs

> Documentation for Shielded Protocol.

Part of [Shielded Protocol](https://github.com/Shielded-Protocol) —
private, compliant DeFi on Stellar.

[![CI](https://github.com/Shielded-Protocol/shielded-docs/actions/workflows/ci.yml/badge.svg)](https://github.com/Shielded-Protocol/shielded-docs/actions/workflows/ci.yml)
[![Stellar Wave](https://img.shields.io/badge/Stellar-Wave-blue)](https://drips.network/wave/stellar)
[![Issues](https://img.shields.io/github/issues/Shielded-Protocol/shielded-docs)](https://github.com/Shielded-Protocol/shielded-docs/issues)

Built with [Astro Starlight](https://starlight.astro.build).

---

## Pages

| Page | Status | Description |
|---|---|---|
| Getting started / Quickstart | ✅ | End-to-end setup guide |
| Getting started / How it works | ✅ | Plain-English ZK explainer |
| Reference / Glossary | ✅ | 14 ZK terms defined for non-cryptographers |
| Guides / Integration | 🔧 Open issue | Adding Shielded to your dApp |
| Guides / Compliance | 🔧 Open issue | Institutional auditor guide |
| Contracts / Commitment pool | 🔧 Open issue | API reference |
| SDK / @shielded/core | 🔧 Open issue | Function reference |

---

## Quickstart

```bash
git clone https://github.com/Shielded-Protocol/shielded-docs
cd shielded-docs
pnpm install

# Local preview
pnpm dev
# → http://localhost:4321

# Production build
pnpm build
```

---

## Contributing to docs

No cryptography knowledge required. If you can read and write clearly,
you can contribute.

Good places to start:
- **Translations**: Portuguese and Spanish quickstart guides are open issues
- **Missing pages**: Integration guide, compliance guide, API references
- **Improvements**: Clarify confusing sentences, add examples, fix broken links

Browse [Wave-ready docs issues](https://github.com/Shielded-Protocol/shielded-docs/issues?q=label%3Astatus%3Awave-ready+state%3Aopen).

---

## Writing style

- Short sentences. One idea per sentence.
- Define every technical term on first use (or link to glossary).
- Always include a code example.
- Never assume the reader knows ZK — explain from first principles.

---

## License

MIT
