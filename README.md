# Wild Eggs Content Engine

Source of truth for campaign copy and the media-facing documents generated from it.

## Campaigns

- `campaigns/spice-spice-baby/` — Fall LTO 2026, on sale Sep 30 – Nov 24, 2026.
  Live menu page: https://www.wildeggs.com/menu/fall-lto

## How the media fact sheet works

`media-fact-sheet.md` is the source for the Google Doc we send in response to
press requests. Edit the markdown here, then re-publish to the Doc so the two
never drift. Item names, descriptions and prices are reconciled against the live
Framer page — that page is the external source of truth, not the tasting sheet
or the Monday tracker.

Anything not yet confirmed by the kitchen or the bar stays out of the fact sheet
and gets logged in `open-items.md` instead. The fact sheet is written to be
forwarded to a reporter as-is, so it carries no internal notes.
