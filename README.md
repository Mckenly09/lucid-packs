# Lucid subject packs

Offline study notes for [Lucid](https://github.com/Mckenly09/lucid), the offline AI study app. Each pack is a small SQLite file (full-text search) that the app downloads once and searches on the phone when answering a question.

- `catalog.json` — the list the app reads (id, version, size, sha256, license, attribution).
- `packs/<id>-v<version>.sqlite` — the packs. Built by `tools/packs` in the Lucid repo; don't edit by hand (the app checks the sha256).

## Packs and licenses

Every pack carries its source's license and attribution (also stored inside the file, in the `meta` table).

| Pack | Source | License |
|---|---|---|
| `science-chem` · Science · Chemistry (Grades 7–10) | Adapted from *Chemistry 2e* by Paul Flowers, Klaus Theopold, Richard Langley, William R. Robinson (OpenStax, Rice University), https://openstax.org/details/books/chemistry-2e. Access for free at openstax.org. | [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) |

Changes made to the sources: text split into short notes by section; figures, tables and exercises removed; math written as plain text. Packs adapted from ShareAlike sources are shared under the same license. NonCommercial packs may not be used commercially.
