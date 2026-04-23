# Omer El Idrissi

**Firmware Engineer** | Linux Kernel Contributor | Systems & USB

- LinkedIn: https://www.linkedin.com/in/omer-el-idrissi-921a073a1/ 
- Email: omer.e.idrissi@gmail.com

---

## Core Competencies for Firmware Roles

- **Embedded & Kernel**: Linux staging drivers, USB isochronous transfers, interrupt handling, DMA
- **Performance Critical**: SIMD, cache-friendly data layouts (PPM lib)
- **Static Analysis**: libclang-based data dependency analysis, control-flow graphs
- **Hardware Adjacent**: Physical microphone integration, isochronous endpoints, timing constraints
- **Toolchain**: C (primary), Python for automation, Git

---

## Featured Projects (Relevant to Firmware)

| Project | Tech | What it shows firmware folks |
|---------|------|-------------------------------|
| **cachepix** | C, SIMD | Compile-time selected SIMD backend, loop vectorization -> directly maps to DSP/ISP firmware |
| **fifine_mic_driver** | C, Linux USB stack | Isochronous endpoint handling, URB lifecycle, real-time audio streaming |
| **prongc** | C, libclang | Dataflow across functions — useful for firmware safety analysis and untangling messy codebases |

---

## Linux Kernel Contributions

- `drivers/staging/`: [brief — e.g., “Code refactoring for cleaner error returns” or “Changing use of non-standard vendor-defined macros”]
- Upstream link: [https://lore.kernel.org/linux-staging/, look up "Omer El Idrissi"]

---

## Why this matters for firmware

- **Real-time & isochronous** – Handled jitter, scheduling, ring buffer management at USB frame level (multi-producer, single-blocked-consumer model).
- **Cache optimization / SIMD** – Proven ability to leverage CPU cache hits with cache-aware data structure designs.
- **Static analysis tool** – Analyzes data dependencies before runtime; critical for analyzing messy codebases.

---

## Quick resume

includes details on:
- Reverse-engineered USB descriptor parsing for custom microphone
- SIMD PPM library achieving 
- libclang tool to detect cross-function data dependency

