---
term: "CEWPOS"
expansion: "CIRIS Epistemic Web Platform OS"
category: system
earliest_known_public_use: "2026-06-27"
earliest_source_repo: "CIRISAI/CEWPOS"
earliest_source_commit: "7778729"
earliest_source_url: "https://github.com/CIRISAI/CEWPOS/commit/7778729"
scope_claimed: "the names 'CEWPOS' and 'Attestation Calculus', and the specific architecture: an operating system as a deterministic evaluator over signed records, with authority separated from execution and rendering isolated from authority"
---

# CEWPOS and the Attestation Calculus

**CEWPOS** (CIRIS Epistemic Web Platform OS) is an operating system built not as a scheduler of processes but as an evaluator over immutable, signed records:

- **State** is an append-only history of signed, content-addressed attestations in CEG, the CIRIS Epistemic Grammar. Nothing is mutated. A record is superseded, and the old one stays.
- **Execution** is the **Attestation Calculus**, a deterministic, total, effect-typed evaluator. Its only effect is an `emit` that must pass a gate.
- **Authority is separated from execution.** An agent, human or AI, does not control anything. It emits an attestation, and an independent admission gate admits or rejects it. No participant gains power merely by running.
- **Rendering is isolated from authority.** Views are pure functions (*view-forms*) compiled to WebAssembly components with zero ambient authority. Each produces a renderer-neutral **Scene IR**, and a host renderer turns that into pixels.

CEWPOS is the earliest public statement of the architecture that the [CIRIS Kernel](kernel.md) later made exact for governance. It is also the public precursor of [CIRISISA](isa.md), which carries the Kernel's primitives into computation.

## Earliest known public use

- **2026-06-27 20:36 −05:00**: [`CEWPOS@7778729`](https://github.com/CIRISAI/CEWPOS/commit/7778729), *"Initial commit — CEWPOS: superalignment infrastructure as a civilizational OS"*. Introduces the Attestation Calculus, typed view-forms and the zero-ambient-authority WASM view component.
- **2026-06-27 21:30 −05:00**: [`CEWPOS@a20b198`](https://github.com/CIRISAI/CEWPOS/commit/a20b198), `WHY.md`: *"CEWPOS is an operating system built not as a scheduler of processes but as an evaluator over immutable, signed records … authority is separated from execution, so no participant (human or AI) gains power merely by running."*

## Subsequent significant uses

- 2026-11-15: [holon-draw](holon-draw.md) takes CEWPOS as its whole-screen host profile, where the drawn scene is the entire screen.

## Canonical definition (excerpt)

> CEWPOS is an operating system built not as a scheduler of processes but as an **evaluator over immutable, signed records** — computation is deterministic, history is append-only, and **authority is separated from execution**, so no participant (human or AI) gains power merely by running.

(Source: [`CEWPOS/WHY.md`](https://github.com/CIRISAI/CEWPOS/blob/main/WHY.md).)

## Scope of priority claim

The pieces have long prior art, and CEWPOS's own README names several of them:

- Git's object model and content-addressed storage.
- RDF.
- Capability systems and object capabilities (Dennis and Van Horn, 1966; Miller, 2006).
- Lisp homoiconicity.
- Event sourcing and immutable databases.
- The WebAssembly component model.
- Views as pure functions of state, as in the Elm architecture.

CIRIS claims priority on the names **"CEWPOS"** and **"Attestation Calculus"**, and on the specific combination. The operating system is an evaluator over signed records in a closed attestation grammar, its only effect is an `emit` checked by an independent admission gate, and its views are zero-authority components. That gives one architecture in which neither a human nor an AI gains authority by executing.
