# Float Docs

Documentation for [Float](https://usefloat.xyz) — Solana-native AI agent treasury.

Built with [Mintlify](https://mintlify.com). Deployed at **usefloat.xyz/docs**.

## Development

```bash
npm install -g mintlify
mintlify dev
```

Opens at http://localhost:3000.

## Deploy

Docs deploy automatically via Mintlify's GitHub integration.
Push to `main` → Mintlify rebuilds and deploys.

## Structure

```
float-docs/
├── mint.json              ← Mintlify config (nav, colors, domain)
├── llms.txt               ← Flat index for AI agents
├── introduction.mdx
├── quickstart.mdx
├── setup/
│   ├── for-humans.mdx
│   └── for-agents.mdx
├── mcp/
│   ├── overview.mdx
│   └── tools.mdx
├── concepts/
│   ├── x402.mdx
│   ├── treasury.mdx
│   └── agent-wallets.mdx
└── api-reference/
    ├── overview.mdx
    ├── agents.mdx
    ├── payments.mdx
    └── services.mdx
```

## Custom domain setup

In the Mintlify dashboard, set the custom domain to `usefloat.xyz` with base path `/docs`.
Or use `docs.usefloat.xyz` as a subdomain — either works with Mintlify.

Add a CNAME record pointing `docs` to `mint.mintlify.app`.
