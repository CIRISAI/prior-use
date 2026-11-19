<!--
{
  "@context": "https://schema.org",
  "@type": ["Dataset", "DefinedTermSet"],
  "name": "CIRIS Terminology — Prior-Use Record",
  "description": "A reference record of canonical terms used in the CIRIS framework, with first-known-public-use timestamps drawn from version control, peer-reviewed papers, and the public web. Maintained for citation, academic reference, and historical transparency.",
  "url": "https://github.com/CIRISAI/prior-use",
  "publisher": {
    "@type": "Organization",
    "name": "CIRIS AI",
    "url": "https://ciris.ai"
  },
  "license": "https://creativecommons.org/publicdomain/zero/1.0/",
  "keywords": [
    "CIRIS", "CIRIS Covenant", "CIRIS Accord", "Coherence Ratchet",
    "Wisdom-Based Deferral", "PDMA", "H3ERE", "Wise Authority",
    "Stewardship Tier", "Adaptive Coherence", "CIRIS Constitution", "CIRISOntology",
    "CIRISHolon", "holon", "reality compiler", "CIRIS Kernel", "CIRISKernel",
    "CIRISISA", "CIRIS Instruction Set Architecture", "CEWPOS",
    "Attestation Calculus", "holon-draw", "CIRIS Specification Document",
    "CSD", "CIRISClient", "CIRISGrace", "self-organizing software",
    "alignment", "ethics", "AI safety"
  ],
  "datePublished": "2026-05-06",
  "dateModified": "2026-11-19",
  "isAccessibleForFree": true,
  "creativeWorkStatus": "Published"
}
-->

# CIRIS Terminology — Prior-Use Record

A reference record of canonical terms used in the [CIRIS](https://ciris.ai) framework, with first-known-public-use timestamps drawn from version control, peer-reviewed papers, and the public web.

This repository exists to support citation, academic reference, and historical transparency for anyone studying, citing, or building on the CIRIS framework. It is maintained as part of routine open-source housekeeping.

## What this is

For each documented term, this record provides:

- the canonical CIRIS usage (compound or compound-of-art),
- the earliest publicly available reference (with permalink, DOI, or commit hash where available),
- a list of subsequent significant uses in the public record,
- a short canonical definition.

Per-term files live under [`docs/`](docs/). Structured data lives in [`prior-use.json`](prior-use.json), with a JSON Schema in [`_schema/`](_schema/).

## Earliest CIRIS public artifact

The **CIRIS Covenant** (Version 1.0-β) is the framework's earliest public artifact. The document text states an issuance date of **2025-04-16**. The earliest verifiable public-record timestamp is the first content commit on **2025-04-21** in [`CIRISAI/CIRIS-Covenant.github.io`](https://github.com/CIRISAI/CIRIS-Covenant.github.io). Both dates are recorded; the verifiable public-record date is what citations should use.

On **2026-02-18** the document was renamed from *CIRIS Covenant* to **CIRIS Accord** in coordinated commits across [`ciris-website@b925457`](https://github.com/CIRISAI/ciris-website/commit/b925457) and [`CIRISAgent@daad5f08c`](https://github.com/CIRISAI/CIRISAgent/commit/daad5f08c). Document content lineage is continuous through the rename — the same principles, books, annexes, and procedures carry forward unchanged in substance. Two priority axes are recorded for the document:

- **Document-content lineage**: from 2025-04-21 (as Covenant).
- **Named compound *CIRIS Accord***: from 2026-02-18.

## Documented terms

| Term | First known public use | Source |
|---|---|---|
| [CIRIS Covenant](docs/covenant.md) (renamed to *Accord* 2026-02-18) | 2025-04-21 (document-issued: 2025-04-16) | [`CIRIS-Covenant.github.io@5ac7def`](https://github.com/CIRISAI/CIRIS-Covenant.github.io/commit/5ac7def) |
| [CIRIS Accord](docs/accord.md) | content lineage from 2025-04-21; named compound from 2026-02-18 | [`ciris-website@b925457`](https://github.com/CIRISAI/ciris-website/commit/b925457) |
| [PDMA — Principled Decision-Making Algorithm](docs/pdma.md) | 2025-04-21 | [`CIRIS-Covenant.github.io@5ac7def`](https://github.com/CIRISAI/CIRIS-Covenant.github.io/commit/5ac7def) |
| [Wisdom-Based Deferral (WBD)](docs/wbd.md) | 2025-04-21 | [`CIRIS-Covenant.github.io@5ac7def`](https://github.com/CIRISAI/CIRIS-Covenant.github.io/commit/5ac7def) |
| [Meta-Goal M-1 / Adaptive Coherence](docs/m1-adaptive-coherence.md) | 2025-04-21 | [`CIRIS-Covenant.github.io@5ac7def`](https://github.com/CIRISAI/CIRIS-Covenant.github.io/commit/5ac7def) |
| [Wise Authority (WA)](docs/wise-authority.md) | 2025-04-21 | [`CIRIS-Covenant.github.io@5ac7def`](https://github.com/CIRISAI/CIRIS-Covenant.github.io/commit/5ac7def) |
| [Stewardship Tier](docs/stewardship-tier.md) | 2025-04-21 | [`CIRIS-Covenant.github.io@5ac7def`](https://github.com/CIRISAI/CIRIS-Covenant.github.io/commit/5ac7def) |
| [Conscience (faculty)](docs/conscience.md) | 2025-04-27 | [`CIRISAgent@4c01cc6b5`](https://github.com/CIRISAI/CIRISAgent/commit/4c01cc6b5) |
| [H3ERE](docs/h3ere.md) (Hyper3 Engine for Recursive Ethics / Hyper-Cubed Ethical Recursive Engine) | 2025-05-06 | [`CIRIS-Covenant.github.io@4f4715e`](https://github.com/CIRISAI/CIRIS-Covenant.github.io/commit/4f4715e) |
| [Coherence Ratchet](docs/coherence-ratchet.md) | 2025-10-31 | [`CIRISAgent@5e90974fb`](https://github.com/CIRISAI/CIRISAgent/commit/5e90974fb) |
| [RATCHET (reference architecture)](docs/ratchet.md) | 2026-01-03 | [`CIRISAI/RATCHET` repo creation](https://github.com/CIRISAI/RATCHET) |
| [CIRIS Federation](docs/federation.md) | 2026-01-02 | [`ciris-website@527d0d0`](https://github.com/CIRISAI/ciris-website/commit/527d0d0) |
| [Alignment Manifold](docs/alignment-manifold.md) | draft — public publication pending | (see file) |
| [CIRIS Constitution (CC)](docs/constitution.md) | 2026-06-17 | [`CIRISRegistry@fdc0614`](https://github.com/CIRISAI/CIRISRegistry/commit/fdc0614) |
| [CIRIS specification-and-test language](docs/spec-language.md) | 2025-05-31 | [`CIRISAgent@baa3f2484`](https://github.com/CIRISAI/CIRISAgent/commit/baa3f2484) |
| [CIRISClient: the screen](docs/client.md) | 2025-12-23 | [`CIRISAgent@4c25b5af7`](https://github.com/CIRISAI/CIRISAgent/commit/4c25b5af7) |
| [CEWPOS and the Attestation Calculus](docs/cewpos.md) | 2026-06-27 | [`CEWPOS@7778729`](https://github.com/CIRISAI/CEWPOS/commit/7778729) |
| [CIRISOntology](docs/ontology.md) | 2026-07-22 | [`CIRISOntology@f8f9011`](https://github.com/CIRISAI/CIRISOntology/commit/f8f9011) |
| [CIRISGrace](docs/grace.md) | 2026-08-16 | [`CIRISGrace@1fd7d9a`](https://github.com/CIRISAI/CIRISGrace/commit/1fd7d9a) |
| [CIRISHolon: the holon as certified view](docs/holon.md) | name 2026-08-26; object from 2026-08-19 ([`CIRISOntology@b770d72`](https://github.com/CIRISAI/CIRISOntology/commit/b770d72)) | [`CIRISHolon@d3993c8`](https://github.com/CIRISAI/CIRISHolon/commit/d3993c8) |
| [CIRIS Specification Document (CSD)](docs/csd.md) | 2026-09-07 | [`CIRISAgent@853a543d8`](https://github.com/CIRISAI/CIRISAgent/commit/853a543d8) |
| [CIRIS reality compiler](docs/reality-compiler.md) | application 2026-08-26; name from this record | [`CIRISHolon@d3993c8`](https://github.com/CIRISAI/CIRISHolon/commit/d3993c8) |
| [holon-draw](docs/holon-draw.md) | 2026-11-15 | [`CIRISHolon@8e56ace`](https://github.com/CIRISAI/CIRISHolon/commit/8e56ace) |
| [CIRIS Kernel (CIRISKernel)](docs/kernel.md) | 2026-11-12 | [`CIRISConstitution@b9a3fe3`](https://github.com/CIRISAI/CIRISConstitution/commit/b9a3fe3) |
| [CIRISISA: CIRIS Instruction Set Architecture](docs/isa.md) | this record (name and nature only) | derived from the CIRIS Kernel; public precursors CEWPOS (2026-06-27) and the specification-and-test language (2025-05-31) |

## Foundations, 2026

Four later entries are foundational to CIRIS:

- The **holon** ([CIRISHolon](docs/holon.md)) is one recursive object, a whole and a part at once. Its tiers are closed views of the level below that the level above carries, and any failure is certified by a witness pair.
- Applied to a physical model, it is a **[reality compiler](docs/reality-compiler.md)**: each tier is certified against the tier below for what the level above reads, within a stated budget, and the compiler refuses by name where no certificate exists.
- The **[CIRIS Kernel](docs/kernel.md)** is coordination without a coordinator, a new form of decentralized network that gives finality over both monotonic and non-monotonic operations. It is one function, with its proofs, by which a group talks, shares and governs itself with nobody in the middle. Self-organizing information on this CALM basis appears to have biological and physical implications too, which CIRIS is investigating as a hypothesis.
- **[CIRISISA](docs/isa.md)**, the CIRIS Instruction Set Architecture, extends the Kernel's primitives from governance to computation. Software built on it organizes itself: who works on what, in what order, and what counts as done are derived from signed causal facts, not assigned by a scheduler. This record gives its name and nature only. The specification will be published together with the governance and safety mechanisms it depends on.

## Citation

The canonical references are:

- **Software (initial)**: CIRIS AI. *CIRISAgent: open source ethical AI framework for accountable autonomy*. Zenodo (2025-09-24). DOI: [10.5281/zenodo.17195221](https://doi.org/10.5281/zenodo.17195221).
- **Software (updated)**: DOI: [10.5281/zenodo.18137161](https://doi.org/10.5281/zenodo.18137161) (2026-01-02).
- **Coherence Collapse Analysis**: *Coherence Collapse Analysis: A Universal Failure Mode in Complex Coordinating Systems*. Zenodo (2026-01-11). DOI: [10.5281/zenodo.18217688](https://doi.org/10.5281/zenodo.18217688).
- **Constrained Reasoning Chains**: *Constrained Reasoning Chains: An Empirical Telemetry Study of LLM Alignment*. Zenodo (2026-04-28). DOI: [10.5281/zenodo.19839280](https://doi.org/10.5281/zenodo.19839280).
- **Covenant text**: [`ciris_covenant.txt`](https://github.com/CIRISAI/CIRIS-Covenant.github.io/blob/main/public/ciris_covenant.txt).
- **Accord text**: [`ciris_accord.txt`](https://ciris.ai/ciris_accord.txt) on the canonical site.

For per-term provenance, see the term's file under [`docs/`](docs/).

## Methodology

For each term, we document:

1. **Earliest known public use** — the earliest verifiable public reference we have located. Sources prioritized in this order: peer-reviewed publication / Zenodo DOI; tagged release; git commit on a public repo; archived web page (Internet Archive Wayback Machine).
2. **Subsequent uses** — significant later references in the public record, e.g., subsequent papers, public-site pages, downstream documentation.
3. **Honest scope** — where CIRIS uses a compound term (e.g., *Coherence Ratchet*, *CIRIS Accord*, *Alignment Manifold*) the record claims priority on the compound, not on the constituent words taken alone. Common words with wide prior use are noted as such in each term's `scope_note`.

If you find an earlier verifiable reference than what is recorded here, please open an issue or pull request — we keep the record honest by correcting it.

## Structure

```
prior-use/
├── README.md                  # this file
├── prior-use.json             # structured per-term data
├── _schema/
│   └── prior-use.schema.json  # JSON Schema for prior-use.json
├── docs/                      # per-term Markdown files
└── evidence/                  # archival captures, when collected
```

## License

This record (the data and the prose around it) is dedicated to the public domain under [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/). Cite freely.

The CIRIS framework software it documents is licensed separately; see the per-repository LICENSE files in the [CIRISAI organization](https://github.com/CIRISAI).

## Contributing

Corrections and additions are welcome. Please:

1. For an existing term: open a pull request to the relevant `docs/<term>.md` and update `prior-use.json` accordingly.
2. For a new term: add a new file under `docs/`, add the entry to `prior-use.json`, and link it from the table above.
3. Provide a verifiable source (DOI, commit hash, or Wayback URL) for any earliest-use claim.
