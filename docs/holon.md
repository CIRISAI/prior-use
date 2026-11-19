---
term: "CIRISHolon"
category: architectural-component
earliest_known_public_use: "2026-08-26"
earliest_source_repo: "CIRISAI/CIRISHolon"
earliest_source_commit: "d3993c8"
earliest_source_url: "https://github.com/CIRISAI/CIRISHolon/commit/d3993c8"
object_lineage_earliest: "2026-08-19"
object_lineage_source_url: "https://github.com/CIRISAI/CIRISOntology/commit/b770d72"
scope_claimed: "the name 'CIRISHolon' / 'holon' for this object, and the specific combination: the closed view with a certified witness-pair failure, admission of a tier by carriage with a stated price, and the engine built on it with preregistered kills"
---

# CIRISHolon: the holon as certified view

In CIRIS, a **holon** is a component that is a whole and a part at once. It runs its own dynamics, and it is a coarse reading of finer holons.

- A view `v` of the level below is **Closed** when its square commutes: some update `h` on the coarse readings reproduces what the fine dynamics `T` does, `v ∘ T = h ∘ v`. Closed is the exact statement. The engine uses its approximate form, a non-expanding leak within a stated budget (`Budget.lean`).
- When a view is not closed, the failure is a certificate. A **witness pair** is two fine states the view cannot tell apart whose successors it can (`nonfactoring_iff_not_closed`).
- A **tier** is a Closed view that the level above *carries*, meaning one the level above cannot remove within its budget. A closed view that the level above does not carry is a **sector**, not a tier. The selector is whatever consumes the view, and a conservation law is one kind of consumer. (Corrections of 2026-09-25 and 2026-11-15 in `OBJECT.md`.)
- A *generated* scene has no fine motion to close over. It is certified differently, by an exact section law plus a transport cost against a frozen reference sample (`SceneCert.lean`).

The holon is foundational to CIRIS. Its first application is the [CIRIS reality compiler](reality-compiler.md).

## Earliest known public use

The object predates the name. All the commits below are on public `main` branches; the dates are commit dates.

- **2026-08-19 (object: the witness pair)**: [`CIRISOntology@b770d72`](https://github.com/CIRISAI/CIRISOntology/commit/b770d72), *"NonFactoring: the founding shape stated once, witnessed thrice"*.
- **2026-08-24 (object: Closed)**: [`CIRISOntology@1c883fa`](https://github.com/CIRISAI/CIRISOntology/commit/1c883fa), `def Closed (v : X → C) (T : X → X) : Prop := Factoring.Factors (v ∘ T) v`.
- **2026-08-26 (the square written literally)**: [`CIRISOntology@9cf05b7`](https://github.com/CIRISAI/CIRISOntology/commit/9cf05b7), `v ∘ T = h ∘ v`. Later the same day, [`45c53a8`](https://github.com/CIRISAI/CIRISOntology/commit/45c53a8) adds `nonfactoring_iff_not_closed`.
- **2026-08-26 (name)**: [`CIRISHolon@d3993c8`](https://github.com/CIRISAI/CIRISHolon/commit/d3993c8), *"Seed CIRISHolon: the object as engineering contract, verified"*. This is the first use of "holon" for the object and of the name CIRISHolon. (Earlier "holon" hits in CIRISOntology are "holonomy", a different word.)

## Subsequent significant uses

- 2026-09-25: tier versus sector, decided by the removability gate (`OBJECT.md` correction).
- 2026-11: the scene certificate for generated content (`SceneCert.lean`).
- 2026-11-15: the selector is the consumer of the view (`OBJECT.md` correction).

## Canonical definition (excerpt)

> The engine's unit is the **holon**: a component that is simultaneously a whole (it runs its own dynamics) and a part (it is a coarse reading of finer holons).

(Source: [`CIRISHolon/README.md`](https://github.com/CIRISAI/CIRISHolon). Read it with the README's 2026-11-15 correction: closure alone does not license running a tier in place of the one below.)

## Scope of priority claim

Neither the word nor the mathematics is CIRIS's:

- **Hierarchy and the word "holon"**: Herbert A. Simon, "The Architecture of Complexity" (*Proc. Am. Phil. Soc.* 106, 1962), and Simon and Ando on near-decomposability (*Econometrica*, 1961). Arthur Koestler, who drew on Simon, coined "holon" in *The Ghost in the Machine* (1967).
- **The commuting square for abstractions of dynamics**: lumpability of Markov chains (Kemeny and Snell, *Finite Markov Chains*, 1960), bisimulation (Park, 1981; Milner), and abstract interpretation (Cousot and Cousot, 1977).
- **Coarse-graining and closure in physics**: Mori–Zwanzig projection operators; renormalisation (Wilson, Kadanoff); and TICA/VAMP, which the engine uses as an instrument (credited in `TIERS.md` §5).
- **Emergence and closure**: Barnett and Seth (dynamical independence), Rosas et al. (causal emergence), Shalizi and Crutchfield (computational mechanics), Krakauer et al. (information theory of individuality), Montévil and Mossio (closure of constraints), Kolchinsky and Wolpert (semantic information), and Kabernik (quantum coarse-graining).
- **The selection rule**: the information bottleneck (Tishby, Pereira and Bialek, 1999).
- **Convergent independent work**: "Six Birds" (Tsiokos, arXiv [2602.00134](https://arxiv.org/abs/2602.00134), [2604.03239](https://arxiv.org/abs/2604.03239)), stated as relative lumpability. No citation runs in either direction. CIRISHolon records it as corroboration, not as a priority contest.

CIRIS does not claim the commuting square or the idea of closure, both of which are standard. It claims priority on the name **"CIRISHolon"**, on "holon" for this object, and on the **specific combination**: the closed view with a certified witness-pair failure, admission of a tier by carriage with a stated price, and an engine built on that object with preregistered kill conditions. This matches the verdict in CIRISHolon's own `PRIOR_ART.md`.
