<img src="favicon.svg" width="72" height="72" alt="Porchlamp's symbol: a porch lamp with its light on">

# Porchlamp

**Find the projects that leave the light on.**

A porch lamp left on tells a visitor they are expected. Porchlamp ranks
open-source projects the same way: by what happens to a stranger's pull
request, not by how many stars the project has.

**Open the ranking: https://porchlamp.org/**

**Read the report, with charts and the method: https://porchlamp.org/black-holes/**

## Stars don't review pull requests

Measured on the 2026-10-25 snapshot of 11,000 projects:

- **More than 1 in 8 active projects are black holes.** Of the 4,168 licensed,
  maintained software projects with at least ten counted outside pull requests
  in six months, 567 (13.6%) left most of them with no human reply, review,
  merge or close within two weeks or since. We could not judge 184 busy projects yet: we hold only
  the newest 500 pull requests of each, and they do not reach back to 25 April.
- **More stars, more silence.** The black-hole share rises with popularity: 11%
  of projects with 1k–10k stars, 17% at 10k–50k, and 17% at 50k or more.
- **Stars barely predict the ranking.** Across the 3,027 ranked projects the
  rank correlation between stars and the Porchlamp score is 0.00, and 1 of the
  100 most-starred projects makes the top 100.

## Where the numbers come from

We followed 1,442,863 pull requests from 227,260 outside contributors to 11,000
projects over six months: who got an answer, how fast, how many reached a
decision, whether first-time contributors came back, and how much other software
depends on each project. Black holes, and projects that are archived,
unmaintained, unlicensed or not software, are listed but never ranked. The rest
are scored on five pillars and re-weighted for five kinds of contributor. Every
number traces back to a recorded GitHub response and its content hash.

## This repository

This repository is the published site and nothing else: a static snapshot
served by GitHub Pages. Every ranking, filter and project page is answered
from precomputed JSON under `data/2026-10-25/` by `api.js` (project records sharded into 256
hash-bucketed files under `data/2026-10-25/repos/`), so the site needs no
server.

- **Snapshot ID:** `2026-10-25` (measured as of `2026-10-22T22:47:00+00:00`, benchmark `2.0.0-rc1`)
- **Universe Counts:** `3,027` rated (ranked) · `5,099` gated (Stage 0) · `2,874` unrated (`<60%` coverage) · `11,000` total
- **Persona Visible Counts:** `balanced: 3,027` · `first_timer: 1,636` · `career_capital: 553` · `senior_systems: 1,101` · `ai_assisted: 3,541`
- **Verification Hashes:** `constants_hash: de2c71c1d7ba…` · `manifest_root: ee5e52f23120…` · `canonical_dump_hash: 766e12564ccc…`

## License and citation

The data under `data/` and the text of this site are licensed under [CC BY 4.0](LICENSE): reuse them freely, with credit to "Porchlamp rankings" and a link to https://porchlamp.org/. To cite the dataset, use GitHub's "Cite this repository" button, which reads `CITATION.cff`. To cite a finding, link the report frozen for this snapshot: https://porchlamp.org/black-holes/2026-10-25/ . The code in this repository is not covered by this license, and the engine that collects the data is private.
