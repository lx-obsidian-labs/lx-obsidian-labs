# Engineering Evidence Register

This register distinguishes **source-confirmed facts**, **declared features**, and **unverified outcomes**. It is intended for technical reviewers and recruiters.

_Last reviewed: 2026-11-06. This is a targeted manifest/documentation review, not a full security audit._

| Repository | Evidence observed | Still to verify |
| --- | --- | --- |
| [Revona CLI](https://github.com/lx-obsidian-labs/revona-cli) | Python package metadata requires Python >=3.11; Click, Rich, Requests and OpenAI SDK are declared; `revona` CLI entry point is configured. | Clean installation, command behavior, automated tests, original/upstream attribution and published releases. |
| [Edu Learn](https://github.com/lx-obsidian-labs/e-learning-platform) | Next.js, Supabase and Vitest dependencies; `test` and `test:coverage` scripts declared. | Test execution, coverage results, deployment, accessibility and advertised feature behavior. |
| [LX Obsidian Portal](https://github.com/lx-obsidian-labs/lx-obsidian-portal) | Wrangler-based Cloudflare workflow; `build` and `check` scripts; GitHub Actions verification workflow added. | Actual CI run results, live deployment, security review and end-to-end forms. |
| [MMS Platform](https://github.com/lx-obsidian-labs/mms-platform) | Next.js and Supabase dependencies; `build` and `lint` scripts declared. | Passing builds, tests, architecture and product use cases. |
| [SA Innovation College](https://github.com/lx-obsidian-labs/sa-innovation-college) | Next.js, React, PDF-generation and Nodemailer dependencies. | Passing builds, client publication permission, accessibility and live deployment. |

## Evidence policy

- A declared dependency is **not** proof that a feature works.
- A configured CI workflow is **not** a passing CI result.
- A public repository is **not** proof of sole authorship.
- Do not publish customer information, credentials or private implementation details.
- Link test logs, releases, architecture diagrams and reproducible setup instructions once verified.

## Next audit gates

1. Review repository trees and commit histories for attribution and licensing.
2. Inspect configuration, source, tests and secret-handling practices.
3. Run builds and tests; record exact commands and results.
4. Add screenshots and concise, evidence-backed case studies.
5. Select six repositories for the GitHub profile based on verified quality.

Maintainer: LX Obsidian Labs — Nathan Vilane.
