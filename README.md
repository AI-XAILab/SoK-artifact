# SoK: Interpretable by Design, Secure by Design? — Anonymous Research Artifact

This repository accompanies the anonymized Systematization of Knowledge (SoK) manuscript **“Interpretable by Design, Secure by Design?”**.

The artifact supports the paper’s **coverage-oriented evidence synthesis**. It is intended to make the paper’s corpus construction, coding scheme, descriptive coverage counts, citation roles, and Figure 6 qualitative synthesis easier to inspect.

## Scope

The manuscript distinguishes between:

- a **55-work coded evidence map** used for quantitative coverage observations; and
- a broader **215-reference context corpus** used to establish architectural, methodological, privacy, adversarial-ML, and interpretability context.

The 55 coded works include direct security evidence, reliability evidence, verification evidence, boundary evidence, architecture-related evidence, and secondary systematizations/evaluation resources. Therefore, the 55 records **must not be interpreted as 55 independent attack demonstrations**.

The search and selection process is **coverage-oriented rather than an exhaustive bibliometric census**. The repository does not claim PRISMA-style exhaustive retrieval or independent dual-reviewer screening.

## Repository Contents

| File | Purpose |
|---|---|
| `evidence_map.csv` | The 55-work coded evidence map used for the manuscript’s coverage-oriented analysis. |
| `context_corpus.csv` | The broader 215-reference contextual bibliography used to establish the surrounding literature and architectural scope. |
| `citation_trace.csv` | Trace of the 215 context references and their role in the manuscript. |
| `coverage_summary.csv` | Descriptive counts for the coded evidence set. These counts describe this curated corpus and are not prevalence estimates for the full research field. |
| `codebook.csv` | Operational definitions used to interpret the coded evidence categories. |
| `evidence_role_mapping.csv` | Mapping of evidence roles used to distinguish direct, reliability, verification, boundary, and secondary evidence. |
| `search_protocol.md` | Coverage-oriented search, expansion, inclusion, exclusion, and coding protocol, together with its reproducibility boundaries. |
| `figure6_source_matrix_from_table_XII.csv` | Source matrix corresponding to the six family × threat-domain classifications reported in the manuscript. |
| `figure6_36_cell_evidence_ledger.csv` | Cell-level evidence ledger for the 36 family × threat-domain entries underlying Figure 6 / Appendix Table XII, including representative references and bounded rationales. |

## Evidence Roles

The artifact separates several kinds of evidence rather than treating every cited paper as a direct security experiment.

- **Direct security evidence**: explicit adversary, attack, defense, or security evaluation.
- **Direct reliability evidence**: evaluation of failures such as instability, semantic misalignment, noisy concepts, or non-identifiability that can affect trustworthy auditing.
- **Direct verification evidence**: formal or explicit verification of a relevant property.
- **Boundary evidence**: adjacent post-hoc XAI, privacy, or related work used to establish mechanisms that may motivate transfer questions for intrinsic carriers.
- **Secondary evidence**: surveys, SoKs, and evaluation resources used for framing, search seeding, and comparison.

These categories should be interpreted according to `codebook.csv` and `evidence_role_mapping.csv`.

## Coverage-Oriented Search Protocol

The artifact documents a structured mapping procedure based on:

1. seed surveys and systematizations;
2. backward and forward snowballing;
3. targeted combinations of intrinsic-carrier terms with trustworthiness/security terms;
4. explicit inclusion and exclusion rules; and
5. row-level coding by carrier family, evidence role, attack/failure locus, and relevant ICS property.

The supplied working material does **not** contain complete original records for:

- all search databases/interfaces,
- exact query strings and execution dates,
- full retrieval and deduplication counts,
- per-stage screening/exclusion counts,
- complete snowballing timestamps, or
- independent dual-screening agreement/adjudication.

Accordingly, these items are not reconstructed or invented in this artifact.

## Figure 6 / Appendix Table XII

Figure 6 is a **qualitative family × threat-domain synthesis**, not a numerical score computed from 55 per-paper P1–P6 vectors.

The two supporting files are:

- `figure6_source_matrix_from_table_XII.csv`
- `figure6_36_cell_evidence_ledger.csv`

For each of the 36 cells, the ledger provides representative manuscript references and a bounded rationale. Labels such as **direct**, **adjacent**, and **open** apply to the curated corpus and should not be interpreted as universal statements about the entire literature.

In particular:

- **direct** means that the topic is directly represented by evidence in the curated corpus;
- **adjacent** means that the available evidence informs the topic without directly establishing it under the paper’s definition; and
- **open** means that no direct study was coded for that cell within this curated evidence set.

## Reproducibility and Interpretation Boundaries

This artifact is designed to support **auditability of the manuscript’s evidence organization**, not to certify the scientific correctness of every cited publication.

The repository therefore supports inspection of:

- corpus membership,
- evidence-role assignments,
- descriptive counts,
- citation roles,
- coding definitions, and
- the rationale behind the manuscript’s Figure 6 synthesis.


## Suggested Audit Path

To inspect a claim associated with the coded evidence map:

1. locate the corresponding record in `evidence_map.csv`;
2. check the evidence-role definition in `codebook.csv` and `evidence_role_mapping.csv`;
3. use `citation_trace.csv` and `context_corpus.csv` to inspect the paper’s role in the broader manuscript context; and
4. for Figure 6 claims, inspect the matching family × threat-domain entry in `figure6_36_cell_evidence_ledger.csv` and compare its representative references with the manuscript bibliography and the original publications.

## Anonymity

This repository is prepared for double-anonymous review. It intentionally excludes author names, institutional identifiers, personal contact information, and other identifying metadata.

