# Multichain Data Observatory

> **Local private review:** publication is paused. See [security review and remaining release conditions](docs/SECURITY_REVIEW.md). Local fixes have not been pushed.


An interactive interface for inspecting multichain observations, source context and relationships in a Three.js visualization.

![review](https://img.shields.io/badge/review-private-374151) ![primary](https://img.shields.io/badge/primary-TypeScript-2563EB) [![LinkedIn](https://img.shields.io/badge/LinkedIn-Douglas%20Silva-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/douglas-silva-data-analyst/)

[Overview](#overview) · [Architecture](#architecture) · [Setup](#setup) · [Validation](#validation) · [Roadmap](#roadmap) · [Review notes](docs/REVIEW.md)

## Overview

- Network observations retain identity, timestamps and source references.
- Interactive views expose linked market and social context.
- A local preview server and private-preview build path are provided.

**Technology:** TypeScript · JavaScript · React · Three.js · Vite · Node.js

**Persistence and data:** Observation envelopes and client-side state drive visualization. Database references in individual adapters should not be interpreted as a complete bundled backend deployment.

## Architecture

```text
Observation adapters → normalized evidence envelope → React views → Three.js scene and detail inspection
```

| Location | Review focus |
| --- | --- |
| [`src/main.tsx`](src/main.tsx) | Source/configuration inspected for scope and structure |
| [`server.mjs`](server.mjs) | Source/configuration inspected for scope and structure |
| [`docs/DATA-CONTRACT.md`](docs/DATA-CONTRACT.md) | Source/configuration inspected for scope and structure |
| [`docs/ARCHITECTURE.md`](docs/ARCHITECTURE.md) | Source/configuration inspected for scope and structure |
| [`package.json`](package.json) | Source/configuration inspected for scope and structure |

Internal package and module names are retained where changing them would affect imports or compatibility. This descriptive repository name does not imply a completed package/API migration.

## Setup

Use a current Node.js version compatible with the package lock. Install with npm ci --ignore-scripts; inspect package.json before selecting npm test, npm run typecheck or a preview build.

Start from an isolated environment. Use `.env.example` when present and inspect the configuration loader: an example file is not necessarily loaded automatically. Runtime databases, real account sessions and private credentials are not bundled. Live integration prerequisites are separate from local tests.

## Validation

Static parsing checked 0 Python files and 4 strict JSON files. Python syntax errors: 0; JSON errors: 0. No functional test/build result is claimed for this preparation.

Available test scripts are inventoried in [the review notes](docs/REVIEW.md). Choose offline checks before operating any integration.

These results apply to the selected checks on the preparation copy. They do not establish deployment readiness, full coverage, live provider availability or measured performance. CI definitions, when present under `docs/ci-templates/`, are inactive review templates; no remote CI badge is claimed.

## Limits and current status

Existing confidentiality notices remain applicable. Some binary visual assets and live data access are omitted from this review copy. A visualization does not prove a live ingestion pipeline.

This private snapshot is for code and portfolio review. Generated runtime material and unreviewed binary assets may be excluded. [Review notes](docs/REVIEW.md) record preparation scope, findings and outstanding validation.

## Roadmap

- [ ] Run the declared Node tests, typecheck and private-preview build.
- [ ] Provide a synthetic dataset with documented source contracts.
- [ ] Review asset attribution and confidential integration boundaries before public release.

## History and attribution

21 existing commits were retained after path/content filtering. Original authors and author/committer dates were retained; commit hashes may change. Upstream commits are not presented as new work by the maintainer.

No open-source license is granted by this preparation. A license and attribution review is required before public redistribution.

## Maintainer and feedback

Douglas de Oliveira Silva · [GitHub](https://github.com/qquante) · [LinkedIn](https://www.linkedin.com/in/douglas-silva-data-analyst/)

For this private review, report reproducible issues with a minimal fixture and the exact check output. Keep account data, credentials and generated sensitive reports out of issues and commits. Existing contribution guidelines apply where present.

**Topics:** `typescript`, `react`, `threejs`, `data-visualization`, `blockchain`, `vite`
