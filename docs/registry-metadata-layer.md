# Registry Metadata Layer

API20 v0.3 introduces a structured metadata layer for documenting x402-powered APIs.

The metadata layer is designed to describe:

- API identity (`id`, `name`)
- endpoint URL
- category
- network
- asset
- price
- payment protocol
- MCP-ready status
- Builder Code attribution status
- attribution standard (ERC-8021 research)
- status
- description
- example HTTP 402 responses (documentation)

## Public registry JSON

Example export: [examples/registry.json](../examples/registry.json)

On the website, a demo static file is available at [api20.xyz/registry.json](https://api20.xyz/registry.json).

## Current status

This is **documentation and schema research only**. It is not a live backend registry.

- Demo/static preview entries
- No real payment execution
- No production registry API
- MCP support is research/planned only
- Builder Codes support is research/planned only

## Related docs

- [Registry Schema](registry-schema.md)
- [API Detail Pages](api-detail-pages.md)
- [Registry](registry.md)
