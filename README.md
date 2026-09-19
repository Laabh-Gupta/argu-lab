<p align="center">
  <img src="assets/argulab-logo.png" alt="ArguLab logo: a brain joined with a speech bubble" width="160" />
</p>

# ArguLab

**Practice the conversation before it matters.**

ArguLab is a cooperative project for AI-assisted communication practice. Explore a topic, respond to a challenge, and review your reasoning through debate, interviews, group discussions and other simulated conversations.

**Current app version: 3.0.1** · Formerly MindForge

[Open ArguLab](https://argulab.netlify.app) · [Explore the features](FEATURES.md) · [Project history](PROJECT_HISTORY.md)

## What you can do

- Choose from **nine practice modes**, including debate, interviews and public speaking.
- Set a topic or scenario, difficulty, and supported role or format. Practice in English, Hindi or a mix of both.
- Read AI-generated feedback on claims, evidence, counterarguments and communication.
- Resume unfinished sessions and revisit transcripts, reviews and custom scoring profiles.
- Track completed practice, activity, streaks and achievements. Leaderboard participation is optional.
- Record an answer, choose whether to transcribe it, edit the transcript, and send it yourself. Listen to replies with browser read-aloud.
- Export reports and account data, clear history, or delete your account through Settings.

## Try a session

1. [Open the app](https://argulab.netlify.app) and continue as a guest or sign in with email and password.
2. Choose a practice mode and topic. AI practice is for adults aged 18 or older and asks you to acknowledge the terms.
3. Work through the conversation at your own pace, then request a review.
4. Revisit your session or export the results you want to keep.

Guest history belongs to that browser. Signed-in history is stored with your account; guest history is not automatically merged into it.

## Current availability

The app is free, with no paid subscription, checkout or automatic charges. AI usage limits apply. Free hosting can sleep or pause, so the first request may need time to connect.

Email/password sign-in is available. Google sign-in is implemented but its live provider setup is pending. Password recovery also requires a configured email sender. These integrations are not presented as already enabled.

AI reviews are coaching estimates, not verified facts or guarantees of improvement. Speech feedback assesses submitted text; it does not measure pronunciation or vocal delivery. Real-time human multiplayer and paid plans are not current features.

## Technology overview

| Part                            | Technology                                                |
| ------------------------------- | --------------------------------------------------------- |
| Interface                       | React, TypeScript, Vite, TanStack Router and Tailwind CSS |
| API and accounts                | Fastify and Better Auth                                   |
| Persistent storage              | PostgreSQL hosted by Supabase                             |
| Conversations and transcription | Groq                                                      |
| Hosting                         | Netlify frontend and Render backend                       |

## Privacy and accessibility

The app provides essential-storage disclosures, explicit form acknowledgements, account export/deletion, light and dark themes, larger text, reduced motion and keyboard navigation. Fonts are hosted with the app. There are no advertising or marketing analytics SDKs in this release.

[Privacy and accessibility overview](docs/PRIVACY_AND_ACCESSIBILITY.md) · [Privacy policy](https://argulab.netlify.app/privacy) · [Terms](https://argulab.netlify.app/terms) · [Cookies](https://argulab.netlify.app/cookies) · [Refund policy](https://argulab.netlify.app/refunds) · [Accessibility](https://argulab.netlify.app/accessibility) · [Licenses](https://argulab.netlify.app/licenses)

## About this repository

This is ArguLab's public product documentation and release-history repository. It contains descriptions and the supplied brand logo. The application source, prompts, tests, deployment configuration and credentials are maintained separately in a private repository. This repository is not an installable copy of the app.

See [NOTICE.md](NOTICE.md) for the publication scope and rights notice.
