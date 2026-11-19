---
term: "holon-draw"
category: architectural-component
earliest_known_public_use: "2026-11-15"
earliest_source_repo: "CIRISAI/CIRISHolon"
earliest_source_commit: "8e56ace"
earliest_source_url: "https://github.com/CIRISAI/CIRISHolon/commit/8e56ace"
scope_claimed: "the name 'holon-draw' and its rule that a drawn scene is a view of a list, applying the holon's closed-versus-carried distinction to the screen"
---

# holon-draw

**holon-draw** is the draw core of the [CIRISHolon](holon.md) engine. It has no dependencies. Its one rule is that **a drawn scene is a view of a list**:

- Every mark a person can pick or act on is one row of a list the consumer holds, under one stable tag.
- A mark with no row is decoration. It cannot be picked, carries no value, and is labelled as decoration wherever a person could mistake it for data.

This is the holon's closed-versus-carried distinction applied to the screen: a mark is carried when a consumer reads it. It pairs with the CIRIS Kernel's result that **the screen is the same function**, meaning that what a person is offered, what an act would change, and whether the door admits it are one answer.

The core packs tiles of tagged 52-byte instance records, one batch per tile and kind. It also provides:

- a pure pick that names an instance,
- a per-frame digest,
- a detail allocator,
- a plain WebAssembly boundary.

It is hosted in two ways: as a canvas inside a client, or as the whole screen, as in [CEWPOS](cewpos.md). In the whole-screen case it composes the 24 UX primitives of the CIRIS screen standard. Companion crates `holon-draw-atoms` and `holon-draw-ladder` draw the engine's atomic and scale-ladder views.

## Earliest known public use

- **2026-11-15**: [`CIRISHolon@8e56ace`](https://github.com/CIRISAI/CIRISHolon/commit/8e56ace), *"holon-draw: a generic draw core with no dependency"* (`engine/crates/holon-draw`). The seam contract with consumers is [`INTERFACE.md`](https://github.com/CIRISAI/CIRISHolon/blob/main/INTERFACE.md), written the same day.

## Subsequent significant uses

- 2026-11-15: the CEWP twin's street-leaf builder was re-implemented on this side of the seam. On 2,000 synthetic leaves it matched the twin byte for byte, with 0 of 27,090,780 floats differing, and ran 6.8× faster in WebAssembly. These are synthetic buffers, not the twin's real leaves.
- 2026-11-15: `holon-draw-ladder` became the scale-ladder adapter the CEWP twin calls.

## Scope of priority claim

The techniques are standard: instanced rendering, GPU picking, model–view separation, and "UI as a function of state" (Elm, React). CIRIS claims priority on the name **"holon-draw"** and on its rule: every pickable mark is a carried row of a consumer's list, and anything else is labelled decoration. That ties the holon's closure and carriage to what a person is shown.
