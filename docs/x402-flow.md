# x402 Flow

API20 explores **HTTP 402 Payment Required** flows for pay-per-request APIs on **Base** using **USDC**.

## Basic flow

1. Client requests a protected API resource
2. Server responds with `402 Payment Required` and payment metadata
3. Client parses requirements (network, asset, amount, resource)
4. Client prepares payment (research / planned — not live in API20 yet)
5. Client retries the request with payment proof (research / planned)

## What API20 inspects

When scanning or inspecting an endpoint, API20 aims to surface:

| Field | Example |
|-------|---------|
| HTTP status | `402 Payment Required` |
| Protocol | `x402` |
| Network | `base` |
| Asset | `USDC` |
| Amount | `0.001` |
| Resource | `/weather` |

## Example response

See [examples/x402-response-example.json](../examples/x402-response-example.json).

## Current limitations

- Website scanner is a **simulation** — no real network probe in the static version
- No payment execution on Base
- Demo API at [server.api20.xyz](https://server.api20.xyz) returns sample 402 JSON only

## Related docs

- [API Metadata](api-metadata.md)
- [Commands](commands.md)
- [Registry Schema](registry-schema.md)
