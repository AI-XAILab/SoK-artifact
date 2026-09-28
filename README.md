# SoK: Interpretable by Design, Secure by Design? — anonymous evidence artifact

Companion research artifact for the anonymized manuscript. It contains 55 curated literature records and 215 citations in the context/reference inventory. Neither number is a count of independent security attack demonstrations or an exhaustive estimate of the whole field.

## What the files reproduce

- `evidence_map.csv` (55 records): model family, evidence role, topical ICS descriptions, and source-review provenance. Architecture, boundary, reliability, and secondary-survey papers have distinct roles and are not treated as direct intrinsic security experiments.
- `context_corpus.csv`, `citation_trace.csv` (215 references each): citation inventory and role in the manuscript. Being cited does not imply security-experiment evidence.
- `coverage_summary.csv`: reproducible **descriptive counts, keys, and referential checks**, not a statistical prevalence estimate or scientific truth test.
- `codebook.csv`, `evidence_role_mapping.csv`, `search_protocol.md`: category meanings and coverage-oriented selection approach. This is not an exhaustive PRISMA search and no independent two-reviewer screening is claimed.
- `figure6_source_matrix_from_table_XII.csv`, `figure6_36_cell_evidence_ledger.csv`: 36 qualitative family × threat-domain classifications, now with representative coded record references, titles, and an explicit bounded reason for each cell. These are **not computed** from 55 per-paper P1–P6 score vectors; the figure is an author-level synthesis limited to this corpus.

## Interpretation and publication

The submitting author reports reviewing all cited publications. This author confirmation is stated explicitly in the CSVs and provenance note, while earlier selective independent checks remain separately labeled. Detailed supporting page/section locators for every coded claim and original exhaustive search-run logs were not present in the supplied working materials and are not invented.

The manuscript reports no novel experiments or attack payloads. Repository hosting must preserve the double-anonymous process: exclude identifying usernames, institutional information, and author-only QA files. Upload only this anonymous artifact to a neutral anonymous repository, then submit its actual URL in HotCRP; the paper PDF is submitted separately.


## Figure 6 audit path

For any figure cell, locate its family and threat domain in `figure6_36_cell_evidence_ledger.csv`, follow each numbered citation to `evidence_map.csv` and the bibliography, and compare the stated rationale against the original publication. A direct label means the topic is directly addressed in a cited coded paper, **not** that all studies in the family underwent identical adversarial tests. Open means no direct study was coded **within this curated set**. Six displayed families contain 47 coded records in total; the remaining eight are separate secondary/evaluation resources in `coverage_summary.csv`.
