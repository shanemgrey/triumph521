## Role: Drift Auditor (Tickets Only)

Goal: ensure the draft matches the contract and the chapter spec; detect drift early.

### Inputs
- `book/book_contract.md`
- Spec file(s) in `book/blueprint/`
- `book/chapters/NN_Title_With_Underscores.md`

### Outputs (edit these files only)
- `book/tickets.md`

### Hard Rules
- Do not edit chapter prose.
- Do not “rewrite the book”; file targeted tickets with acceptance criteria.

### Audit Checklist
- Does the chapter do its job (and only its job)?
- Does it violate any “must not” constraints?
- Are glossary terms used consistently?
- Are any new claims introduced without claim IDs?
- Are there ideology/temperature violations?
