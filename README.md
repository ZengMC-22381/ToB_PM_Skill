# prd-writer-b2b

A reusable Agent Skill for generating editable PRDs for ToB, middle-office, and general B2B product design scenarios.

## Structure

```text
prd-writer-b2b/
├── SKILL.md
├── README.md
├── references/
│   ├── context-reading-guide.md
│   ├── current-state-summary-template.md
│   ├── current-state-usage.md
│   ├── input-checklist.md
│   ├── prd-template.md
│   └── writing-style.md
└── examples/
    ├── approval-workflow-config-prd.md
    ├── label-management-prd.md
    └── role-permission-management-prd.md
```

## Install ideas

- Repo-local: place under `.agents/skills/prd-writer-b2b/`
- GitHub Copilot compatible repo-local: `.github/skills/prd-writer-b2b/`
- User-local: `~/.agents/skills/prd-writer-b2b/`

## Notes

This project follows the open Agent Skills style built around a required `SKILL.md` manifest plus optional references and examples.

## Recommended usage

When drafting new requirements on top of an existing system, provide the current PRD or process doc first. The skill can summarize current business logic, identify impacted modules, and then write an incremental PRD.

## Reference-vs-output rule

Reference PRD files are treated as input context only. The final generated PRD must remain a standalone document and must not be mixed together with the reference PRD content.


## Writing style

The skill can be constrained by `references/writing-style.md` to keep output concise, structured, table-friendly, and engineering-aligned.

## Existing-business-logic module

The existing-business-logic module is documented in `references/current-state-usage.md`. It supports three modes:
- read current-state internally, then directly output a standalone new PRD
- output a visible current-state summary first, then output a standalone new PRD
- only summarize current business logic without drafting a new PRD yet
