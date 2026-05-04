# Changelog

All notable changes to this project are documented in this file.

## Prismatic 0.0.0

Status: still a prototype, but now a usable prototype.

Prismatic reflects the current stage of Designer: like light through a prism, the product now has multiple viable directions, and this phase is about choosing which reflected beam to follow next.

### Added

- Usable single-file prototype with real AI integration (OpenRouter + Gemini)
- Onboarding flow with name, gender, goals, and vibe selection
- Mode system: Relaxed, Real, Locked in, Beast, Brutal
- Profile generation with score, tier, strengths, weaknesses, and roadmap
- Full screen loop: Home, Chat, Audit, Profile
- Transfer import/export for local profile portability
- Photo upload and progress comparison
- Score history tracking and chart view
- Intake answers viewer modal
- Brutal mode confirmation gate
- Shareable score card modal
- Reminder settings screen with local persistence
- Score unlock milestone overlay
- Category drill-down details
- To-Do task screen from roadmap with persistent check state
- Daily micro-prompt loop
- "What does 90 look like?" coaching CTA

### Changed

- AI coaching prompt now asks for a concrete real-life scenario during personality/confidence coaching before giving advice

### Fixed

- Chat score header now displays correctly
- Profile action trigger now waits for better chat completion signal and higher fallback threshold

## Version naming policy

- One-word codenames are for major updates only (for example, 1.x.x to 2.x.x)
- Do not assign codenames for minor/patch ranges (for example, 1.1.5 to 1.6.0)
