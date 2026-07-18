# Core 1 Trainer

A free, gamified CompTIA A+ 220-1101 (Core 1) study app — no paywall, no login, no subscription.

Built as an alternative to paid "AI tutor" cert-prep apps that lock most content behind a subscription.

## Features

- **5 domains, 15 lessons, 80+ questions** mapped to the real 220-1101 exam objectives (Mobile Devices, Networking, Hardware, Virtualization & Cloud, Hardware & Network Troubleshooting)
- **Diagnostic test** — 20 questions sampled proportionally to the actual exam blueprint weighting, with a domain-by-domain score breakdown
- **Review missed questions** — see exactly what you got wrong and why, not just a percentage
- **Diagnostic history** — tracks your score over time so you can see improvement run to run
- **XP + streak system** — lightweight gamification to keep you coming back
- **Instant explanations** after every question, correct or not
- **AI hint button** — optional; requires the Anthropic API and is meant to run inside Claude.ai (see note below)

## Running it

This is a single self-contained HTML file — no build step, no dependencies. Just open `index.html` in a browser, or serve it via GitHub Pages.

Progress is saved locally in your browser via `localStorage`, so it's private to whatever browser/device you're using it from.

## Note on the AI hint feature

The "Ask for a hint" button calls the Anthropic API directly from the browser. That only works when this app is rendered inside Claude.ai (which proxies the request). Hosted standalone (e.g. on GitHub Pages), that button will fail gracefully and show a fallback message instead of a real hint — everything else works normally.

## Disclaimer

Independent study tool, not affiliated with or endorsed by CompTIA.
