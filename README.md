# 🏥 LLMs in Clinical Medicine

A curated evidence repository accompanying the systematic review:

> **A Systematic Review of LLMs in Clinical Medicine Across Multimodal Architectures, Benchmarks, and Personalized Healthcare**
>
> Walid Mohamed, Mohamed Elsharkawy, Shahad Al Hamadani, Rafia Fayyaz, Usama Mousattat, Taysir Hassan A. Soliman, Amr Mohamed Abdelaziz, Ali Mahmoud, Mohamed Ghazal, Tania Tahtouh, Ayman El-Baz

This revision expands the repository from the earlier 56-study version to a **frozen corpus of 145 included studies (2022–2026)** and aligns the public resources with the review's updated analytical framework: **model evolution, multimodal fusion, retrieval/reasoning/agents, patient-centric personalization, safety, and translational evidence**.

## 📊 Final corpus at a glance

| Item | Final coding |
|---|---:|
| Included studies | **145** |
| Fusion-active studies (F1–F5) | **72 (49.7%)** |
| Deep/decision/hybrid fusion (F3–F5) | **44 (30.3%)** |
| Explicit RAG | **34 (23.4%)** |
| Agent/tool use | **33 (22.8%)** |
| Agentic reasoning | **26 (17.9%)** |
| Any patient-specific capability (P1–P5) | **73 (50.3%)** |
| Advanced personalization (P3–P5) | **42 (29.0%)** |
| Prospective/workflow/outcome evidence (T3–T5) | **19 (13.1%)** |

### Temporal evolution

| Year | Studies | Generative LLMs | Multimodal LLMs | Reasoning / agentic systems |
|---:|---:|---:|---:|---:|
| 2022 | 3 | 3 | 0 | 0 |
| 2023 | 6 | 4 | 2 | 0 |
| 2024 | 25 | 8 | 14 | 3 |
| 2025 | 58 | 26 | 18 | 14 |
| 2026 | 53 | 14 | 14 | 25 |

The three primary-paradigm columns are mutually exclusive **for temporal visualization only**. The detailed coding remains multi-dimensional.

## 🧭 Updated evidence architecture

The repository now mirrors the review's central questions rather than the older task-only organization:

1. **Model evolution and adaptation**
2. **Multimodal fusion (F0–F5)**
3. **Retrieval, reasoning, and clinical agents**
4. **Patient-centric personalization and longitudinal intelligence (P0–P5)**
5. **Safety and trustworthy AI**
6. **Clinical translation (T0–T5)**

## 📁 Repository structure

```text
.
├── README.md
├── CITATION.cff
├── CHANGELOG.md
├── CONTRIBUTING.md
├── FAQ.md
├── data/
│   ├── Final_145_Studies_FROZEN.xlsm
│   ├── studies.csv
│   ├── studies.jsonl
│   ├── architecture_fusion.csv
│   ├── performance.csv
│   ├── personalization_safety.csv
│   ├── codebook.csv
│   └── review_metadata.json
├── models/
│   ├── foundation-models.md
│   └── medical-llms.md
└── papers/
    ├── studies.md
    ├── multimodal.md
    ├── retrieval-reasoning-agents.md
    ├── personalization.md
    ├── safety-translation.md
    └── datasets.md
```

## 📚 Study register

- [`papers/studies.md`](papers/studies.md) — human-readable register.
- [`data/studies.csv`](data/studies.csv) — machine-readable register.
- [`data/studies.jsonl`](data/studies.jsonl) — JSONL export.
- [`data/Final_145_Studies_FROZEN.xlsm`](data/Final_145_Studies_FROZEN.xlsm) — frozen evidence matrix.

The final primary corpus contains original empirical studies in which a **generative LLM, medical LLM, MLLM, or LLM-centered retrieval/reasoning/tool-use/agentic framework** is a substantive evaluated component. Standalone encoder-only PLMs and conventional multimodal systems without a substantive generative LLM component are contextual rather than part of the primary quantitative corpus.

## 🔀 Multimodal fusion
See [`papers/multimodal.md`](papers/multimodal.md).

## 🔎 Retrieval, reasoning, and clinical agents
See [`papers/retrieval-reasoning-agents.md`](papers/retrieval-reasoning-agents.md).

## 👤 Personalization and longitudinal intelligence
See [`papers/personalization.md`](papers/personalization.md).

## 🛡️ Safety and translational evidence
See [`papers/safety-translation.md`](papers/safety-translation.md).

## 📦 Datasets and resources
See [`papers/datasets.md`](papers/datasets.md).

## 🤝 Contributing
Please read [`CONTRIBUTING.md`](CONTRIBUTING.md). New candidate studies should not be inserted directly into the frozen S001–S145 register.

## 📖 Citation

```bibtex
@article{mohamed2026clinical_llm_systematic_review,
  title={A Systematic Review of LLMs in Clinical Medicine Across Multimodal Architectures, Benchmarks, and Personalized Healthcare},
  author={Walid Mohamed and Mohamed Elsharkawy and Shahad Al Hamadani and Rafia Fayyaz and Usama Mousattat and Taysir Hassan A. Soliman and Amr Mohamed Abdelaziz and Ali Mahmoud and Mohamed Ghazal and Tania Tahtouh and Ayman El-Baz},
  year={2026},
  note={Systematic review manuscript}
}
```

## 🔗 Repository
https://github.com/walid798/llms-in-medicine
