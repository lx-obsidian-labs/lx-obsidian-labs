# Documentation quality standard

**Owner:** LX Obsidian Labs · **Updated:** 2026-11-07

This standard defines what **9/10 documentation quality** means for the portfolio. It is a target and review framework, **not a claim that every repository currently meets it**.

## Weighted documentation rubric

| Dimension | Points | Required evidence |
| --- | ---: | --- |
| Purpose and audience | 10 | Clear problem, users, project identity and ownership |
| Scope and maturity honesty | 15 | Implemented vs planned, status and known limitations |
| Reproducible setup | 15 | Runtime, package manager, exact commands, configuration names |
| Architecture and data flow | 15 | Components, integrations, trust boundaries and design decisions |
| Verification and testing | 15 | Commands, test coverage, dated CI run evidence and results |
| Security and privacy | 10 | Credential handling, authorization, data retention and disclosure path |
| Deployment and operations | 10 | Hosting, environment requirements, rollback, observability |
| License and provenance | 5 | Licensing, third-party attribution, client/publication permissions |
| Navigation and maintenance | 5 | Working links, index, owners, review date and update process |
| **Total** | **100** | |

**Scoring:** 90–100 = documentation target achieved; 80–89 = strong but incomplete; 70–79 = adequate; below 70 = significant gaps. Do not award points for placeholder text or unexecuted commands presented as successful.

## Minimum README contract

Every maintained public application repository should provide:

1. One-paragraph purpose, intended audience and project ownership.
2. Explicit maturity and verification labels, dated when practical.
3. Implemented feature inventory separated from roadmap.
4. Source-backed technology stack and repository layout.
5. Clean setup, prerequisites, environment variable **names** and local commands.
6. Build/lint/test commands with evidence or a clear statement that results are unverified.
7. Architecture and external integration notes.
8. Security/privacy limitations and safe vulnerability reporting.
9. Deployment and release/rollback notes, or a clear pending status.
10. License, attribution and permission to publish client material.
11. Known limitations and next milestone.
12. Links back to the portfolio and evidence register.

Asset-only repositories use a tailored contract: asset inventory, provenance, dimensions, license, approval and intended use replace app runtime instructions.

## Quality gates before marking a repository complete

- [ ] Every command was checked against its manifest or source.
- [ ] Every important relative link resolves.
- [ ] No default framework boilerplate remains in the main README.
- [ ] No invented performance numbers, user counts or passing CI assertions.
- [ ] No credentials, personal records or unapproved client materials.
- [ ] No unsubstantiated sole-authorship claims for upstream derivatives.
- [ ] Evidence includes reviewed commit SHA, date and result.
- [ ] One maintainer can reproduce the documented setup in a clean environment.
- [ ] Screenshots are current and rights-cleared, where applicable.
- [ ] Documentation reflects the current deployment, not a planned release.

## Review workflow

1. **Inventory:** inspect root files, manifests, docs and workflow definitions.
2. **Validate:** check implementation and links; mark uncertain claims explicitly.
3. **Improve:** write concise, accurate README and focused supporting docs.
4. **Verify:** execute setup and CI, test production behavior where permitted.
5. **Score:** assign rubric points with evidence and unresolved gaps.
6. **Maintain:** update docs on material feature, security or deployment changes.

## Current assessment boundary

The portfolio has received an extensive **documentation structure and discoverability pass**. Several repositories now have source-backed setup instructions and explicit verification boundaries. A portfolio-wide 9/10 rating is **not yet justified** without reproducible setup, architecture review, live evidence and complete ownership/license checks across selected flagship repositories.

[Documentation index](DOCUMENTATION_INDEX.md) · [Portfolio audit](REPOSITORY_AUDIT_2026.md) · [Evidence register](ENGINEERING_EVIDENCE_REGISTER.md)
