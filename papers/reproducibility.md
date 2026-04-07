# Reproducibility Tracker

Reproducibility rating for all 47 included studies based on 
availability of code, data, and model weights.

> **Last updated:** April 2025  
> **Note:** Update this file when new papers are added to the corpus.

---

## Rating Scale

| Rating | Meaning |
|--------|---------|
| ✅ Full | Code + data + model weights all publicly available |
| 🔶 Partial | Code only, or data only, or weights only |
| ❌ None | No code, data, or weights publicly available |

---

## Text-Based Applications

### Clinical Documentation & Information Extraction

| Study | Code | Data | Weights | Rating | Notes |
|-------|------|------|---------|--------|-------|
| Yang et al. 2022 — GatorTron | ✅ | ❌ | ✅ | 🔶 Partial | Code and weights on GitHub; UF Health EHR not public |
| Jiang et al. 2023 — NYUTron | ❌ | ❌ | ❌ | ❌ None | NYU Langone EHR institutional only |
| Tariq et al. 2025 — Hybrid LLM | ❌ | ❌ | ❌ | ❌ None | Mayo/Stanford data institutional only |
| Guevara et al. 2024 — Flan-T5 | ❌ | ❌ | ❌ | ❌ None | Multi-site EHR not public; Flan-T5 base model open |
| Siepmann et al. 2025 — GPT-4 | ❌ | ❌ | ❌ | ❌ None | German discharge letters institutional; GPT-4 closed |

### Biomedical Literature Mining & Knowledge Synthesis

| Study | Code | Data | Weights | Rating | Notes |
|-------|------|------|---------|--------|-------|
| Lee et al. 2020 — BioBERT | ✅ | ✅ | ✅ | ✅ Full | Fully open on GitHub and HuggingFace |
| Luo et al. 2022 — BioGPT | ✅ | ✅ | ✅ | ✅ Full | Fully open on GitHub (Microsoft) |
| Li et al. 2025 — BiomedRAG | ✅ | ✅ | ❌ | 🔶 Partial | Code and data available; weights not released |

### Clinical Decision Support & Question Answering

| Study | Code | Data | Weights | Rating | Notes |
|-------|------|------|---------|--------|-------|
| Singhal et al. 2023 — Med-PaLM | ❌ | ❌ | ❌ | ❌ None | Google proprietary; MultiMedQA benchmark open |
| Nori et al. 2023 — GPT-4 | ❌ | ✅ | ❌ | 🔶 Partial | MedQA/USMLE benchmark open; GPT-4 closed |
| Li et al. 2023 — ChatDoctor | ✅ | ✅ | ✅ | ✅ Full | Fully open on GitHub |
| Xu et al. 2024 — Mental-LLM | ✅ | ✅ | ❌ | 🔶 Partial | Code and Reddit data available; fine-tuned weights not released |
| Einspänner et al. 2025 — GPT-4 | ❌ | ❌ | ❌ | ❌ None | Radiology consent forms institutional; GPT-4 closed |

### Report Classification — Radiology

| Study | Code | Data | Weights | Rating | Notes |
|-------|------|------|---------|--------|-------|
| Liu et al. 2023 — GPT-4 Radiology | ❌ | ✅ | ❌ | 🔶 Partial | Public radiology benchmarks; GPT-4 closed |
| Olivato et al. 2024 — Italian BERT | ❌ | ❌ | ❌ | ❌ None | Italian CT reports institutional |
| Matsuo et al. 2024 — GPT-3.5 TNM | ❌ | ❌ | ❌ | ❌ None | Lung cancer reports institutional |
| Kanzawa et al. 2024 — Japanese BERT | ❌ | ❌ | ❌ | ❌ None | Japanese MRI reports institutional |

### Report Classification — Pathology

| Study | Code | Data | Weights | Rating | Notes |
|-------|------|------|---------|--------|-------|
| Kefeli et al. 2024 — BB-TEN | ❌ | ✅ | ❌ | 🔶 Partial | TCGA open; Columbia data institutional |
| Sushil et al. 2024 — GPT-4 Zero-shot | ❌ | ❌ | ❌ | ❌ None | UCSF pathology data institutional |
| Saluja et al. 2025 — Path-llama3.1 | ❌ | ✅ | ❌ | 🔶 Partial | TCGA open; WCM external data not public |
| Ishida et al. 2025 — Gemini | ❌ | ❌ | ❌ | ❌ None | Gynecologic oncology reports institutional |

### Clinical Text Summarization

| Study | Code | Data | Weights | Rating | Notes |
|-------|------|------|---------|--------|-------|
| Fink et al. 2023 — GPT-4 | ❌ | ❌ | ❌ | ❌ None | Lung cancer CT reports institutional |
| Chua et al. 2024 — Domain LLM | ❌ | ❌ | ❌ | ❌ None | Progress notes institutional |
| Barabadi et al. 2024 — PEFT LLM | ❌ | ❌ | ❌ | ❌ None | MSKCC radiology reports institutional |
| Williams et al. 2025 — GPT-4 | ❌ | ❌ | ❌ | ❌ None | Discharge summaries institutional |

---

## Multimodal Applications

### Radiology Report Generation

| Study | Code | Data | Weights | Rating | Notes |
|-------|------|------|---------|--------|-------|
| Wang et al. 2023 — R2GenGPT | ✅ | ✅ | ✅ | ✅ Full | Fully open on GitHub; MIMIC-CXR credentialed |
| Tanno et al. 2024 — Flamingo-CXR | ❌ | ❌ | ❌ | ❌ None | Proprietary clinical deployment |
| Li et al. 2025 — BrainGPT | ✅ | ❌ | ✅ | 🔶 Partial | Code and weights on Zenodo; 3D-BrainCT not public |
| Goswami et al. 2025 — MediVLM | ❌ | ❌ | ❌ | ❌ None | Not yet released |

### Pathology Report Generation

| Study | Code | Data | Weights | Rating | Notes |
|-------|------|------|---------|--------|-------|
| Chen et al. 2024 — MI-Gen | ❌ | ✅ | ❌ | 🔶 Partial | TCGA open; code not released |
| Hu et al. 2025 — Gastric RAG | ❌ | ❌ | ❌ | ❌ None | GastricADC institutional Chinese dataset |
| Kim et al. 2025 — MIL + T5 | ❌ | ❌ | ❌ | ❌ None | K-MEDICON 2024 competition dataset |

### Medical Visual Question Answering

| Study | Code | Data | Weights | Rating | Notes |
|-------|------|------|---------|--------|-------|
| Li et al. 2023 — LLaVA-Med | ✅ | ✅ | ✅ | ✅ Full | Fully open on GitHub (Microsoft) |
| Zhang et al. 2024 — PMC-VQA | ✅ | ✅ | ✅ | ✅ Full | Fully open on GitHub |
| Liang et al. 2024 — CH-ICL | ❌ | ✅ | ❌ | 🔶 Partial | VQA benchmarks open; code not released |
| Bawazir et al. 2025 — Falcon | ❌ | ✅ | ❌ | 🔶 Partial | VQA benchmarks open; code not released |
| Alsabbagh et al. 2025 — MiniMedGPT | ❌ | ✅ | ❌ | 🔶 Partial | VQA benchmarks open; code not released |
| Yu et al. 2025 — FAVP | ✅ | ✅ | ❌ | 🔶 Partial | Code on GitHub; weights not released |
| Xu et al. 2025 — CIF | ❌ | ✅ | ❌ | 🔶 Partial | VQA benchmarks open; code not released |

### LLM-Guided Segmentation

| Study | Code | Data | Weights | Rating | Notes |
|-------|------|------|---------|--------|-------|
| Tang et al. 2025 — LLM4Seg | ✅ | ✅ | ❌ | 🔶 Partial | Code available; ISIC/BTCV open; weights not released |
| Kumar et al. 2025 — MedVisionLlama | ❌ | ✅ | ❌ | 🔶 Partial | Decathlon dataset open; code not released |
| Dai et al. 2025 — Zeus | ❌ | ✅ | ❌ | 🔶 Partial | MSD datasets open; code not released |

### Multimodal Diagnosis & Clinical Reasoning

| Study | Code | Data | Weights | Rating | Notes |
|-------|------|------|---------|--------|-------|
| Liu et al. 2025 — M3FM | ❌ | ❌ | ❌ | ❌ None | Not yet released |
| Zhou et al. 2024 — GPT-4V CXR | ❌ | ✅ | ❌ | 🔶 Partial | NIH/MIDRC datasets open; GPT-4V closed |
| Liang et al. 2025 — Claude 3.5 | ❌ | ❌ | ❌ | ❌ None | Laryngeal cancer data institutional |
| Ferber et al. 2024 — GPT-4V Histopath | ❌ | ✅ | ❌ | 🔶 Partial | CRC100K/PatchCamelyon open; GPT-4V closed |
| Zhou et al. 2024 — SkinGPT-4 | ✅ | ❌ | ❌ | 🔶 Partial | Code on GitHub; skin disease images institutional |

---

## Summary

| Rating | Count | Percentage |
|--------|-------|------------|
| ✅ Full | 5 | 11% |
| 🔶 Partial | 18 | 38% |
| ❌ None | 24 | 51% |

---

## Key Observations

- **51% of studies provide no reproducibility resources** — 
  the dominant barrier is institutional EHR and clinical 
  image data that cannot be shared publicly.
- **Fully open studies cluster in biomedical NLP** — 
  BioBERT, BioGPT, ChatDoctor, LLaVA-Med, PMC-VQA, and 
  R2GenGPT all provide complete reproducibility.
- **GPT-4 and Claude studies are structurally irreproducible** — 
  closed model weights and API-only access mean results 
  cannot be independently verified at the model level.
- **Segmentation studies are partially reproducible** — 
  benchmark datasets are open but code and weights are 
  consistently withheld.

---

<!-- ## How to Update

When adding a new paper to the survey:

1. Add a row to the appropriate table above
2. Check the paper's GitHub, HuggingFace, and supplementary 
   materials for code, data, and weights
3. Assign a rating based on the scale above
4. Update the Summary counts at the bottom
5. Commit with message: `Update reproducibility: add [Author Year]` -->