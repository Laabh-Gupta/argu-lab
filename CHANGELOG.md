# ArguLab changelog

**Release: v3.0.2**

Selected releases only. The [project story](PROJECT_HISTORY.md) explains the larger milestones; [versioning](VERSIONING.md) explains tags and future updates.

## [3.0.2] — 2026-09-26

- Replaced the catch-all API dispatcher with explicit route groups and a shared frontend/backend URL contract.
- Preserved account ownership, authentication, streaming, speech limits and the existing Netlify/Render deployment.
- Stopped unknown AI URLs and unsupported methods consuming AI quota; malformed review JSON now returns a client error.
- Added HTTP routing and streaming regression coverage: 58 backend/integration tests and 21 browser tests passed for the routing implementation.
- Added a task-by-task AI guide, synchronized package versions, a release check in CI, four release-tool regression tests and documented release preparation.
- Updated both repositories' current guides and graphics to v3.0.2. Historical release notes retain their original version and date.

[Full v3.0.2 release notes](docs/releases/3.0.2.md)

## [3.0.1] — 2026-09-19

Privacy and policy pages, essential-storage disclosure, adult/terms acknowledgements, account export/deletion and accessibility improvements. Source release: `48c68ef`. The following branding/documentation updates retained this app version.

## [2.0.1] — 2026-09-12

Resumable practice, first-party accounts, actual activity-based progress, local recording, exports and automated verification. Source release: `1e7ebb4`.

## [2.0.0] — retrospective August 2026 milestone

Expanded training modes, Thinking View, scoring profiles, shared navigation and simulated group discussion. The consolidated `fedb5c5` snapshot from 30 August represents this stage; the original history did not contain a v2.0.0 tag.

## [1.0.0] — retrospective August 2026 milestone

The initial MindForge debate experience and real transcript scoring. The `2023593` snapshot from 4 August represents this stage; the original history did not contain a v1.0.0 tag.
