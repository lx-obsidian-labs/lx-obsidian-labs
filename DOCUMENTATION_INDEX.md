# Documentation index — LX Obsidian Labs

**Updated:** 2026-11-07

This index provides a single entry point for company engineering documentation. It records documentation availability, **not certification that the software works in production**.

## Portfolio-level documentation

| Document | Purpose |
| --- | --- |
| [Profile](README.md) | Curated introduction, project navigation and contact |
| [Repository audit](REPOSITORY_AUDIT_2026.md) | Thirty-repository inventory, risks and phased remediation |
| [Evaluation standard](PORTFOLIO_EVALUATION.md) | Evidence-based engineering scoring and maturity definitions |
| [Evidence register](ENGINEERING_EVIDENCE_REGISTER.md) | Project tests, workflows and outstanding checks |
| [Additional engineering evidence](ENGINEERING_EVIDENCE.md) | Source/manifest findings and limitations |
| [Project review template](PROJECT_REVIEW_TEMPLATE.md) | Repeatable technical assessment |
| [Contributing](CONTRIBUTING.md) | Documentation changes, attribution and collaboration |
| [Security policy](SECURITY.md) | Private vulnerability reporting |

## Flagship project entry points

| Project | Documentation | Remaining verification |
| --- | --- | --- |
| [LX Obsidian Portal](https://github.com/lx-obsidian-labs/lx-obsidian-portal) | [README](https://github.com/lx-obsidian-labs/lx-obsidian-portal/blob/master/README.md) | CI, live lead persistence and notification delivery |
| [Revona CLI](https://github.com/lx-obsidian-labs/revona-cli) | [README](https://github.com/lx-obsidian-labs/revona-cli/blob/main/README.md), [security model](https://github.com/lx-obsidian-labs/revona-cli/blob/main/docs/SECURITY_MODEL.md) | Default-branch CI, command and filesystem security |
| [LX Obsidian CLI](https://github.com/lx-obsidian-labs/lx-obsidian-cli) | [README](https://github.com/lx-obsidian-labs/lx-obsidian-cli/blob/main/README.md) | Upstream comparison and attributable contributions |
| [Edu Learn](https://github.com/lx-obsidian-labs/e-learning-platform) | [README](https://github.com/lx-obsidian-labs/e-learning-platform/blob/master/README.md) | Feature claim audit, tests, live deployment |
| [Crankified's Beauty Bar](https://github.com/lx-obsidian-labs/crankifieds-beauty-bar) | [README](https://github.com/lx-obsidian-labs/crankifieds-beauty-bar/blob/master/README.md), [case study](https://github.com/lx-obsidian-labs/crankifieds-beauty-bar/blob/master/docs/ENGINEERING_CASE_STUDY.md) | Session runtime tests, database concurrency and live authentication |
| [MMS Platform](https://github.com/lx-obsidian-labs/mms-platform) | [README](https://github.com/lx-obsidian-labs/mms-platform/blob/master/README.md) | Build, Supabase authorization and workflow verification |
| [SA Innovation College](https://github.com/lx-obsidian-labs/sa-innovation-college) | [README](https://github.com/lx-obsidian-labs/sa-innovation-college/blob/master/README.md) | Build, email/PDF functionality, client approval and accessibility |
| [LX Obsidian](https://github.com/lx-obsidian-labs/lx-obsidian) | [README](https://github.com/lx-obsidian-labs/lx-obsidian/blob/main/README.md) | Cross-framework detector and installation tests |
| [Brand assets](https://github.com/lx-obsidian-labs/brand-assets) | [README](https://github.com/lx-obsidian-labs/brand-assets/blob/main/README.md) | Upload approved raster exports; confirm asset inventory |

## Additional public projects documented

| Project | Documentation | Verification focus |
| --- | --- | --- |
| [Nexus AI](https://github.com/lx-obsidian-labs/nexus-ai) | [README](https://github.com/lx-obsidian-labs/nexus-ai/blob/main/README.md) | Supabase permissions, implemented AI scope, build and lint |
| [EC Tech Hub](https://github.com/lx-obsidian-labs/ec-tech-hub) | [README](https://github.com/lx-obsidian-labs/ec-tech-hub/blob/master/README.md) | Community workflows, Supabase permissions, build and lint |
| [Synapse Social](https://github.com/lx-obsidian-labs/synapse-social) | [README](https://github.com/lx-obsidian-labs/synapse-social/blob/main/README.md) | Browser extension permissions, platform compliance, monorepo tests |
| [Hookd](https://github.com/lx-obsidian-labs/hookd) | [README](https://github.com/lx-obsidian-labs/hookd/blob/master/README.md) | Nested web application tests and agent skill boundaries |
| [All Things Store](https://github.com/lx-obsidian-labs/all-things-store) | [README](https://github.com/lx-obsidian-labs/all-things-store/blob/main/README.md) | Checkout, supplier integration and webhook authorization |

## Publication and verification rules

1. Do not equate repository visibility with permission to publish client material.
2. Do not claim a configured CI workflow passed without a corresponding run result.
3. Do not claim a deployed URL is healthy without a live smoke test.
4. Do not claim sole authorship of third-party or upstream code.
5. Keep release blockers and missing evidence explicit.
6. Review and date documentation when significant implementation changes occur.

**Current boundary:** The portfolio index, audit and several project READMEs have been updated. Complete documentation sign-off still depends on reviewing remaining repositories, confirming client permissions and collecting build, test and deployment evidence.
