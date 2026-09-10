# Wild Eggs Content Engine

Source of truth for campaign copy and the media-facing documents generated from it.

## Campaigns

- `campaigns/spice-spice-baby/`: Fall LTO 2026, on sale Sep 30 to Nov 24, 2026.
  Live menu page: https://www.wildeggs.com/menu/fall-lto

## How the media fact sheet works

`media-fact-sheet.md` is the source for the Google Doc we send in response to
press requests. Edit the markdown here, then re-publish to the Doc so the two
never drift.

Item names, prices, descriptions and allergens come from the **Framer CMS**
(`Menu Items` collection, category "Limited Time Only"). Read it with the Framer
MCP tools or the CLI. The CMS is the source of truth, not the rendered page, not
the tasting sheet and not the Monday tracker. The landing page only surfaces a
subset of each record, so scraping it loses most of the ingredient detail and
several prices.

Anything the CMS does not yet specify stays out of the fact sheet and gets logged
in `open-items.md` instead. The fact sheet is written to be forwarded to a
reporter as-is, so it carries no internal notes.

## House style

No em-dashes. Use commas, colons, periods or parentheses instead. Same for
en-dashes in ranges: write "Sep 30 to Nov 24", not a dash. This applies to menu
copy, press documents and internal notes alike.
