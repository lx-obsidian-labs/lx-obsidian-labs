# Portfolio Case Study Template

Use this template for each flagship project. Do not replace evidence gaps with promotional language.

## Project identity

- **Project:**
- **Repository:**
- **Client/product ownership:**
- **Publication permission:** Confirmed / Pending
- **Maintainer and role:**
- **Review date / commit SHA:**
- **Maturity:** Prototype / Development / Beta / Production / Maintenance
- **Verification:** Unverified / Partially verified / Verified for stated scope

## Executive summary

Describe the user problem, intended audience and the scope actually implemented in 3–5 sentences. Distinguish delivered work from planned features.

## Problem and constraints

What operational or customer problem motivated the project? Record business, technical, privacy, budget and platform constraints without revealing confidential information.

## My contribution

Specify work personally implemented or led. For third-party codebases, forks and AI-assisted work, identify upstream foundations, independently attributable changes and validation responsibility.

## Architecture

```text
[User/browser/mobile client]
        |
        v
[Frontend or API boundary]
        |
        v
[Authorization + business logic]
        |
        +----> [Database/storage]
        +----> [External providers]
```

Replace the placeholder diagram with actual components and trust boundaries. Explain data flow, authorization and failure handling.

## Implemented capabilities

| Capability | Evidence in source | Test or demo | Status |
| --- | --- | --- | --- |
| Example | Path / commit | CI link / test | Unverified |

## Engineering decisions and trade-offs

Describe two or three important decisions: alternatives considered, why the implementation was chosen, trade-offs, operational impact and remaining limitations.

## Security and privacy

Record authentication, authorization, validation, secrets, rate limiting, data retention, logging and dependency risks. Include unresolved issues and compensating controls.

## Quality and reproducibility

```text
Runtime:
Install:
Lint:
Typecheck:
Unit/integration tests:
Build:
CI run URL and conclusion:
Live smoke test date and result:
Accessibility evidence:
```

## Results and impact

Use only verified metrics. If adoption, latency, uptime or revenue cannot be independently substantiated, say **not measured**. Avoid invented testimonials or user counts.

## Known limitations

List unresolved security, functional, deployment and usability issues.

## Next milestones

Order by user impact, security and engineering risk.

## Attribution and rights

List dependencies, upstream sources, licenses, client publication approvals and screenshot permissions.

[Documentation quality standard](DOCUMENTATION_QUALITY_STANDARD.md)
