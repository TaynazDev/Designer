# Designer by Prism

Current prototype release: Prismatic 0.0.0

Designer is a single-file HTML prototype for an AI personal style and self-improvement app in the Prism Suite.

Live demo: https://taynazdev.github.io/Designer

## Version concept

This version is named Prismatic 0.0.0.

Prismatic reflects the core moment this product is in: light splitting into multiple directions. The app is now a usable prototype, and this stage is about choosing which reflected beam to commit to next.

Status note: still a prototype, but now a usable prototype.

## Changelog

### Prismatic 0.0.0

- Established a usable single-file prototype with real AI integration (OpenRouter + Gemini).
- Added onboarding flow with name, gender, goals, and vibe selection.
- Implemented mode system (Relaxed, Real, Locked in, Beast, Brutal) with mode-specific coaching behavior.
- Added profile generation with score, tier, strengths, weaknesses, and AI roadmap.
- Added full dashboard loop: Home, Chat, Audit, Profile.
- Added transfer import/export for local profile portability.
- Added photo upload and progress comparison.
- Added score history tracking and chart view.
- Added intake answers viewer modal.
- Added Brutal mode confirmation gate.
- Added shareable score card modal.
- Added reminder settings screen and local persistence.
- Added score unlock milestone overlay.
- Added category drill-down details.
- Added To-Do task screen from roadmap with persistent check state.
- Added daily micro-prompt loop and 90-vision coaching CTA.
- Fixed chat score header display and improved profile update trigger threshold.
- Improved AI coaching prompt to require concrete real-life examples in personality/confidence coaching.

Naming policy:
- Word codenames are for major updates only (for example, 1.x.x to 2.x.x).
- Do not assign new codenames for minor/patch updates (for example, 1.1.5 to 1.6.0).

## What it does

- Runs as a static site with no build step.
- Uses real AI providers from the browser: OpenRouter or Google Gemini.
- Stores local app state in localStorage.
- Guides onboarding with name, gender, goals, and desired vibe.
- Builds an AI-generated profile with scores, strengths, weaknesses, and a tiered roadmap.

## Main screens

- Onboarding
- Mode selection
- API key setup
- Intake / check-in chat
- Home dashboard
- Audit
- Profile
- Deferred features tracker

## Roadmap model

The app structures improvement actions into three AI-controlled tiers:

- now: free or immediate actions
- effort: actions needing some money, planning, or routine changes
- time: actions that take weeks or months to improve

The AI can fully restructure the roadmap each session based on what is strongest or weakest.

## Local storage keys

- ds_api_key
- ds_api_type
- ds_name
- ds_mode
- ds_gender
- ds_vibe
- ds_goals
- ds_chat_history
- ds_chat_type
- ds_checkins
- ds_score_start
- ds_profile
- ds_photos
- ds_score_history
- ds_remind
- ds_todo_checked
- ds_last_micro
- ds_audience
- ds_legacy_score
- ds_changed_log
- ds_todo_events
- ds_quick_win
- ds_weekly_drop

## Transfer document / sign-in import

Designer currently supports device-to-device account transfer through a portable transfer document. In the prototype, this acts as the app's sign-in/import path for moving an account between devices without a backend.

What the transfer document includes:

- API key and provider type
- Name, gender, mode, vibe, audience, and goals
- Current profile JSON
- Check-in count and starting score
- Chat type and chat history
- Photos
- Score history
- Reminder settings
- To-do checked state and to-do events
- Last micro-prompt date
- Legacy score
- What changed log
- Quick win mode state
- Weekly drop state

Notes:

- This is a full local account snapshot, not just a profile summary.
- Because photos are embedded in the document, large accounts can produce very large transfer text.
- This is a local prototype portability feature, not a secure cloud sign-in system.

## Files

- designer-app.html: the working app prototype
- index.html: GitHub Pages entry redirect
- designer-deferred.html: deferred work tracker
- designer-plan.html: original product spec
- prism-branding-theme.html: branding/theme reference

## Running locally

Open designer-app.html directly in a browser, or serve the folder with any static file server.

## Notes

- API keys are stored locally in the browser and sent only to the chosen AI provider.
- The demo URL above reflects the requested deployment URL text. If GitHub Pages is using the repository name path, update the link to match the published site path.

## Parked Backlog (Hidden From Deferred Tracker)

These are intentionally moved out of `designer-deferred.html` so the active deferred list stays focused.

### Backend And Ecosystem (Moved From Deferred)

- Profile persistence (Supabase): profiles, scores, check_ins, photo_analyses tables, profile JSON persistence, and row-level score history.
- Prism ID auth: shared sign-in and sign-up across Prism apps (suite-level identity).
- Rate limiting (Upstash Redis): free/pro session caps and separate tracking for vision calls.
- Roast-to-fix pipeline (Prism Roast to Designer): one-tap import from Prism Roast into Designer scoring and roadmap updates.

### Prism Suite Integrations (Post-MVP)

- Prism Mood to AI tone shift
- Prism Grind to roadmap sync
- Prism Roast to check-in import
- Prism Social to score share

### Product Features (Post-MVP)

- Score battles (viral mode): two-user Beast-mode category comparison with winner card for sharing.
- Designer wrapped: monthly/yearly recap card (journey, improvements, best week, worst week, dominant mode).
- Glow-up verified badge: journey-based badge for meaningful improvement threshold (for example, +20 from start).
- Friend audit: anonymous friend photo audit with strong safety framing and consent language.
- Accountability partner: paired accountability sharing roadmap completion only (not scores), anonymous by default until mutual reveal.
- Designer certified annual certificate: yearly certificate for consistent check-ins plus meaningful improvement.
- Waitlist aura prelaunch flow: prelaunch waitlist with one-line vibe submission and AI one-line reaction.
- My Designer told me quote cards: save sharp AI lines as shareable quote cards with score and mode badge.
- Improvement leaderboard (opt-in): rank users by gain from baseline with weekly reset and privacy control.

### Monetisation (Not Wired)

- Paywall / upgrade flow
- Designer Pro subscription management
- Prism Pass bundle
