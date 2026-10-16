# Product Lifecycle Documentation (`product/`)

This directory holds the living **AntIntent** System of Record and slice artifacts for the project. All files in `product/` (along with `/AGENTS.md`) are tracked exclusively on the local `lifecycle` Git branch (mounted via `git worktree` in `/.lifecycle/`) and are ignored on all application code branches via `.gitignore`.

## Structure

- **`intent.md`** *(System of Record, created from `_templates/intent.md`)* — Living document capturing the current product problem statement, desired outcomes, target users, constraints, and open questions.
- **`spec.md`** *(System of Record, created from `_templates/spec.md`)* — Living document capturing the current technical and product design, evaluated alternatives, architecture boundaries, and system invariants.
- **`slices/<slice-slug>/`** *(instantiated from `_templates/slices/slice-slug/`)* — Holds per-slice artifacts for each vertical increment:
  - `plan.md` — Under-the-hood mechanics, affected files, step-by-step tasks, and completion criteria.
  - `validations.md` — Automated test harness definitions, integration checks, and step-by-step user validation scenarios.
  - `experiments.md` — Hypotheses, spikes, benchmarks, and rejected alternatives explored during design or build.
  - `artifacts.md` — Traceability ledger linking the slice to code branch names, commit SHAs, test outputs, and supplementary docs.
- **`_templates/`** — Canonical Markdown templates used to bootstrap new intents, specs, and vertical slices.

## Inspecting Lifecycle History

From the workspace root, run:
```bash
git log lifecycle --stat
```

## Active Work Index

| Artifact / Slice | Status | Description |
| :--- | :--- | :--- |
| `product/intent.md` | Not started | Copy from `_templates/intent.md` when beginning the first intent. |
| `product/spec.md` | Not started | Copy from `_templates/spec.md` after `intent.md` is approved. |
