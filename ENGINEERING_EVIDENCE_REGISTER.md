# Engineering evidence register

This is an evidence index, not a claim that CI is passing. Development stage and engineering quality are assessed separately under [the portfolio rubric](PORTFOLIO_EVALUATION.md).

| Project | Inspectable engineering artifacts | Next verification |
| --- | --- | --- |
| [Revona CLI](https://github.com/lx-obsidian-labs/revona-cli) | [Python CI](https://github.com/lx-obsidian-labs/revona-cli/blob/main/.github/workflows/python-package.yml), [tests](https://github.com/lx-obsidian-labs/revona-cli/tree/main/tests), [security model](https://github.com/lx-obsidian-labs/revona-cli/blob/main/docs/SECURITY_MODEL.md) | Confirm CI conclusion; strengthen shell working-directory and symlink boundaries |
| [LX Obsidian Portal](https://github.com/lx-obsidian-labs/lx-obsidian-portal) | [CI](https://github.com/lx-obsidian-labs/lx-obsidian-portal/blob/master/.github/workflows/verify.yml), [contact tests](https://github.com/lx-obsidian-labs/lx-obsidian-portal/blob/master/tests/contact-api.test.cjs) | Confirm CI conclusion and real lead delivery |
| [Crankified's Beauty Bar](https://github.com/lx-obsidian-labs/crankifieds-beauty-bar) | [CI](https://github.com/lx-obsidian-labs/crankifieds-beauty-bar/blob/master/.github/workflows/verify.yml), [case study](https://github.com/lx-obsidian-labs/crankifieds-beauty-bar/blob/master/docs/ENGINEERING_CASE_STUDY.md) | Booking concurrency and admin authorization tests |
| [MMS Platform](https://github.com/lx-obsidian-labs/mms-platform) | [CI](https://github.com/lx-obsidian-labs/mms-platform/blob/master/.github/workflows/verify.yml) | Confirm stage and run results |
| [Edu Learn](https://github.com/lx-obsidian-labs/e-learning-platform) | [CI](https://github.com/lx-obsidian-labs/e-learning-platform/blob/master/.github/workflows/test.yml) | Confirm stage and run results |

## Evidence policy

1. Record the commit SHA and date of each review.
2. Score implemented, claimed behavior; do not penalize unfinished roadmap features.
3. Distinguish a configured workflow from a successful run.
4. Mark missing results **Not verified**, never automatically **Failed**.
5. Cite tests, reproducible commands, security boundaries and release artifacts before assigning a high score.

**Status:** This register lists inspectable code artifacts. CI success, deployment status and complete end-to-end functionality have not been independently verified in this register.
