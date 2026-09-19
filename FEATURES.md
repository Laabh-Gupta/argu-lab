# ArguLab features

Current app version: **3.0.1**. This guide describes implemented product behavior; provider-dependent features are identified separately.

## Nine ways to practice

| Mode                  | Practice experience                                                                                                      |
| --------------------- | ------------------------------------------------------------------------------------------------------------------------ |
| Debate Arena          | Present an argument, respond to Socratic challenges, clarify a position and review the discussion.                       |
| Group Discussion      | Join a simulated room with an AI moderator and distinct participants; contribute, listen, and review your participation. |
| Interview Simulator   | Choose an interview format, describe your background or target role, and answer contextual follow-up questions.          |
| Public Speaking       | Work on a topic or speech and receive feedback on its submitted content and structure.                                   |
| Extempore             | Practice with a generated topic, preparation time and a timed response.                                                  |
| Negotiation           | Respond to a counterpart in a scenario and review concessions, priorities and trade-offs.                                |
| Case Discussion       | Frame a problem, reason through evidence and propose a recommendation.                                                   |
| Real-World Simulation | Take a role in a scenario with simulated stakeholders and events.                                                        |
| Observer Mode         | Read a generated discussion, answer analysis questions and review your interpretation.                                   |

These are simulations with AI participants, not live rooms with other human users.

## Conversations and reviews

- Configurable topics, difficulty, and mode-specific roles or formats.
- English, Hindi and mixed-language response preferences.
- Streamed replies, saved transcripts and resumable unfinished sessions.
- Mode-specific reviews with strengths, weaknesses, reasoning issues and suggested next steps.
- Fifteen underlying review dimensions, preset scoring profiles and custom weights; re-scoring a review does not award a second completion.
- Thinking View for structured argument analysis where supported. It is an explanatory output, not access to a model's hidden internal reasoning.

AI output may be inaccurate. Suggested evidence is not independently fact-checked, and scores do not certify ability or predict admission, examination or employment outcomes.

## History and progress

- Guest practice stays in the current browser; account practice can be retrieved after signing in on another device.
- Dashboard activity and progress come from saved practice records.
- Calendar streaks, levels, achievements, skill trends and history filters help organize repeated practice.
- The optional leaderboard publishes a display name and aggregate totals, not private transcripts or email addresses.
- A separate demonstration dataset contains 18 clearly fictional sessions across all nine modes. These are examples, not customer reviews. Demo credentials are not published here.

## Audio, with explicit controls

Record, pause, resume, play back or download a short recording. Recording alone does not upload the audio. Choose **Transcribe** to send it for speech-to-text conversion, review the editable draft, then send the text yourself.

**Listen** uses the browser or operating system's speech service. Some voices may process text remotely. Recording and voice support depend on the browser and device, and written input remains available.

Recordings are limited to two minutes and transcription uploads to 4 MB. Transcription has separate application limits of 10 requests per visitor/hour, 20 per visitor/day, 100 globally/day and 5 globally/minute. Provider quotas also apply. Current conversation defaults are 60 requests per visitor/hour and 600 across the app/hour.

The configured defaults are Groq `openai/gpt-oss-120b` for conversation/review and `whisper-large-v3-turbo` for transcription. Browser read-aloud does not use a paid text-to-speech API. Provider availability and deployment settings can change.

## Exports and account controls

Download text reports, print or save a report as PDF, export practice/account data as JSON, and download local recordings. Clear history or permanently delete an account from **Settings → Your data**.

Account deletion requires the current password for email accounts, or a recent sign-in for Google-only accounts when that provider is enabled. It removes active account and practice records and revokes sessions. Exports, copies on other devices, and provider backup/log retention are separate.

## Preferences and accessibility

Light, dark and system themes; larger text; reduced motion; keyboard navigation; visible focus controls; labelled inputs; and responsive dialogs. The v3.0.1 release includes automated accessibility checks in both themes and small-screen checks for consent and deletion. These checks are not a claim of complete WCAG conformance.

## Limits of the current release

- Adults only, with age self-declaration rather than identity verification; no children's accounts or parental-consent flow.
- Google OAuth and recovery email need their live provider setup completed.
- No payments, subscriptions, advertisements, marketing email list or analytics-tracking SDK.
- No automatic migration of guest history into a signed-in account.
- No real-time human multiplayer, identity-verified competition, vocal-delivery grading or guaranteed AI accuracy.

[Back to overview](README.md) · [Project history](PROJECT_HISTORY.md)
