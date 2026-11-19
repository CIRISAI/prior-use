---
term: "CIRISISA"
expansion: "CIRIS Instruction Set Architecture"
category: architectural-component
earliest_known_public_use: null
earliest_source_note: "First public naming is the commit adding this file to CIRISAI/prior-use."
scope_claimed: "the name 'CIRISISA' / 'CIRIS Instruction Set Architecture' and the extension of the CIRIS Kernel's coordination primitives from governance to computation, giving self-organizing software"
---

# CIRISISA: CIRIS Instruction Set Architecture

**CIRISISA** is the [CIRIS Kernel](kernel.md), slightly extended, used as an instruction set. The kernel's primitives govern who may act and when an act is final: causal admission over signed rows, digest-named dependencies, consent-based authority, cuts, receipts, acknowledgement finality, and safe checkpoints. In CIRISISA the same primitives coordinate computation.

What follows from this:

- **Partial order as the execution model.** Work is a causal graph, not a global instruction sequence. Sequential execution is a special case. Parallel execution is the natural case. Synchronization is a causal dependency.
- **No global scheduler.** Each worker derives for itself, from the rows it holds, what work is available, what it is authorized to do, what has been cancelled, and what may be committed, the way each member derives a group's state under the kernel.
- **One substrate for computation and for the authority to compute.** The mathematics that settles a governance act settles a computation's result. Execution, validation and settlement are kept distinct.
- **Self-organizing software.** Software built this way organizes itself: who works on what, in what order, and what counts as done are derived from signed causal facts and not assigned by a coordinator.

## Disclosure

This entry records the name and nature of CIRISISA and its place in the CIRIS lineage. The specification will be published together with the governance and safety mechanisms it depends on.

## Earliest known public use

- **This record**: the commit adding this file to [`CIRISAI/prior-use`](https://github.com/CIRISAI/prior-use) is the first public naming.
- **Derived from**: the [CIRIS Kernel](kernel.md), public from 2026-11-12.

## Scope of priority claim

Executing a partial order instead of a sequence has long prior art: dataflow architectures (Dennis and Misunas, 1975; Arvind's tagged-token machine), actor models (Hewitt, 1973), and task-graph runtimes. "Instruction set architecture" is a standard term. CIRIS claims nothing on those.

CIRIS claims priority on the name **"CIRISISA" / "CIRIS Instruction Set Architecture"** and on the specific idea: using the CIRIS Kernel's causal admission, consent-based authority and acknowledgement finality as the coordination substrate of computation, so that one function governs both computation and the authority to perform it.
