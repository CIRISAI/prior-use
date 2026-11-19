---
term: "CIRISArray"
category: system
earliest_known_public_use: "2026-01-10"
earliest_source_repo: "CIRISAI/CIRISArray"
earliest_source_commit: "f4ad779"
earliest_source_url: "https://github.com/CIRISAI/CIRISArray/commit/f4ad779"
scope_claimed: "the name 'CIRISArray' and the extension of the ossicle sensor to massive arrays of coupled oscillators on GPUs"
---

# CIRISArray

**CIRISArray** extends single-point [CIRISOssicle](ossicle.md) sensors to massive arrays of coupled oscillators on GPUs. It is research-grade software.

**Validated** (January 2026):
- GPU workload detection by mean shift: +83% at 1% load, 1.3 ms latency.
- A GPU timing true random number generator at 120 kbps.
- A thermalisation time of τ = 46.1 ± 2.5 s.

**Not validated**: detection of EMI, temperature and VFD effects, and cross-device coherence. Frequency peaks were not reproducible across runs.

Licensed under BSL 1.1 by CIRIS L3C.

## Earliest known public use

- **2026-01-10**: [`CIRISArray@f4ad779`](https://github.com/CIRISAI/CIRISArray/commit/f4ad779), *"Initial release of CIRISArray"*.

## Scope of priority claim

Sensor arrays, side-channel analysis and timing-based random number generation are established fields. CIRIS claims priority on the name **"CIRISArray"** and on arrays of ossicle sensors as described, at the evidence levels the repository states.
