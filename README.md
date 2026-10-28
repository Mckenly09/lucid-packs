# Lucid subject packs

Offline study notes for [Lucid](https://github.com/Mckenly09/lucid), the offline AI study app. Each pack is a small SQLite file (full-text search) that the app downloads once and searches on the phone when answering a question.

- `catalog.json` — the list the app reads (id, version, size, sha256, license, attribution).
- `packs/<id>-v<version>.sqlite` — the packs. Built by `tools/packs` in the Lucid repo; don't edit by hand (the app checks the sha256).

## Packs and licenses

Every pack carries its source's license and attribution (also stored inside the file, in the `meta` table).

| Pack | Source | License |
|---|---|---|
| `science-chem` · Science · Chemistry (Grades 7–10) | Adapted from *Chemistry 2e* by Paul Flowers, Klaus Theopold, Richard Langley, William R. Robinson (OpenStax, Rice University), https://openstax.org/details/books/chemistry-2e. Access for free at openstax.org. | [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) |
| `science-physics` · Science · Physics (Grades 7–10) | Adapted from *Physics* by Paul Peter Urone, Roger Hinrichs (OpenStax, Rice University), https://openstax.org/details/books/physics. Access for free at openstax.org. | [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) |
| `science-bio` · Science · Biology (Grades 7–10) | Adapted from *Concepts of Biology* by Samantha Fowler, Rebecca Roush, James Wise (OpenStax, Rice University), https://openstax.org/details/books/concepts-biology. Access for free at openstax.org. | [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) |
| `math-algebra` · Math · Algebra (Grades 7–9) | Adapted from *Elementary Algebra 2e* by Lynn Marecek, MaryAnne Anthony-Smith, Andrea Honeycutt Mathis (OpenStax, Rice University), https://openstax.org/details/books/elementary-algebra-2e. Access for free at openstax.org. | [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) |
| `math-advanced` · Math · Functions, Sequences and Circles (Grades 8–10) | Adapted from *Intermediate Algebra 2e* by Lynn Marecek, Andrea Honeycutt Mathis (OpenStax, Rice University), https://openstax.org/details/books/intermediate-algebra-2e. Access for free at openstax.org. | [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) |
| `math-geometry` · Math · Geometry Basics (Grade 7) | Adapted from *Prealgebra 2e* by Lynn Marecek, MaryAnne Anthony-Smith, Andrea Honeycutt Mathis (OpenStax, Rice University), https://openstax.org/details/books/prealgebra-2e. Access for free at openstax.org. Chapter 9. | [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) |
| `math-trig-prob` · Math · Trigonometry and Probability (Grades 9–10) | Adapted from *Algebra and Trigonometry 2e* by Jay Abramson (OpenStax, Rice University), https://openstax.org/details/books/algebra-and-trigonometry-2e. Access for free at openstax.org. | [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) |
| `math-genmath-functions` · Math · Gen Math: Functions (Grade 11) | Adapted from *Algebra and Trigonometry 2e* by Jay Abramson (OpenStax, Rice University), https://openstax.org/details/books/algebra-and-trigonometry-2e. Access for free at openstax.org. | [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) |
| `math-genmath-business-logic` · Math · Gen Math: Business Math and Logic (Grade 11) | Adapted from *Contemporary Mathematics* by Donna Kirk (OpenStax, Rice University), https://openstax.org/details/books/contemporary-mathematics. Access for free at openstax.org. | [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) |
| `english-notes` · English · Grammar, Reading and Writing (Grades 7–10) | *Lucid English Notes* by the Lucid contributors — original notes, source in [`content/english/`](content/english/) | [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) |
| `science-earth` · Science · Earth and Space (Grades 7–10) | Adapted from public web pages of the U.S. Geological Survey, NOAA's National Weather Service (JetStream), NASA, DOST-PHIVOLCS and DOST-PAGASA, retrieved 2026-10-28 — [page list below](#science-earth). Not endorsed by these agencies. | US Government: public domain · Philippine Government works: non-commercial use (IP Code §176) |

Changes made to the OpenStax sources: text split into short notes by section; figures, tables, exercises, readiness quizzes, worked examples drawn only as images, and teacher notes removed; math written as plain text (`x^2`, `sqrt(9)`, `cbrt(8)`, `b/(2a)`). Packs adapted from ShareAlike sources are shared under the same license. NonCommercial packs may not be used commercially.

## science-earth

Text adapted from these pages (retrieved 2026-10-28). US Government works are in the public domain (17 U.S.C. §105). Philippine Government works carry no copyright (IP Code §176); their use here is non-commercial, and commercial use needs the agency's approval. This pack is not endorsed by NOAA, NASA, USGS, PHIVOLCS or PAGASA and is not official government material. Changes: split into short notes; images, menus and some tables removed. Each note in the pack links to its page.

- NOAA/NWS — https://www.noaa.gov/jetstream/atmosphere/layers-of-atmosphere (Public domain (US Government))
- NOAA/NWS — https://www.noaa.gov/jetstream/atmosphere/air-pressure (Public domain (US Government))
- NOAA/NWS — https://www.noaa.gov/jetstream/atmosphere/transfer-of-heat-energy (Public domain (US Government))
- NOAA/NWS — https://www.noaa.gov/jetstream/global/global-atmospheric-circulations (Public domain (US Government))
- NOAA/NWS — https://www.noaa.gov/jetstream/tropical/convergence-zone (Public domain (US Government))
- NASA — https://spaceplace.nasa.gov/seasons/en/ (Public domain (US Government))
- USGS — https://pubs.usgs.gov/gip/earthq1/intro.html (Public domain (US Government))
- USGS — https://pubs.usgs.gov/gip/earthq1/how.html (Public domain (US Government))
- USGS — https://pubs.usgs.gov/gip/earthq1/where.html (Public domain (US Government))
- USGS — https://pubs.usgs.gov/gip/earthq1/measure.html (Public domain (US Government))
- USGS — https://pubs.usgs.gov/gip/earthq1/predict.html (Public domain (US Government))
- DOST-PHIVOLCS — https://www.phivolcs.dost.gov.ph/introduction-to-earthquake/ (Philippine Government work)
- DOST-PHIVOLCS — https://www.phivolcs.dost.gov.ph/phivolcs-earthquake-intensity-scale-2/ (Philippine Government work)
- DOST-PHIVOLCS — https://www.phivolcs.dost.gov.ph/introduction-to-tsunami/ (Philippine Government work)
- NOAA/NWS — https://www.noaa.gov/jetstream/tropical/tropical-cyclone-introduction (Public domain (US Government))
- NOAA/NWS — https://www.noaa.gov/jetstream/tropical/tropical-cyclone-introduction/tropical-cyclone-structure (Public domain (US Government))
- NOAA/NWS — https://www.noaa.gov/jetstream/tropical/tropical-cyclone-introduction/tropical-cyclone-classification (Public domain (US Government))
- NOAA/NWS — https://www.noaa.gov/jetstream/tc-hazards (Public domain (US Government))
- DOST-PAGASA — https://www.pagasa.dost.gov.ph/information/about-tropical-cyclone (Philippine Government work)
- DOST-PAGASA — https://www.pagasa.dost.gov.ph/learning-tools/tropical-cyclone-wind-signal (Philippine Government work)
- USGS — https://pubs.usgs.gov/gip/volc/text.html (Public domain (US Government))
- DOST-PHIVOLCS — https://www.phivolcs.dost.gov.ph/introduction-to-volcanoes/ (Philippine Government work)
- NOAA/NWS — https://www.noaa.gov/jetstream/global/climate-vs-weather (Public domain (US Government))
- NOAA/NWS — https://www.noaa.gov/jetstream/global/climate-zones (Public domain (US Government))
- NOAA/NWS — https://www.noaa.gov/jetstream/tropical/enso (Public domain (US Government))
- NASA — https://science.nasa.gov/climate-change/what-is-climate-change/ (Public domain (US Government))
- USGS — https://pubs.usgs.gov/gip/dynamic/historical.html (Public domain (US Government))
- USGS — https://pubs.usgs.gov/gip/dynamic/developing.html (Public domain (US Government))
- USGS — https://pubs.usgs.gov/gip/dynamic/understanding.html (Public domain (US Government))
- USGS — https://pubs.usgs.gov/gip/dynamic/hotspots.html (Public domain (US Government))

## English notes

`english-notes` is built from our own Markdown notes in [`content/english/`](content/english/), licensed [CC BY 4.0](content/english/LICENSE). Corrections from teachers are welcome.

