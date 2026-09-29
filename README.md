# Vicky's Japan Life Tracker v3.1.1

v3.1 UX patch: departure date now follows the selected arrival date by default.

Scope-frozen core build: rolling 365 dashboard, trips, multi-city route field, stays, Asakusa Home concept, Guess My Stay-ready data model, restaurant passport, dining companions, JSON import/export, and offline PWA shell.

## Important date behavior
Japan days are counted as calendar days with both arrival and departure dates included, matching the v1 tracker behavior. Overlapping trips are currently summed; avoid duplicate/overlapping country records when entering data.

## v1 migration
The importer accepts either a v1-style array or a backup object containing `trips`. It maps `country`, `city`, `start`/`arrival`, and `end`/`departure`.

## Run
For offline PWA/service-worker behavior, serve this folder over HTTPS (GitHub Pages or Cloudflare Pages) or localhost. Opening `index.html` directly still lets the core tracker work, but service-worker installation requires a secure context.


### v3.1 UX fixes
- Departure defaults to the selected arrival date when adding a trip.
- Existing trips can be edited as well as deleted.
