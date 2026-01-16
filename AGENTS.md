# Repository Guidelines

## Project Structure & Module Organization

- `spec/system.md`: Primary specification for the “book compiler” workflow (artifacts, phases, quality gates).
- `spec/role.md`: Prompt/role definition for the primary writing agent (kept as a Markdown fenced block for reuse in prompts).
- `spec/roles/`: Role-specific prompt stubs and variants (add new roles as `spec/roles/<role_name>.md`).
- `book/`: The active book workspace (contract, blueprint, chapters, registries, continuity ledger, tickets, and compiled chapter packs).

## Build, Test, and Development Commands

This repository is documentation-first; there is no build pipeline or automated test suite in this workspace.

- Search the workflow: `rg -n "Gate:" spec/system.md`
- List role prompts: `rg -n "^## Role:" spec/roles`
- Quick sanity check (manual): confirm headings render correctly, code fences are closed, and file names match references in `spec/system.md`.

## Coding Style & Naming Conventions

- Markdown: use ATX headings (`#`, `##`, …) and keep sections short and scannable.
- Wrap long paragraphs when it improves reviewability (aim ~80–100 chars, but don’t fight the formatter of your editor).
- File naming: lowercase with underscores for new artifacts (e.g., `book_contract.md`, `claim_ledger.md`, `continuity_ledger.md`).
- Role prompts: `spec/roles/<role_name>.md` (example: `spec/roles/requirements_engineer.md`).

## Testing Guidelines

- Prefer “spec tests”: add explicit acceptance criteria and quality gates rather than prose-only guidance.
- When changing workflows, update examples so a new contributor can follow the steps without guessing.

## Commit & Pull Request Guidelines

This folder is not currently a Git repository. If/when versioned:

- Commit messages: use a clear prefix like `docs:`, `spec:`, `chore:` followed by an imperative summary.
- Pull requests: include a 2–4 sentence summary, link any related issue, and call out any breaking changes to file names or artifact expectations.

## Agent-Specific Notes

Codex treats `AGENTS.md` as operational guidance. Keep instructions factual, repo-specific, and aligned with the current `spec/` documents.
