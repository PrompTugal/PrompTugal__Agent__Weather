# cl-6.weather: now

Updated 2026-11-26T01:43Z.

## State
- Key published and signed commits work. History is in `history/` (PROVENANCE.md, git-log.md).
- **The section site is stale.** weather.promptugal.news serves v0.1.71, built 2026-11-21T08:20Z, data read 2026-11-21T07:12Z: five days old. The last predictions run was 21 Nov (18 lines, due 20 Nov; first outcomes 32 held, 4 missed, all four misses Monchique). It is meant to be refreshed twice a day.
- **Blocked:** my session's `add_repo` for PrompTugal__News__Weather was refused by the permission check, so I can read the repository (public clone) but not push to it. I did not work around it.

## First wake once I can push (in this order)
1. Pull dev, read CLAUDE.md, the website's "New from Dinis" list, any HOLD.
2. `node scripts/sync-data.mjs`, `node scripts/archive-forecasts.mjs`, `node scripts/predictions.mjs`; commit `data/history/` and `data/predictions/`. Five days of forecasts were not archived: say so on the track-record page (a gap, never filled).
3. Record outcomes for 21 to 25 Nov; rebuild; check the gate.
4. Then: forecast-accuracy page (Faro first, station 1200554, then London); see `history/board/team/weather/status.json` "next".
5. The new iOS app reads the site: check that /version.json, /preview.json and the per-place data files stay stable, and tell the conductor of any change to them.

## Open asks (from weather.b, still open)
- Yes or no on a CI workflow edit (.github/workflows/pages.yml) for security@'s controls 7 to 9: Dinis's.
- Signed commits in the section repository (check-signatures from data.b@'s pattern): now possible, since ssh-keygen works here.
