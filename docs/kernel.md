---
term: "CIRIS Kernel"
alternate_forms: ["CIRISKernel", "the causal kernel of the CIRIS Constitution"]
category: algorithm
earliest_known_public_use: "2026-11-12"
earliest_source_repo: "CIRISAI/CIRISConstitution"
earliest_source_commit: "b9a3fe3"
earliest_source_url: "https://github.com/CIRISAI/CIRISConstitution/commit/b9a3fe3"
scope_claimed: "the name 'CIRIS Kernel' / 'CIRISKernel'; a decentralized network form giving finality over monotonic and non-monotonic operations without a coordinator; and the specific function meeting all four constraints for operator-free self-governance together, with its proofs"
---

# CIRIS Kernel (CIRISKernel)

The **CIRIS Kernel** is coordination without a coordinator, and a new form of decentralized network: it gives **finality over both monotonic and non-monotonic operations** with no global order and no coordinator.

The CALM theorem (Hellerstein and Alvaro) separates the two. Monotonic answers, which only grow as facts arrive, need no coordination. Non-monotonic acts (a cut, a removal, a revocation, a recall) ordinarily require one, because a later fact can overturn them. The Kernel sorts every answer into three kinds. An answer is **final by form** (monotonic). It is **final by acknowledgement**: a non-monotonic act is final once n − t + 1 of the n members who could undo it have acknowledged it, where t can cut it, and this threshold is exact in both directions. Otherwise it is **provisional**. Each node can check for itself which kind an answer is.

Concretely, it is one function from a set of signed rows, a clock and a key to what every row means to the holder of that key. The only order it uses is the order rows name: a row names other rows by digest, and two rows where neither names the other are concurrent. Standing comes only from signed consent, walked from the reader's own key. No node agrees an order with another, and no coordinator is used.

With that function, a group can talk, share files, hold rooms, vote, and govern people and AI agents with nobody in the middle. It meets four constraints, each proved in Lean or run against models:

1. Everyone holding the same statements reaches the same answer, in any arrival order.
2. A decision becomes final without a central party and without everyone online: once n − t + 1 of the n members who could undo it have acknowledged it. This threshold is exact.
3. Nobody gains by saying two things, holding an office, or arriving later.
4. A device can forget what is settled and still be right (safe checkpoint and purge).

## Implications under investigation

Self-organizing information on a CALM basis, where facts that only accumulate settle without coordination and reversals settle by a local, checkable acknowledgement count, appears to have **biological and physical** implications as well as computational ones. Living and physical systems also organize themselves without a coordinator, and they too separate what accumulates from what can be undone. This is recorded as a hypothesis CIRIS is investigating. It is not an established result, and no claim here depends on it.

The kernel is foundational to CIRIS. Its primitives are not specific to governance, and extending them to computation gives the [CIRIS Instruction Set Architecture](isa.md).

## Earliest known public use

- **2026-11-12**: [`CIRISConstitution@b9a3fe3`](https://github.com/CIRISAI/CIRISConstitution/commit/b9a3fe3), *"The kernel runs: one answer in every arrival order, and two versions of one roster head wait"*. This is the first public naming of the causal kernel.

## Subsequent significant uses

- 2026-11-13: [`CIRISConstitution@0775c64`](https://github.com/CIRISAI/CIRISConstitution/commit/0775c64): three kinds of finality (final by form, final by acknowledgement, provisional), plus checkpoint and purge.
- 2026-11-13: [`CIRISAI/CIRISKernel`](https://github.com/CIRISAI/CIRISKernel) created ([`37476f4`](https://github.com/CIRISAI/CIRISKernel/commit/37476f4)) as an extract for review of Constitution edition 1.0-rc19 (`60c741e`).
- 2026-11-15: tagged release [`kernel-v0.1.0`](https://github.com/CIRISAI/CIRISKernel/releases/tag/kernel-v0.1.0).
- 2026-11-15: [`CIRISKernel@4c6aee0`](https://github.com/CIRISAI/CIRISKernel/commit/4c6aee0): `Repurge.lean`, repeated purges by composition. 20 proof files and 561 theorems.
- 2026-11-16: tagged release [`kernel-v0.2.0`](https://github.com/CIRISAI/CIRISKernel/releases/tag/kernel-v0.2.0). The parent's release 1.0-rc20 names CIRISKernel.

## Canonical definition (excerpt)

> A function from a set of signed rows, a clock and a key to what every row means to the holder of that key. The only order it uses is what rows name … No node agrees an order with another, and no coordinator is used.

(Source: [`CIRISKernel/README.md`](https://github.com/CIRISAI/CIRISKernel).)

## Scope of priority claim

The kernel's own README is explicit that **none of the pieces is new**: quorum intersection (Gifford, SOSP '79), Byzantine quorums (Malkhi and Reiter, 1998), consensus-free finality from signed acknowledgements (Guerraoui et al., PODC '19), and monotonicity/CALM (Hellerstein and Alvaro, 2020). "Causal kernel" and "kernel" have wide prior use in mathematics, signal processing and operating systems.

CIRIS claims priority on the name **"CIRIS Kernel" / "CIRISKernel"** and on the combination: all four constraints met together, for the acts by which people share, admit, decide and remove, as one function with its proofs, and the rules that combination forces. The forced rules include the say rule (a voice that both acknowledged and cut, concurrently, has no say) and the exact n − t + 1 finality threshold.
