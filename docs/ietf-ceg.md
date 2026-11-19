---
term: "draft-moore-scitt-ciris-ceg"
category: protocol
earliest_known_public_use: "2026-10-23"
earliest_source_url: "https://datatracker.ietf.org/doc/draft-moore-scitt-ciris-ceg/"
scope_claimed: "the CIRIS Epistemic Grammar as specified to the IETF: signed attestation rows of five types, composite post-quantum signatures, and named refusals, in relation to SCITT"
---

# IETF Internet-Draft: Signed Attestation Rows of the CIRIS Epistemic Grammar and Their Relationship to SCITT

`draft-moore-scitt-ciris-ceg` specifies **CEG**, the CIRIS Epistemic Grammar, for the IETF. It also relates CEG to SCITT (Supply Chain Integrity, Transparency and Trust). This is the wire grammar of the [CIRIS Constitution](constitution.md).

From the abstract:
- CEG records claims between parties as **signed rows**.
- Each row is one or more COSE_Sign1 messages over deterministically encoded CBOR.
- Each message carries one composite **ML-DSA-65 and Ed25519** signature.
- Every row has one of **five types**: a claim, a delegation, a replacement, a withdrawal, or a recantation.
- A node admits a row only after a fixed set of checks, and **refuses a failing row with a named reason**.

## Earliest known public use

- **2026-10-23**: [`draft-moore-scitt-ciris-ceg-00`](https://datatracker.ietf.org/doc/draft-moore-scitt-ciris-ceg/00/) posted on the IETF Datatracker. It was built and committed in CIRISConstitution at [`06be273`](https://github.com/CIRISAI/CIRISConstitution/commit/06be273) on 2026-10-21.

## Subsequent significant uses

- 2026-11-17: [`-01`](https://datatracker.ietf.org/doc/draft-moore-scitt-ciris-ceg/01/) posted on the Datatracker (committed at [`90f3c31`](https://github.com/CIRISAI/CIRISConstitution/commit/90f3c31), merged to `main` at [`c2f4d7f`](https://github.com/CIRISAI/CIRISConstitution/commit/c2f4d7f)).
- 2026-11-17: review requested on the `scitt@ietf.org` mailing list, with the [CIRIS Web4](web4.md) white paper attached.

## Scope of priority claim

COSE, CBOR, ML-DSA, Ed25519 and SCITT are IETF and NIST work, and the draft builds on them. CIRIS claims priority on **CEG** as specified there: the closed set of five row types, the fixed admission checks with named refusals, and their mapping to SCITT. The draft is an individual submission. It is not an IETF standard or a working-group document.
