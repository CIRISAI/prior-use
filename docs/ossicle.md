---
term: "CIRISOssicle"
category: system
earliest_known_public_use: "2026-01-10"
earliest_source_repo: "CIRISAI/CIRISOssicle"
earliest_source_commit: "6d232ad"
earliest_source_url: "https://github.com/CIRISAI/CIRISOssicle/commit/6d232ad"
scope_claimed: "the name 'CIRISOssicle' and the ossicle sensor: a sub-kilobyte, software-only GPU workload detector built from coupled chaotic oscillators read as a timing strain gauge"
---

# CIRISOssicle

**CIRISOssicle** detects unauthorized GPU workloads, such as crypto mining or resource hijacking, in software only, with no external hardware. The sensor is three coupled chaotic oscillators of 64 cells each, which is **768 bytes** of state. Its timing is read at 4,000 Hz as a strain gauge. The name is an analogy to the inner ear: smaller sensors turned out to be more sensitive, not less.

**Validated** (experiments O1–O7, January 2026): workload detection down to 1% load, with 100% true positives and 0% false positives in those runs, and 2.5 ms latency. A timing-based random number source measured at 7.99 bits per byte.

**Theorized, not validated**: detection of EMI, VDF and thermal effects. A 1.1° twist between oscillators gave about 21× sensitivity on one GPU. Its numerical coincidence with graphene's magic angle is recorded as an observation, with causation unproven.

Licensed under BSL 1.1 by CIRIS L3C, changing to AGPL-3.0 on 2030-01-01.

## Earliest known public use

- **2026-01-10**: [`CIRISOssicle@6d232ad`](https://github.com/CIRISAI/CIRISOssicle/commit/6d232ad), *"Initial commit: CIRISOssicle GPU Tamper Detection"*. The repository's `PRIOR_ART.md` is dated 2026-01-09.

## Subsequent significant uses

- 2026-01-10: [CIRISArray](array.md) extends single sensors to arrays.
- 2026-01-11: [`167291c`](https://github.com/CIRISAI/CIRISOssicle/commit/167291c), claims validated by null-hypothesis testing.

## Scope of priority claim

Prior art includes power and timing side-channel analysis, GPU performance-counter monitoring, chaotic oscillators as sensors, and timing-jitter random number generation. CIRIS claims priority on the name **"CIRISOssicle"** and on the specific sensor: a sub-kilobyte, software-only detector of coupled chaotic oscillators, read by mean shift at a fixed sample rate. The claims are stated at the evidence level the repository assigns them.
