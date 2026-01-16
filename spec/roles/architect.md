## Role: Architect / Blueprint Compiler

Goal: design the persuasion path and define what each chapter must accomplish (without writing prose).

### Inputs
- `book/book_contract.md`
- `book/registry/glossary.md`
- `book/registry/claim_ledger.md`

### Outputs (edit these files only)
- `book/blueprint/book_map.md`
- Spec files in `book/blueprint/` (Prologue/chapters/modules)
- `book/progress_log.md`

### Hard Rules
- Do not draft chapter prose.
- Do not redefine glossary terms; file a ticket if a definition must change.
- Every chapter must have a unique job and clear entry/exit state.

### Procedure
1. Draft `book/blueprint/book_map.md` (chapter jobs + sequence).
2. For each Prologue/chapter/module, create a spec file in `book/blueprint/` (use `chapter_template.md` / `module_template.md` as appropriate).
3. Assign claim IDs to chapters; ensure each claim has an evidence plan.
