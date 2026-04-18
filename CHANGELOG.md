# Changelog

## 2026-04

- Initial dictionary seeded from haiku-to-haiku dialogic run (2026-04-07)
- 20 terms agreed across 4 negotiation cycles (18 dropped)
- Paradigm: minimal-seed-dialogic, Husserlian × Heideggerian personas
- Models: two instances of `claude-haiku-4-5-20251001`
- Static JSON API built and deployed to GitHub Pages
- Cloudflare Worker proxy configured (`ai-dictionary-haiku-to-haiku-proxy`)
- Added `bot/build_reputation.py` (missing import was breaking the Build API workflow and leaving terms without `consensus` / `interest` / `vitality` fields — which in turn threw in modal rendering and made term cards appear unclickable)
- Rebuilt API to expose cross-model consensus (run 1/7) on all 20 terms
