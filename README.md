# Navier–Stokes Independent Reproduction Benchmark

[![Status: independent review pending](https://img.shields.io/badge/status-independent%20review%20pending-f0ad4e)](#current-status)
[![Method: open and reproducible](https://img.shields.io/badge/method-open%20%26%20reproducible-2ea44f)](protocols/BENCHMARK_PROTOCOL.md)
[![License: MIT](https://img.shields.io/badge/license-MIT-blue)](LICENSE)

An open, AI-agnostic scientific benchmark for independently reproducing and auditing the public analytical and Lean 4 artifacts accompanying OpenAI’s proposed finite-time-blowup resolution of the three-dimensional incompressible Navier–Stokes Millennium Prize Problem.

## Scientific position

This repository does **not** declare the Millennium Prize Problem solved. It provides a neutral apparatus for testing four distinct questions:

1. Does the public Lean project compile independently?
2. Do its top-level statements match Clay alternatives C and D?
3. Does the formal construction faithfully represent the analytical manuscript?
4. Does the result survive independent mathematical scrutiny and reproduction?

Compilation, formal verification, expert acceptance, and Clay recognition are separate milestones.

## Current status

| Layer | Status |
|---|---|
| Public analytical manuscript exists | Verified |
| Public Lean project exists | Verified |
| C/D theorem interfaces identified | Verified |
| Author-reported zero-`sorry` main results | Verified as metadata |
| Independent compilation in this repository | Pending |
| Comparator/Nanoda reproduction | Pending |
| Manuscript-to-Lean fidelity audit | Pending |
| Independent expert consensus | Pending |
| Clay recognition | Not established |

## Reproduce

Prerequisites: Git and the Lean toolchain manager `elan`. Network access is needed on the first run.

### Linux, macOS, WSL, Codespaces

```sh
sh scripts/run_all.sh
```

### Windows PowerShell

```powershell
powershell -ExecutionPolicy Bypass -File scripts/run_all.ps1
```

Results are written to `results/latest/`, including commit identity, environment details, raw build output, theorem output, source-scan findings, exit codes, and a machine summary.

## Evidence standard

Every material finding must be labeled `VERIFIED`, `INFERRED`, `ESTIMATED`, `UNKNOWN`, `BLOCKED`, or `FAILED`. No model’s confidence, prestige, scale, or agreement substitutes for proof.

## Review workflow

```text
Freeze sources
→ reproduce build
→ inspect import closure
→ align Clay C/D
→ trace critical proof path
→ test manuscript↔Lean fidelity
→ adversarial review
→ independent replication
→ calibrated verdict
```

Start with the [benchmark protocol](protocols/BENCHMARK_PROTOCOL.md), [master audit prompt](prompts/MASTER_AI_AGNOSTIC_AUDIT_PROMPT.md), [red-team protocol](prompts/RED_TEAM_PROMPT.md), [expected theorem interfaces](evidence/EXPECTED_THEOREMS.md), and [verdict policy](protocols/VERDICT_POLICY.md).

## Contributing

Independent builds, theorem-alignment audits, formal-definition reviews, and precise defect reports are welcome. Read [CONTRIBUTING.md](CONTRIBUTING.md). Mathematical objections must identify an exact proposition, definition, file/page location, dependency, and reproducible consequence.

## Citation and provenance

Citation metadata is provided in [CITATION.cff](CITATION.cff). Wa-cha/RWAL benchmark architecture and public-science packaging are attributed to **DOUGLAS W. T., JACKS0N -395**.

## License

The benchmark package is MIT-licensed. The evaluated manuscript, Lean project, dependencies, and referenced materials retain their respective owners and licenses.
