# LX Obsidian Labs — Portfolio Evaluation Standard

## Principle

**Maturity is not quality.** An alpha release may demonstrate exceptional engineering; a deployed application may have serious deficiencies. Never deduct quality points solely because a planned feature is incomplete.

## Three independent signals

| Signal | Allowed values | Purpose |
| --- | --- | --- |
| Stage | Planned / Prototype / Active Development / Beta / Production / Maintenance | Describes the product lifecycle, not merit |
| Verification | Not yet verified / Partially verified / Verified for stated scope | Describes available reproducible evidence |
| Engineering assessment | Evidence-based score out of 10, or Not assessed | Evaluates work that exists and is claimed |

**Stage labels must be substantiated by the project's README, release history or maintained roadmap.** When evidence is insufficient, use **Stage: To confirm** rather than inventing a status.

## Scoring rubric (100 points)

| Dimension | Weight | What reviewers inspect |
| --- | ---: | --- |
| Architecture and technical decisions | 20 | Cohesion, modularity, trade-offs, maintainability |
| Implemented correctness | 20 | Functional behavior in stated scope, edge cases |
| Security and data handling | 20 | Trust boundaries, secrets, authorization, privacy |
| Testing and reproducibility | 15 | Relevant tests, CI evidence, reproducible setup |
| Developer experience and documentation | 15 | README, setup, limitations, API/contracts, provenance |
| UX and accessibility (when applicable) | 10 | Navigation, responsive behavior, inclusive interaction |

For non-UI projects, allocate the UX weight to developer experience and API ergonomics; document the adjustment. **Never substitute absence of evidence with a passing grade.** If the repository cannot be inspected, mark it **Not assessed**. A configured workflow is not a verified passing workflow.

## Scope fairness

- Score only functionality the project currently claims to implement.
- Planned, roadmap or experimental features are not scored as broken.
- Unfinished does not mean defective.
- A critical vulnerability in implemented functionality still matters, whatever the stage.
- Don't award full marks for untested claims, promotional copy or unverified deployments.
- A numerical score is a provisional reviewer assessment, not a certification.

## Project evidence card template

```md
### Project name
Stage: To confirm
Verification: Not yet verified
Implemented scope: [working functions supported by code]
Known limitations: [specific facts]
Next milestone: [one concrete deliverable]
Engineering assessment: Not assessed (until source and tests are inspected)
Evidence: [source paths, test results, CI run links, demo links]
```

## Path to 9–10/10

A high rating requires a reproducible setup, clear architecture, meaningful automated tests, working CI, secure defaults, honest third-party attribution and an accessible demo or documented walkthrough where practical. These are **quality and evidence requirements**, not a demand that every product be feature-complete.

## Portfolio governance

Review each repository independently. Record the evaluation date, commit SHA, scope and evidence. Re-evaluate after material changes. Keep verified facts separate from intended future features.
