# LX Obsidian Labs — GitHub Portfolio Audit and Remediation Plan

**Audit date:** 2026-11-07  
**Scope:** Connected `lx-obsidian-labs` account; 30 accessible repositories (20 public, 10 private); selected README files, repository metadata, engineering evidence and one verified merged pull request.  
**Method:** Remote repository metadata and documentation inspection. **No claim of complete source audit, successful CI, live deployment testing, secret scanning, license verification or penetration testing.** Private repository names are included for owner inventory; their internal content is not disclosed.

## Executive assessment

The account demonstrates a broad range of web, mobile-adjacent, education, AI tooling, commerce and client work. The main weakness is **portfolio coherence and verifiability**, not the number of projects. Similar repository names, missing descriptions, unclear canonical deployments, inconsistent documentation and incomplete CI evidence make it harder for a recruiter or client to identify the strongest implementation.

The profile README has been rebuilt to foreground seven relevant projects and distinguish claims from evidence. The Revona CLI README was corrected after verifying that PR #1 was merged on 2026-11-06. Further remediation requires inspecting source, running builds/tests and obtaining approval before changing public client-facing claims or archiving repositories.

## Repository inventory

Metadata was observed from the connected GitHub account on the audit date. A listed homepage is **configured metadata**, not a confirmed functioning deployment.

| Repository | Visibility | Positioning / observed metadata | Recommended action |
| --- | --- | --- | --- |
| lx-obsidian-labs | Public | Profile and portfolio documentation | Maintain canonical navigation and evidence register |
| lx-obsidian-portal | Public | Company website and product portfolio | Establish as canonical public website repository; verify Cloudflare lead delivery |
| lx-obsidian-labs-website | Public | Separate Next.js company website | Explain relationship to canonical portal; do not archive without owner approval |
| lxobsidianportal | Public | Mining education website, similarly named | Clarify identity to avoid brand confusion |
| brand-assets | Public | Canonical brand guidance; PNG inventory not yet populated | Add approved assets only when source binaries are available |
| revona-cli | Public | Python agent/developer automation | Verify merged hardening and default-branch CI; document upstream attribution |
| lx-obsidian-cli | Public | T3 Code-based agent tooling (MIT) | Keep explicit upstream attribution, license and differences |
| lx-obsidian | Public | Design/tooling repository; sparse metadata | Add concise description, actual feature inventory and tests |
| nexus-ai | Public | AI platform | Document supported capabilities and verification |
| hookd | Public | TypeScript AI tooling prototype | Clarify prototype scope and setup |
| e-learning-platform | Public | Learning platform | Capture reproducible tests, screenshots and permissions |
| mms-platform | Public | Mining training ecosystem | Add architecture, deployment verification and case study |
| sa-innovation-college | Public | Client-oriented education website | Verify client publication permissions, links and accessibility |
| newtons-4th-training-academy | Public | Training website | Verify client approval and production status |
| ec-tech-hub | Public | Tech community hub | Document feature scope and maintenance status |
| all-things-store | Public | Commerce application | Verify payment/data flows and add architecture notes |
| synapse-social | Public | Social platform prototype | Document realtime/privacy boundaries and limitations |
| incognito-party | Public | Anonymous social PWA; description calls it a 'private MVP' | Clarify that **repository is public**; review sensitive content |
| crankifieds-beauty-bar | Public | Booking/admin application | Run authentication and booking integration tests; check publication rights |
| gods-clay-media | Public | Campaign artwork | Document asset rights and usage |
| lxportal-crm | Private | CRM project | Owner-only: identify canonical version |
| lxportal-crm-2 | Private | Second CRM project | Owner-only: compare with CRM original before consolidation |
| lx-mis | Private | MIS project | Owner-only: document deployment and security |
| vista-operations-consoles | Private | Vista operations console | Owner-only: protect administrative endpoints and secrets |
| MadeInAfrica.com | Private | Digital trade infrastructure | Owner-only: review architecture and launch claims |
| PrepPro | Private | Application project | Owner-only: add README and ownership notes |
| Vyralynx | Private | Empty repository at audit | Owner-only: decide whether to retain |
| lx-shopify-admin-mcp | Private | Shopify admin integration | Owner-only: review credential scopes and access boundaries |
| texttopdf-ai | Private | PDF/document generation | Owner-only: review data retention and generated files |
| the-bishop | Private | Application project | Owner-only: add purpose and risk classification |

## Findings and risk register

| ID | Severity | Finding | Evidence and recommended response |
| --- | --- | --- | --- |
| P-01 | High | Unclear canonical company website | `lx-obsidian-portal`, `lx-obsidian-labs-website`, and `lxobsidianportal` coexist. Add relationship notes and a single canonical landing path. |
| P-02 | High | Insufficient evidence for quality claims | Evidence registers explicitly say CI/deployment not verified. Record exact workflow URL, run ID, commit and outcome per flagship project. |
| P-03 | High | Public client-oriented repositories | Public status observed for beauty bar and training/college websites. Confirm contractual permissions and remove real customer information if any is found. Public does not imply a leak; content inspection is still required. |
| P-04 | High | Portfolio discoverability | Several repositories have no description, homepage or topics. Improve metadata after verifying each project's purpose. |
| P-05 | High | Agent-tooling provenance | `lx-obsidian-cli` identifies T3 Code foundation; inspect and preserve upstream licenses and attribution. Revona's authorship/dependency documentation also needs verification. |
| P-06 | Medium | Brand assets incomplete | Brand README says 13 planned PNG exports are not committed. Do not provide dead asset download links or claim files are present. |
| P-07 | Medium | Duplicate/parallel CRM projects | Two private CRM repos have similar names and sizes. Compare history and purpose before any archive, rename or merge. |
| P-08 | Medium | Ambiguous 'private MVP' wording | `incognito-party` is a public repo despite that phrase in its description; clarify whether it describes product availability, not source visibility. |
| P-09 | Medium | Missing documentation on several projects | Add honest README, setup, architecture, test commands, screenshots, license and deployment notes where applicable. |
| P-10 | Medium | Unverified security and production posture | Perform dependency/secret scanning, authorization review, privacy assessment and live smoke tests for flagship applications. |

## Remediation sequence

### Phase 1 — Discoverability and truthfulness
- [x] Rebuild profile README with curated projects, audiences and evidence navigation.
- [x] Correct Revona merged PR claim.
- [x] Produce a dated 30-repository inventory and risk register.
- [ ] Clarify canonical website repository and document relationships between similarly named repos.
- [ ] Review metadata for all public repositories; update only after validating purpose and homepage.
- [ ] Verify whether publicly visible client artifacts may be shared.

### Phase 2 — Flagship engineering evidence
For `lx-obsidian-portal`, `revona-cli`, `lx-obsidian-cli`, `e-learning-platform`, `crankifieds-beauty-bar`, `mms-platform` and `sa-innovation-college`:
- [ ] Record default branch SHA, language/runtime, build and test commands.
- [ ] Execute CI or reproduce locally; save exact passing/failing results.
- [ ] Check security controls and sensitive-data handling.
- [ ] Add one-page architecture diagrams and honest case studies.
- [ ] Provide mobile/desktop screenshots or walkthroughs where permissions allow.
- [ ] Confirm license and third-party attribution.

### Phase 3 — Operational quality
- [ ] Enable dependency update and vulnerability reporting workflows as appropriate.
- [ ] Add `SECURITY.md`, `CONTRIBUTING.md`, issue templates and release notes to actively maintained open projects.
- [ ] Verify branch protection/rulesets and required CI checks.
- [ ] Audit deployed URLs, broken links, forms, accessibility and Core Web Vitals.
- [ ] Document rollback, backups and environment-variable requirements.
- [ ] Revisit archived/legacy candidates **only with owner approval**.

## Evidence collection format

For every flagship review record:

```md
Repository:
Reviewed commit SHA:
Review date:
Implemented scope:
Stage: To confirm / Prototype / Active Development / Beta / Production / Maintenance
Verification: Not yet verified / Partially verified / Verified for stated scope
Commands and results:
CI run URL and conclusion:
Deployment smoke test URL and outcome:
Security findings:
Third-party attribution and license:
Known limitations:
Next milestone:
```

**No numerical quality rating is assigned without sufficient implementation and test evidence.** The inventory and metadata audit are complete for the connected account; deep technical certification is not.
