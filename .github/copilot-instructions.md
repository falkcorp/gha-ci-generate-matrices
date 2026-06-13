<!-- file: .github/copilot-instructions.md -->
<!-- version: 2.4.0 -->
<!-- guid: 4d5e6f7a-8b9c-0d1e-2f3a-4b5c6d7e8f9a -->
<!-- last-edited: 2026-06-13 -->

# gha-ci-generate-matrices — Additional Context

Org-wide coding standards (file headers, language rules, commit format) are at
**<https://github.com/falkcorp/.github>** and apply automatically to this repo.

For full project context: **CLAUDE.md** at the repo root.

## Project overview

GHA composite action: generate CI build matrices. Language: Python/YAML.
This action generates build matrices for GitHub Actions CI workflows, enabling
parallel builds across different configurations.

## Key directories

- `src/` — Python source for matrix generation logic
- `template/` — Matrix templates

## Critical constraints

- This is a GHA composite action — `action.yml` is the entry point
- Python code runs inside GitHub Actions runner environment
- Keep the action interface stable (inputs/outputs in `action.yml`)
