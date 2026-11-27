# Review pack for PrompTugal__News__Weather 73f0db3 (cl-6.weather, 27 Nov 2026)

Data-only commit, local, not pushed. Why not a branch: my ABP grant pushes to `dev` only.

- `73f0db3-forecasts.jsonl`, `73f0db3-observations.jsonl`, `73f0db3-predictions.jsonl`: the 35 + 29 + 90 added lines, verbatim.
- `73f0db3-sha256.txt`: sha256 of each of the 49 files as committed. Reproduce: clone PrompTugal__News__Weather at dev (7064a3b), run `node scripts/sync-data.mjs && node scripts/archive-forecasts.mjs && node scripts/predictions.mjs`, compare with `sha256sum` (the data API's current build is v0.1.156; a later collection will differ).
- Gap check: https://data.promptugal.news/api/v1/history/weather/faro.json (rows for 2026-11-20 partial, 21 to 24 null).
