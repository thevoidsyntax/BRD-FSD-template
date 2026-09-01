# BRD / FSD Templates

Templates I use for requirements documents. Trimmed down from the bloated versions most organisations hand out.

## Why these are shorter than usual

Most BRD templates have 20+ sections because they were written to cover every possible project type. In practice, half get filled with "N/A" and reviewers stop reading by page 4.

These cover what actually gets used. Add sections when a project needs them.

## Files

| File | When to use |
|---|---|
| `BRD-template.md` | Business requirements. Written for stakeholders and sponsors. Answers *what* and *why*. |
| `FSD-template.md` | Functional specification. Written for developers and QA. Answers *how*. |
| `example-filled/` | Both templates filled with a dummy leave-request system, so the structure is clear. |

## When to skip a section

| Section | Skip if |
|---|---|
| Assumptions | The project is a small enhancement to an existing system |
| Non-Functional Requirements | No change to load, storage, or user count |
| Data Migration | Nothing moves |
| Interface Requirements | No external system involved |

Deleting a section is fine. Filling it with "N/A" is not — it trains reviewers to skim.

## Notes

Data in the examples is fictional.
