# shielded-docs

[![CI](https://github.com/Shielded-Protocol/shielded-docs/actions/workflows/ci.yml/badge.svg)](https://github.com/Shielded-Protocol/shielded-docs/actions/workflows/ci.yml)
[![Stellar Wave](https://img.shields.io/badge/Stellar-Wave-blue)](https://drips.network/wave/stellar)
[![Issues](https://img.shields.io/github/issues/Shielded-Protocol/shielded-docs)](https://github.com/Shielded-Protocol/shielded-docs/issues)

The documentation site for [Shielded Protocol](https://github.com/Shielded-Protocol). Built with [Astro](https://astro.build) and [Starlight](https://starlight.astro.build).

---

## What's in the docs

| Page | Status | Description |
|---|---|---|
| Getting started / Quickstart | ✅ | Step-by-step guide to run the app and make your first shielded transaction |
| Getting started / How it works | ✅ | Plain-English explanation of ZK proofs, commitments, and nullifiers |
| Reference / Glossary | ✅ | 14 ZK terms defined for non-cryptographers |
| Guides / Integration | 🔧 Open issue | How to add Shielded to your own Stellar dApp using the SDK |
| Guides / Compliance | 🔧 Open issue | How auditors use viewing keys to verify positions |
| Contracts / Commitment pool | 🔧 Open issue | Full API reference for the commitment-pool contract |
| SDK / @shielded/core | 🔧 Open issue | Function reference for the core TypeScript package |
| SDK / @shielded/react | 🔧 Open issue | Hook and component reference |
| SDK / @shielded/compliance | 🔧 Open issue | Viewing key and CLI reference |

---

## Running the docs site locally

**Prerequisites:** Node.js 18+, pnpm

```bash
git clone https://github.com/Shielded-Protocol/shielded-docs
cd shielded-docs
pnpm install

# Start local dev server with hot reload
pnpm dev
# → http://localhost:4321

# Check for broken links and build errors
pnpm build

# Preview the production build
pnpm preview
```

---

## Directory structure

```
src/
└── content/
    └── docs/
        ├── index.mdx              ← Docs homepage
        ├── getting-started/       ← Quickstart + how it works
        ├── guides/                ← Integration + compliance guides
        ├── reference/             ← Glossary and API references
        ├── circuits/              ← ZK circuit documentation
        ├── contracts/             ← Soroban contract documentation
        └── sdk/                   ← TypeScript SDK reference
```

---

## Contributing to the docs

**No cryptography knowledge required.** The best docs contributors are people who read an explanation, found it confusing, and rewrote it clearly.

### Quick wins (good first contributions)

- **Fix a confusing sentence** — open an issue or send a PR with a clearer rewrite
- **Add a missing code example** — most open pages need at least one
- **Fill in a stub page** — see the table above for `🔧 Open issue` pages
- **Translations** — Portuguese and Spanish quickstart guides are open issues

Browse [Wave-ready docs issues →](https://github.com/Shielded-Protocol/shielded-docs/issues?q=label%3Astatus%3Awave-ready+state%3Aopen)

---

## Writing style guide

Follow these principles when writing or editing docs:

**1. Short sentences. One idea per sentence.**
> ❌ "The nullifier, which is derived deterministically from the secret using Poseidon, is what prevents a note from being spent twice."
> ✅ "The nullifier prevents a note from being spent twice. It is derived from the secret using Poseidon."

**2. Define every term on first use.**
Every ZK term should be explained in plain English before it is used. If the term is in the glossary, link to it.

**3. Always include a code example.**
Readers learn by doing. Every concept should have a runnable code snippet alongside it.

**4. Never assume ZK knowledge.**
Write for a developer who knows Stellar but has never heard of zero-knowledge proofs. The glossary defines the key terms — reference it freely.

**5. Show before tell.**
Lead with what the user can do, then explain how it works underneath.

---

## Local Markdown authoring tips

Pages are written in MDX (Markdown + JSX). Standard Markdown syntax works everywhere.

```mdx
---
title: My new page
description: What this page covers in one sentence
---

## Heading

Regular paragraph text.

```typescript
// Code blocks get syntax highlighting automatically
const note = await createNote(1_000_000n, 1n);
```

import { Aside } from '@astrojs/starlight/components';

<Aside type="tip">
  Use Aside for tips, warnings, and notes.
</Aside>
```

---

## Related repos

| Repo | Description |
|---|---|
| [shielded-app](https://github.com/Shielded-Protocol/shielded-app) | The live frontend app the docs describe |
| [shielded-sdk](https://github.com/Shielded-Protocol/shielded-sdk) | TypeScript SDK the integration guides cover |
| [shielded-contracts](https://github.com/Shielded-Protocol/shielded-contracts) | Contracts the API reference documents |
| [shielded-circuits](https://github.com/Shielded-Protocol/shielded-circuits) | ZK circuits the technical deep-dives explain |

---

## License

MIT
