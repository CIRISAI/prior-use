---
term: "CIRISProxy"
category: architectural-component
earliest_known_public_use: "2025-11-26"
earliest_source_repo: "CIRISAI/CIRISProxy"
earliest_source_commit: "7a000fe"
earliest_source_url: "https://github.com/CIRISAI/CIRISProxy/commit/7a000fe"
scope_claimed: "the name 'CIRISProxy' and its role as temporary, credit-gated, retention-free bridging infrastructure for CIRIS agents"
---

# CIRISProxy

**CIRISProxy** is a secure, credit-gated LLM proxy for CIRIS Agent mobile clients. It is **temporary bridging infrastructure**, designed to be retired once the Veilid decentralized network matures.

- Provider keys stay server-side.
- Users authenticate, and each user interaction costs one credit, which typically covers 12 to 70 LLM calls.
- Requests route across providers with fallback.
- Web search uses zero-data-retention providers.
- Logs carry no message content and no personal data.
- Access fails closed if billing is unavailable.

## Earliest known public use

- **2025-11-26**: [`CIRISProxy@7a000fe`](https://github.com/CIRISAI/CIRISProxy/commit/7a000fe), *"Add CLAUDE.md documenting CIRISProxy architecture"*.

## Scope of priority claim

LLM gateways and API proxies are common. CIRIS claims priority only on the name **"CIRISProxy"** and on its stated design: a proxy that keeps no conversations, is gated per interaction, and is built to be retired.
