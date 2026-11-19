---
term: "CIRISDepot"
category: architectural-component
earliest_known_public_use: "2026-08-13"
earliest_source_repo: "CIRISAI/CIRISDepot"
earliest_source_commit: "1f99381"
earliest_source_url: "https://github.com/CIRISAI/CIRISDepot/commit/1f99381"
scope_claimed: "the name 'CIRISDepot' and its design: a stateless, read-only HTTP shim that serves an artifact only if its signature chains to a baked trust root"
---

# CIRISDepot

**CIRISDepot** is a thin, stateless, read-only shim that serves CIRIS content over ordinary HTTP, from Cloudflare Workers or any disposable container. It ships with a **baked trust root**, by default the humanity accord. It serves an artifact only if that artifact's signature chains back to the root through an accord-blessed build-signing key.

It exists so CIRIS can stop depending on GitHub Releases, PyPI and Cloudflare as sources of truth. Depot is not the artifact store; the CIRIS node is. Depot holds nothing authoritative, and everything it serves it can re-derive.

Status: draft specification, no implementation yet.

## Earliest known public use

- **2026-08-13**: [`CIRISDepot@1f99381`](https://github.com/CIRISAI/CIRISDepot/commit/1f99381), *"CIRISDepot spec draft 0.2"*.

## Scope of priority claim

Signed package repositories (TUF, Sigstore), content-addressed mirrors and edge caching are prior art. CIRIS claims priority on the name **"CIRISDepot"** and on its design: a disposable, authority-free mirror whose trust root is baked into its path and chains to a governance document.
