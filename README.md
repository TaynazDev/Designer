# Designer by Prism

Designer is a single-file HTML prototype for an AI personal style and self-improvement app in the Prism Suite.

Live demo: https://taynazdev.github.io/Designer

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
- ds_checkins
- ds_score_start
- ds_profile

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
