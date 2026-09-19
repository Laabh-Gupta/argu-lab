# ArguLab — project history

From the first MindForge prototype to **Argulab v3.0.1**. This is a curated account of changes that materially altered the app, reconstructed from commit messages, file changes and implementation records through **19 September 2026**. Routine generated changes, merges and small fixes are omitted.

The source history explicitly names **v2.0.1** and tags **v3.0.1**. It does **not** contain a v2.0.0 tag or commit title. The v2.0.0 heading below is a retrospective label for the expanded pre-v2.0.1 application, not a claim that a formal release tag existed. Commit identifiers are reference points in the private source repository; the public documentation repository does not include that repository's code or Git history.

## At a glance

| Stage                                | Period            | Significant change                                                                                           |
| ------------------------------------ | ----------------- | ------------------------------------------------------------------------------------------------------------ |
| Initial MindForge prototype          | 1–4 August 2026   | App shell, dashboard and debate flow, followed by real transcript scoring.                                   |
| v2.0.0 — expanded practice platform  | 5–30 August 2026  | Training hub, multiple modes, structured reviews, shared navigation and moderated group discussion.          |
| v2.0.1 — complete practice workflows | 12 September 2026 | Resumable history, first-party accounts, real progress, local recording, exports and automated verification. |
| Deployment and Argulab transition    | 12 September 2026 | Separate frontend/API deployment, hosted PostgreSQL, verified database TLS and the Argulab name.             |
| Modular workspaces and speech        | 19 September 2026 | Clear ownership of frontend/backend/shared code, opt-in transcription, read-aloud and fictional demo data.   |
| v3.0.1 — privacy and accessibility   | 19 September 2026 | Policies, adult/terms acknowledgements, account export/deletion and accessibility improvements.              |
| Logo refresh                         | 19 September 2026 | New brain-and-speech-bubble logo supplied for the current app.                                               |

## 1. Initial stages — MindForge takes shape

The project began from a TanStack-based template on 1 August. By 4 August, the first MindForge implementation brought together landing, account, dashboard, debate and result screens. Early interface data and placeholder behavior established the product's shape.

The important next step was connecting the debate experience to an AI conversation flow and scoring actual transcripts, giving the result screen something grounded in the user's session.

Selected evidence:

- `b90d714` — **Implemented MindForge app**, 4 August: the first integrated interface and debate-oriented product structure.
- `2023593` — **Added real transcript scoring**, 4 August: server-side conversation/scoring integration and transcript-based results.

## 2. v2.0.0 — from debate app to practice platform

The pre-v2.0.1 application expanded beyond one debate screen. A training hub and reusable session interface supported different conversation formats; Observer Mode added discussion analysis. Thinking View and configurable scoring profiles made the review experience more structured.

A shared application shell consolidated navigation and added dedicated module and progress screens. Group discussion developed into a moderated simulation with distinct AI participants. The late-August implementation checkpoint brought that accumulated work into the main development history.

This stage established the breadth of the product, while later work was still needed for reliable account persistence, honest progress calculations, end-to-end recovery and production deployment.

Selected evidence:

- `c47a346` — **Added AI training modes & hub**, 5 August: reusable sessions, training routes, Observer Mode and shared evaluation.
- `442331c` — **Added thinking-view & scoring**, 6 August: argument-analysis UI and preset/custom evaluation profiles.
- `5f84b82` — **Refactored app into shared shell**, 8 August: consistent navigation, module pages and progress/settings screens.
- `8ad9507` — **Added AI moderator & cast**, 11 August: more developed participant and moderator behavior in group discussion.
- `fedb5c5` — **Update MindForge implementation**, 30 August: consolidated implementation checkpoint before the next major completion pass.

## 3. v2.0.1 — dependable end-to-end practice

The explicitly named v2.0.1 commit on 12 September completed and hardened the practice workflows. Nine modes gained contextual sessions, resumable history and richer reviews. Progress, achievements and leaderboard totals were derived from actual saved activity, with account ownership and completion checks.

Better Auth replaced the earlier Supabase-dependent account integration. At this point the portable server used SQLite; hosted PostgreSQL arrived in the next deployment stage. Guest practice remained available, with separate browser/account histories. Google sign-in integration and recovery configuration were prepared without claiming external provider setup was finished.

This release also added local recording with playback/download, report and JSON exports, request limits, safe provider errors, test coverage, CI and portable deployment instructions. Recording was local at this stage; transcription and read-aloud came later. The visual style moved toward a restrained charcoal-and-green workspace with self-hosted fonts and improved sidebar behavior.

Selected evidence: `1e7ebb4` — **MindForge v 2.0.1**, 12 September. Its implementation record documents the completed workflows and the limitations that still remained.

## 4. Separate deployment and the Argulab name

The application was then adapted for a static frontend on Netlify and a separate Fastify API on Render. PostgreSQL hosted by Supabase replaced production SQLite while Better Auth continued to manage accounts on the backend.

The split added a same-origin account proxy, a direct API path for AI streaming, database persistence/import checks and compatible frontend dependencies. Verified TLS secured the hosted database connection. The public-facing name became Argulab, with documentation for the actual deployment; compatibility identifiers were retained to preserve existing accounts and history.

Selected evidence:

- `238e48d` — **Split deployment on main and fix Vite dependency compatibility**, 12 September.
- `0c936c8` — **Configure verified Supabase TLS in backend deployment**, 12 September.
- `9b4cfc8` — **Rename app to Argulab and document setup and deployment**, 12 September.

## 5. Clearer workspaces, optional speech and demonstration data

On 19 September, frontend, backend and shared contracts became explicit workspaces with separate manifests and TypeScript configurations. Features and backend modules were grouped by responsibility, duplicated helpers were consolidated, and stale files were removed from the active source layout.

Audio gained optional Groq transcription into an editable draft and browser read-aloud, with separate speech quotas. Uploading requires an explicit transcription action. An idempotent demonstration seed added 18 fictional sessions across all nine modes, with credentials kept out of published files.

Selected evidence: `c99d4a4` — **Separate application workspaces and add speech practice and demo data**, 19 September. This was the major engineering step immediately before v3.0.1; the source history does not tag it as a separate v3.0.0 release.

## 6. Current release — Argulab v3.0.1

The v3.0.1 release added public privacy, terms, refund, cookie, accessibility and license pages, together with an essential-storage notice. Registration and AI practice require adult/terms acknowledgements. Users can export account data and permanently delete an account with authenticated ownership checks and session revocation.

The release reduced unnecessary authentication metadata, clarified optional audio transfers, included font/icon licenses, removed unsupported promotional claims, and improved contrast, focus behavior and small-screen dialogs. No payment, marketing, analytics or parental-consent service was introduced. Public operator/contact details were deferred by the collaborators.

The release validation recorded 47 unit/integration tests and 21 browser tests, plus persistence, import, build, type, accessibility and credential checks. Netlify and Render deployments and existing demo history were checked. These are engineering results, not guarantees of legal compliance, complete accessibility or uninterrupted availability.

Selected evidence: `48c68ef` — **Argulab v3.0.1**, 19 September; annotated source tag **`v3.0.1`**.

## 7. Current branding — logo refresh

The following **logo change** commit (`1bfc8fe`, 19 September) supplied the new brain-and-speech-bubble artwork and updated the site's favicon asset. The public documentation uses that supplied image. The app version remains 3.0.1; this branding commit did not create another version tag.

## What remains separate from completed features

Google sign-in and password-recovery email still require their live provider setup. AI review assesses submitted text, not vocal delivery. Human multiplayer, paid subscriptions and independently verified outcome claims are not part of the current release.

The project now publishes product documentation separately from its private source. This history is intentionally present in both repositories so the same milestones can be read without exposing implementation files, credentials or source history.
