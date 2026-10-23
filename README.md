<img src="favicon.svg" width="72" height="72" alt="Porchlamp's symbol: a porch lamp with its light on">

# Porchlamp

**Find the projects that leave the light on.**

A porch lamp left on tells a visitor they are expected. Porchlamp ranks
open-source projects the same way: by what happens to a stranger's pull
request, not by how many stars the project has.

**Open the ranking: https://porchlamp.org/**

**Read the report, with charts and the method: https://porchlamp.org/black-holes/**

## Stars don't review pull requests

Measured on the 2026-10-24 snapshot of 11,000 projects:

- **More than 1 in 5 active projects are black holes.** Of the 4,125 licensed,
  maintained software projects with at least ten counted outside pull requests
  in six months, 845 (20.5%) left most of them with no human reply, review or
  merge for two weeks. We could not judge 184 busy projects yet: we hold only
  the newest 500 pull requests of each, and they do not reach back to 25 April.
- **More stars, more silence.** The black-hole share rises with popularity: 17%
  of projects with 1k–10k stars, 24% at 10k–50k, and 27% at 50k or more.
- **Stars barely predict the ranking.** Across the 2,765 ranked projects the
  rank correlation between stars and the Porchlamp score is 0.03, and 1 of the
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
from precomputed JSON under `data/2026-10-24/` by `api.js` (project records sharded into 256
hash-bucketed files under `data/2026-10-24/repos/`), so the site needs no
server.

- **Snapshot ID:** `2026-10-24` (measured as of `2026-10-22T22:47:00+00:00`, benchmark `2.0.0-rc1`)
- **Universe Counts:** `2,765` rated (ranked) · `5,506` gated (Stage 0) · `2,729` unrated (`<60%` coverage) · `11,000` total
- **Persona Visible Counts:** `balanced: 2,765` · `first_timer: 1,497` · `career_capital: 510` · `senior_systems: 1,019` · `ai_assisted: 3,256`
- **Verification Hashes:** `constants_hash: d8c067b9e928…` · `manifest_root: a9ba6065bf64…` · `canonical_dump_hash: ed57ff66801c…`

## License and citation

The data under `data/` and the text of this site are licensed under [CC BY 4.0](LICENSE): reuse them freely, with credit to "Porchlamp rankings" and a link to https://porchlamp.org/. To cite the dataset, use GitHub's "Cite this repository" button, which reads `CITATION.cff`. To cite a finding, link the report frozen for this snapshot: https://porchlamp.org/black-holes/2026-10-24/ . The code in this repository is not covered by this license, and the engine that collects the data is private.
