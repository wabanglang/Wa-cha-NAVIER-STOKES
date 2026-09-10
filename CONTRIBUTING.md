# Contributing

Contributions should increase reproducibility, falsifiability, or clarity without overstating the proof’s validation status.

## Accepted contributions

- independently generated build and Comparator logs;
- theorem-to-specification mappings;
- import-closure and axiom analyses;
- manuscript-to-Lean fidelity tables;
- focused mathematical checks of critical lemmas;
- reproducible defect reports;
- portability and documentation improvements.

## Required evidence for a mathematical issue

Include the exact source version, file/page and proposition, statement, hypotheses, dependencies, minimal counterargument or failing test, severity, downstream impact, and reproduction instructions.

Use one of: `NOT_A_DEFECT`, `PRESENTATIONAL`, `LOCAL_REPAIRABLE`, `MAJOR`, `THEOREM_FATAL`, or `UNRESOLVED`.

## Independence disclosure

State any affiliation with the proof authors, competing projects, model providers, funders, or prior review teams. AI assistance is permitted but must be disclosed with model, version, protocol version, tools, and human verification performed.

## Pull requests

- keep raw evidence separate from interpretations;
- do not rewrite or delete prior run evidence;
- update `CHANGELOG.md`;
- ensure JSON remains valid and shell scripts pass syntax checks;
- version any acceptance-criteria change made after results are known.

