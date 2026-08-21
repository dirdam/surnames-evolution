# Surnames Evolution

Go to **[https://dirdam.squadro.app/surnames/](https://dirdam.squadro.app/surnames/)** to access the app.

A population simulation: starting from a country's most common surnames, a seeded
population of 2,000 people is simulated generation by generation — marrying, having
children, and dying by real age-based mortality rates — until either one surname
takes over everyone, or the mix stays stable for a thousand years. Watch it as a
streamgraph, pick a dataset (US/Spain/Japan census surname frequencies) independently
of the UI language (English/Spanish/Japanese), and control playback speed.

Rebuilt from an older portfolio project (`dirdam.github.io/projects/evo/`) as a
standalone app in the same style as `solis`/`timezones`/`flags`. The original engine
was fully de-obfuscated before porting, so every rule/constant here (mating window,
birth-probability decay, death rates, population safety valve, end conditions) is a
faithful behavioral port, not a re-guess — see this repo's git history / the original
planning notes for the exact derivation.

Fully static (no backend, no build step, no external CDN dependencies) — a single
self-contained `index.html`.
