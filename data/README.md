# Data files

`Final_145_Studies_FROZEN.xlsm` is the frozen source evidence matrix.

Derived machine-readable exports:

- `studies.csv` — master study register enriched with the main coding dimensions used by the repository.
- `studies.jsonl` — one JSON object per included study.
- `architecture_fusion.csv` — architecture, adaptation, fusion, RAG, and tool-use coding.
- `performance.csv` — study-level performance extraction as stored in the frozen matrix.
- `personalization_safety.csv` — personalization, retrieval, agentic reasoning, safety, risk-mitigation evidence, and translational maturity.
- `codebook.csv` — operational coding definitions.
- `review_metadata.json` — corpus-level counts used in the README and figures.

## Source-of-truth rule

Study IDs `S001`–`S145` are stable. Do not renumber existing studies when updating the repository.

The frozen workbook is preserved unchanged. Repository-derived metadata supplements the otherwise incomplete master metadata row for `S007` (DeepMed) from the peer-reviewed ACL 2026 record.
