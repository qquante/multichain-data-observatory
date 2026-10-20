# Multichain Data Observatory

An interactive interface for inspecting multichain observations, source context and relationships in a Three.js visualization.

## Features

- Network observations retain identity, timestamps and source references.
- Interactive views expose linked market and social context.
- A local preview server and private-preview build path are provided.

## Stack

TypeScript · JavaScript · React · Three.js · Vite · Node.js

Observation envelopes and client-side state drive visualization. Database references in individual adapters should not be interpreted as a complete bundled backend deployment.

## Getting started

Use a current Node.js version compatible with the package lock. Install with npm ci --ignore-scripts; inspect package.json before selecting npm test, npm run typecheck or a preview build.

## How it works

```text
Observation adapters → normalized evidence envelope → React views → Three.js scene and detail inspection
```

## Current limitations

Existing confidentiality notices remain applicable. Some binary visual assets and live data access are omitted from this review copy. A visualization does not prove a live ingestion pipeline.

## License

Project-authored source code is licensed under the [MIT License](LICENSE). Third-party components and datasets retain their respective rights and licenses.
