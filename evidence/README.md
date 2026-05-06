# Evidence

This directory holds archival captures of the sources cited in the prior-use record. It is populated incrementally as captures are made.

## Subdirectories

- `wayback/` — Internet Archive Wayback Machine capture URLs and PDF/HTML snapshots
- `arxiv/` — arXiv preprint records (where applicable)
- `zenodo/` — Zenodo DOI records and metadata snapshots
- `git/` — git commit metadata (`git show <sha> --stat`) and trees pinned at significant SHAs

## Format

Each evidence file is named after the term and source it documents, e.g., `wayback/coherence-ratchet-20260212.html` for the 2026-02-12 Wayback snapshot of the canonical `/coherence-ratchet` page.

## Status

Initial bootstrap — captures pending. The structured record in [`../prior-use.json`](../prior-use.json) and the per-term files under [`../docs/`](../docs/) carry the citations themselves; this directory holds the archival copies for completeness.
