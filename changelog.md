# Changelog

All notable changes to this project are documented in this file.

## 0.0.2

### Added

- Photo Vision V2 with richer structured analysis: hair status/score, body presentation band, silhouette read, key pieces, and trend directions
- In-browser camera capture in Photos modal (take photo directly without leaving app)
- One-time "What's New: Vision V2" popup with local acknowledgement persistence
- Trend direction library expanded for male/female/unisex coaching examples

### Changed

- Vision V2 context is now forced into ongoing coaching prompts (always-on visual anchoring)
- Chat photo analysis now uses Vision V2 outputs and returns trend-biased look formulas
- Onboarding no longer forces preset style-vibe selection; style direction is now defined in intake
- Intake prompt behavior updated to establish style direction when missing and modernize outdated aesthetics

### Fixed

- Transfer import parser hardened for more pasted formats and noisy payload wrappers
- Transfer import now reports explicit status/errors instead of failing silently
- Import flow now handles localStorage quota limits with progressive fallback (drop photos/chat history when needed)
- Missing tier helper restored to prevent runtime "getTier is not defined" failures

## 0.0.1

### Added

- Unified quick check-in path so daily micro prompt and chat quick-check use the same flow
- Per-prompt live score movement in chat/check-ins (score can go up or down after each user prompt)

### Changed

- Sign-in/import routing now lands directly in the app when account data is present
- Mode changes no longer force users into a new intake chat if a profile already exists
- Deferred tracker organization updated: version-name section moved to the bottom
- Post-MVP feature items moved out of deferred tracker into README backlog section

### Fixed

- Transfer/import flow no longer auto-overwrites pasted transfer docs on modal open
- Import no longer falls back to stale local identity fields when restoring account data
- Remaining mojibake/symbol rendering issues in app UI text were corrected

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
