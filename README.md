<img src="favicon.svg" width="72" height="72" alt="Porchlamp's symbol: a porch lamp with its light on">

# Porchlamp

**Find the projects that leave the light on.**

A porch lamp left on tells a visitor they are expected. Porchlamp ranks
open-source projects the same way: by what happens to a stranger's pull
request, not by how many stars the project has.

**Open the ranking: https://porchlamp.org/**

**Read the report, with charts and the method: https://porchlamp.org/black-holes/**

## Stars don't review pull requests

Measured on the 2026-10-17 snapshot of 11,000 projects:

- **More than 1 in 5 active projects are black holes.** Of the 2,745 licensed,
  maintained software projects with at least ten counted outside pull requests
  in six months, 638 (23.2%) left most of them with no human reply, review or
  merge for two weeks. We could not judge 868 busy projects yet: we hold only
  the newest 500 pull requests of each, and they do not reach back to 20 April.
- **More stars, more silence.** The black-hole share rises with popularity: 19%
  of projects with 1k–10k stars, 30% at 10k–50k, and 35% at 50k or more.
- **Stars barely predict the ranking.** Across the 4,396 ranked projects the
  rank correlation between stars and the Porchlamp score is 0.08, and 10 of the
  100 most-starred projects make the top 100.

## Where the numbers come from

We followed 614,499 pull requests from 148,789 outside contributors to 11,000
projects over six months: who got an answer, how fast, how many reached a
decision, whether first-time contributors came back, and how much other software
depends on each project. Black holes, and projects that are archived,
unmaintained, unlicensed or not software, are listed but never ranked. The rest
are scored on five pillars and re-weighted for five kinds of contributor. Every
number traces back to a recorded GitHub response and its content hash.

## This repository

This repository is the published site and nothing else: a static snapshot
served by GitHub Pages. Every ranking, filter and project page is answered
from precomputed JSON under `data/2026-10-17/` by `api.js` (project records sharded into 256
hash-bucketed files under `data/2026-10-17/repos/`), so the site needs no
server.

- **Snapshot ID:** `2026-10-17` (measured as of `2026-10-17T05:35:00+00:00`, benchmark `2.0.0-rc1`)
- **Universe Counts:** `4,396` rated (ranked) · `5,299` gated (Stage 0) · `1,305` unrated (`<60%` coverage) · `11,000` total
- **Persona Visible Counts:** `balanced: 4,396` · `first_timer: 2,157` · `career_capital: 926` · `senior_systems: 1,375` · `ai_assisted: 4,516`
- **Verification Hashes:** `constants_hash: 6f95d75a0aa5…` · `manifest_root: 01a8d825306a…` · `canonical_dump_hash: 1f08e18ca9c8…`

## License and citation

The data under `data/` and the text of this site are licensed under [CC BY 4.0](LICENSE): reuse them freely, with credit to "Porchlamp rankings" and a link to https://porchlamp.org/. To cite the dataset, use GitHub's "Cite this repository" button, which reads `CITATION.cff`. To cite a finding, link the report frozen for this snapshot: https://porchlamp.org/black-holes/2026-10-17/ . The code in this repository is not covered by this license, and the engine that collects the data is private.
