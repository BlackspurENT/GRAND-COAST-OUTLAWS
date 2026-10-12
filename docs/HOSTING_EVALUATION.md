# GCO — Technical Hosting Evaluation Brief

*Partner-facing evaluation outline · 12 October 2026*

## Executive summary

**Grand Coast Outlaws (GCO)** is an independent multiplayer action project built using Unreal Engine 5 and C++. The team is evaluating options for an **eventual** dedicated server prototype. This document is an early technical planning brief, **not a request to deploy an existing production-ready game**.

## Current verified scope

Project development records report a successful Unreal Development Editor build, C++ foundation and **limited two-player PIE listen-server tests**. This does **not** establish a dedicated Linux/Windows server binary, a container image, production multiplayer scalability or a public playable demo.

**Dedicated-server package status: not yet validated.**

## Proposed evaluation stages

| Gate | Deliverable | Evidence required |
| --- | --- | --- |
| A: Build | Small UE dedicated server build for the selected host OS | Executable, logs, reproducible build instructions |
| B: Package | Reproducible server deployment bundle, or a container image where supported | Manifest, launch args, port map, dependencies |
| C: Connectivity | Independent clients join a remote test server | Host/client session logs and observed behavior |
| D: Stability | Repeatable sessions, restart tests, failure handling | Test notes with version, duration and errors |
| E: Benchmark | Measured resource usage and latency for declared test conditions | CPU, memory, bandwidth and connection counts |
| F: Review | Consolidated pilot results and next steps | Written technical summary and limitations |

## Questions for potential infrastructure partners

1. Supported operating system, architecture, runtime and Unreal-specific packaging requirements?
2. Container image support and registry choices (if applicable)?
3. Trial compute quotas, RAM/CPU allocations, storage, geographic regions and networking restrictions?
4. Payment method requirement, automatic charges and trial-expiration behavior?
5. Availability of deployment diagnostics, session logs, and monitoring tools?
6. Allowed workload types and a route for technical support during the pilot?

## Safe scope for a pilot

- Use a small, test-oriented multiplayer level with synthetic test accounts.
- Do not upload private credentials, game source or licensed assets without written authorization and a clear need.
- Begin measurements only after a real build passes local checks.
- Keep the evaluation separate from public claims about production readiness.
- Do not imply a provider is sponsoring the game solely because they discuss testing options.

## Requested next step

When the dedicated-server artifact is ready, align on a short deployment window, define what will be measured, and prepare a concise results report. Until then, the project remains in engineering preparation.

**No hosting agreement, free perpetual server or launch timetable is claimed by this document.**

[Development roadmap](ROADMAP.md) · [Current project status](DEVELOPMENT_STATUS.md)
