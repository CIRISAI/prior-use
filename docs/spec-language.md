---
term: "CIRIS specification-and-test language"
category: concept
earliest_known_public_use: "2025-05-31"
earliest_source_repo: "CIRISAI/CIRISAgent"
earliest_source_commit: "baa3f2484"
earliest_source_url: "https://github.com/CIRISAI/CIRISAgent/commit/baa3f2484"
scope_claimed: "the CIRIS line in which declaring what a system should do and checking that it does are one text: mock LLM, adapter manifests, the QA runner, CSD flows, and the RATCHET modelling of H3ERE context"
---

# The CIRIS specification-and-test language

Across CIRIS, one discipline has grown into a language: **declaring what a system should do and checking that it does are the same text.** It started as a way to describe the QA process and has become the language used to model the agent's own reasoning.

| Stage | Date | What it added | Source |
|---|---|---|---|
| Mock LLM | by 2025-05-31 | a deterministic stand-in for the model, so the agent's behaviour can be specified and replayed | [`CIRISAgent@baa3f2484`](https://github.com/CIRISAI/CIRISAgent/commit/baa3f2484) |
| Adapter manifests | 2025-06-24 | an adapter declares what it is and what it provides (the first manifest is the mock LLM's) | [`CIRISAgent@50a4e1de4`](https://github.com/CIRISAI/CIRISAgent/commit/50a4e1de4) |
| QA runner | 2025-08-23 | modular, declarative QA: the testing language | [`CIRISAgent@30c3df512`](https://github.com/CIRISAI/CIRISAgent/commit/30c3df512) |
| CSD flows | 2026-09-07 / 09-08 | a [CIRIS Specification Document](csd.md) is its own test; the QA runner drives its flows on the running client | [`CIRISAgent@853a543d8`](https://github.com/CIRISAI/CIRISAgent/commit/853a543d8), [`e7a4ee7b7`](https://github.com/CIRISAI/CIRISAgent/commit/e7a4ee7b7) |
| RATCHET kindscope | 2026-11-11 | a language of stakes, misfits and diagnoses, with an obligation auditor and a deterministic proposer | [`RATCHET@acd225a`](https://github.com/CIRISAI/RATCHET/commit/acd225a) |
| RATCHET market4 | 2026-11-18 | H3ERE's context flow measured over 42,998 calls and modelled in TLA+: what each stage should see (10 invariants) against what it does (8 violated). This is the instrument for showing that context at each H3ERE stage is purposeful | [`RATCHET@361371a`](https://github.com/CIRISAI/RATCHET/commit/361371a) |

This language is one of the two roots of [CIRISISA](isa.md). The other is the [CIRIS Kernel](kernel.md)'s coordination.

## Scope of priority claim

Test doubles and mock objects, plugin manifests, behaviour-driven development, executable specifications and TLA+ (Lamport) are established practice. CIRIS claims priority on this specific line: one language that started by describing QA and became the language for modelling the agent's own reasoning stages, with the mock LLM making every stage specifiable and replayable.
