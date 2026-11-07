# CI Evidence Snapshot — 2026-11-07

**Source:** GitHub Actions REST API; latest available workflow runs checked on 2026-11-07.  
**Scope:** Five selected public repositories. This is a **point-in-time record**, not a live dashboard or certification of production readiness.

| Repository | Workflow | Run | Commit SHA | Conclusion | Failed step if applicable |
| --- | --- | --- | --- | --- | --- |
| [LX Obsidian Portal](https://github.com/lx-obsidian-labs/lx-obsidian-portal) | Verify portal | [42397050121](https://github.com/lx-obsidian-labs/lx-obsidian-portal/actions/runs/42397050121) | `a5f96f28d682d91931970f3be730b28e2e5f58a8` | **Success** | — |
| [Revona CLI](https://github.com/lx-obsidian-labs/revona-cli) | Python package smoke test | [42397053506](https://github.com/lx-obsidian-labs/revona-cli/actions/runs/42397053506) | `217acf1338b2b32a32991bbb0615396dd80a66ce` | **Success** | — |
| [MMS Platform](https://github.com/lx-obsidian-labs/mms-platform) | Verify Next.js application | [42393763372](https://github.com/lx-obsidian-labs/mms-platform/actions/runs/42393763372) | `02add610525562a12aa89100458308d8cc552653` | **Success** | — |
| [Crankified's Beauty Bar](https://github.com/lx-obsidian-labs/crankifieds-beauty-bar) | Verify application | [42397057238](https://github.com/lx-obsidian-labs/crankifieds-beauty-bar/actions/runs/42397057238) | `b6b83db40b060c87c2bf5b6289cbaa7f76514c8e` | **Failure** | TypeScript |
| [Edu Learn](https://github.com/lx-obsidian-labs/e-learning-platform) | Test learning platform | [42396935182](https://github.com/lx-obsidian-labs/e-learning-platform/actions/runs/42396935182) | `467720ab2386a2a0feffb00ed32bcb9deebcbe6f` | **Failure** | Install locked dependencies |

## Immediate remediation queue

### P0 — Crankified's Beauty Bar

1. Inspect the TypeScript step log for run 42397057238 and identify the exact compiler diagnostic.
2. Fix source or configuration rather than bypassing typechecking.
3. Re-run the full verification workflow and link the passing result.
4. Separately test booking concurrency and admin authorization; successful CI does not replace integration testing.

### P0 — Edu Learn

1. Inspect the dependency-installation step log for run 42396935182.
2. Reconcile `package.json`, `package-lock.json` and the workflow's Node/npm versions.
3. Re-run locked installation, tests and build without disabling the lockfile integrity check.
4. Separately audit certificate and blockchain language and verify actual feature behavior.

### Follow-up — Passing workflows

- **Portal:** Verify real lead persistence and notification delivery with controlled production-safe data.
- **Revona:** Verify filesystem and shell boundaries in a disposable workspace.
- **MMS:** Verify Supabase row-level security, role authorization and key training workflows.

## Evidence limitations

A green workflow is evidence only for the jobs and steps configured in that workflow at that commit. A red workflow is a release blocker, not a maturity score. Neither result establishes production availability, customer outcomes, client permissions or complete security.

Update this snapshot when a new run changes any conclusion. Preserve older snapshots as historical evidence rather than rewriting the past.

[Documentation hub](DOCUMENTATION_INDEX.md) · [Evidence register](ENGINEERING_EVIDENCE_REGISTER.md)
