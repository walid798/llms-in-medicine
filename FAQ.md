# FAQ

## How many studies are in the current review?
The frozen quantitative corpus contains **145 studies**, published from 2022 through 2026.

## Why does the repository no longer organize the evidence only by task?
The revised review is centered on multimodal fusion, retrieval/reasoning/agents, personalization, safety, and translational maturity. Clinical task remains available in the master register.

## Are BERT, BioBERT, ClinicalBERT, and PubMedBERT included?
They are important contextual models, but standalone encoder-only PLMs are not part of the primary quantitative corpus unless embedded within an LLM-centered evaluated system.

## Are preprints allowed?
Methodologically complete preprints may be included when no corresponding peer-reviewed version is available at the final search date.

## What do F0–F5, P0–P5, and T0–T5 mean?
See `data/codebook.csv`.

## Which file is the source of truth?
`data/Final_145_Studies_FROZEN.xlsm`.

## Can I add a new paper directly as S146?
Not to the frozen corpus. Submit it through the contribution workflow for the next version.
