---
term: "CIRIS Specification Document (CSD)"
short_form: "CSD"
category: protocol
earliest_known_public_use: "2026-09-07"
earliest_source_repo: "CIRISAI/CIRISAgent"
earliest_source_commit: "853a543d8"
earliest_source_url: "https://github.com/CIRISAI/CIRISAgent/commit/853a543d8"
scope_claimed: "the name 'CIRIS Specification Document (CSD)' and the specific form: one document that is both a feature's specification and its executable test"
---

# CIRIS Specification Document (CSD)

A **CIRIS Specification Document** is Mission Driven Development applied to one feature. It states:

- the **mission** a surface serves,
- the **schemas** it is made of: screens, guaranteed tags and fields,
- the **protocols** it reads: endpoints, version floors and owners,
- the **logic** that drives it, written as a flow in a UI DSL.

It also includes one thing a feature has that an architecture does not: **a test that is the same document as the spec.**

## Earliest known public use

- **2026-09-07**: [`CIRISAgent@853a543d8`](https://github.com/CIRISAI/CIRISAgent/commit/853a543d8), *"docs: the CSD standard, and the first four CSDs for CIRISClient#45"*.

## Subsequent significant uses

- 2026-09-08: [`CIRISAgent@e7a4ee7b7`](https://github.com/CIRISAI/CIRISAgent/commit/e7a4ee7b7). The QA runner drives CSD flows on the running client.
- 2026-09-08: [`CIRISClient@4941f61d`](https://github.com/CIRISAI/CIRISClient/commit/4941f61d), CSD-B. The arrow reverses, so a surface can be designed before it is built.
- 2026-09-09: [`CIRISClient@145f9934`](https://github.com/CIRISAI/CIRISClient/commit/145f9934), CSD/3. *"The DSL checks what the spec promises, and the CEG family IS the field."*
- Later: CSD/4 binds each card's tests to the closed 20-topology catalogue. This leads to the CIRIS screen standard of 24 UX primitives, which [holon-draw](holon-draw.md) composes.

## Canonical definition (excerpt)

> A CIRIS Specification Document is Mission Driven Development applied to one feature … Plus the one thing a feature has that an architecture does not: a test that is the same document as the spec.

(Source: [`CIRISAgent@853a543d8`](https://github.com/CIRISAI/CIRISAgent/commit/853a543d8).)

## Scope of priority claim

The ideas behind CSDs are long established:

- executable specifications and behaviour-driven development (Cucumber/Gherkin),
- design by contract (Meyer),
- literate programming (Knuth),
- OpenAPI.

Some CIRIS documents expand "CSD" as "Client Surface Definition". The canonical expansion is **CIRIS Specification Document**.

CIRIS claims priority on the name **"CIRIS Specification Document"** and on its specific form: one document that holds mission, schemas, protocols and logic, and is its own test. Its fields are bound to the CEG attestation grammar, and from CSD/4 its tests are bound to a closed topology catalogue.
