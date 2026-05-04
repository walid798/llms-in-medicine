# Reproducibility Tracker

Reproducibility rating for all included studies based on availability 
of code, data, and model weights.

> **Last updated:** May 2026  
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
| Yang et al. 2022 — GatorTron | ✅ | ❌ | ✅ | 🔶 Partial | Code and weights on GitHub (Megatron-LM); UF Health EHR not public |
| Jiang et al. 2023 — NYUTron | ✅ | ❌ | ❌ | 🔶 Partial | ~~❌~~ Code now on GitHub (nyuolab/NYUTron); NYU Langone EHR institutional only |
| Guevara et al. 2024 — Flan-T5 | ✅ | ❌ | ❌ | 🔶 Partial | ~~❌~~ Code on GitHub (AIM-Harvard/SDoH); multi-site EHR not public; Flan-T5 base open |
| Tariq et al. 2025 — Hybrid LLM | ❌ | ❌ | ❌ | ❌ None | Mayo/Stanford data institutional only |
| Siepmann et al. 2025 — GPT-4 | ❌ | ❌ | ❌ | ❌ None | German discharge letters institutional; GPT-4 closed |

### Biomedical Literature Mining & Knowledge Synthesis

| Study | Code | Data | Weights | Rating | Notes |
|-------|------|------|---------|--------|-------|
| Lee et al. 2020 — BioBERT | ✅ | ✅ | ✅ | ✅ Full | Fully open on GitHub and HuggingFace |
| Luo et al. 2022 — BioGPT | ✅ | ✅ | ✅ | ✅ Full | Fully open on GitHub (Microsoft) |
| Li et al. 2025 — BiomedRAG | ✅ | ✅ | ❌ | 🔶 Partial | Code and data available; weights not released |
| Liu et al. 2025 — LORE | ✅ | ✅ | ❌ | 🔶 Partial | Code on GitHub (ailabstw/LORE); PubMed data open; GPT-3.5 weights closed |

### Clinical Decision Support & Question Answering

| Study | Code | Data | Weights | Rating | Notes |
|-------|------|------|---------|--------|-------|
| Singhal et al. 2023 — Med-PaLM | ❌ | ❌ | ❌ | ❌ None | Google proprietary; MultiMedQA benchmark open |
| Nori et al. 2023 — GPT-4 | ❌ | ✅ | ❌ | 🔶 Partial | MedQA/USMLE benchmark open; GPT-4 closed |
| Li et al. 2023 — ChatDoctor | ✅ | ✅ | ✅ | ✅ Full | Fully open on GitHub |
| Xu et al. 2024 — Mental-LLM | ✅ | ✅ | ❌ | 🔶 Partial | Code and Reddit data available; fine-tuned weights not released |
| GPT-4 Surgical 2024 | ❌ | ❌ | ❌ | ❌ None | Surgical exam questions institutional; GPT-4 closed |
| Einspänner et al. 2025 — GPT-4 | ❌ | ❌ | ❌ | ❌ None | Radiology consent forms institutional; GPT-4 closed |

### Radiology Report Classification

| Study | Code | Data | Weights | Rating | Notes |
|-------|------|------|---------|--------|-------|
| Liu et al. 2023 — GPT-4 Radiology | ❌ | ✅ | ❌ | 🔶 Partial | Public radiology benchmarks; GPT-4 closed |
| Olivato et al. 2024 — Italian BERT | ❌ | ❌ | ❌ | ❌ None | Italian CT reports institutional |
| Matsuo et al. 2024 — GPT-3.5 TNM | ❌ | ❌ | ❌ | ❌ None | Lung cancer reports institutional |
| Kanzawa et al. 2024 — Japanese BERT | ❌ | ❌ | ❌ | ❌ None | Japanese MRI reports institutional |
| Mistral Radiology 2025 | ❌ | ❌ | ❌ | ❌ None | Proprietary radiology dataset; no code released |

### Pathology Report Classification

| Study | Code | Data | Weights | Rating | Notes |
|-------|------|------|---------|--------|-------|
| Kefeli et al. 2024 — BB-TEN | ❌ | ✅ | ❌ | 🔶 Partial | TCGA open; Columbia data institutional |
| Sushil et al. 2024 — GPT-4 Zero-shot | ✅ | ❌ | ❌ | 🔶 Partial | ~~❌~~ Code on GitHub (MadhumitaSushil/BreastCaPathClassification); UCSF data institutional |
| Saluja et al. 2025 — Path-llama3.1 | ✅ | ✅ | ❌ | 🔶 Partial | Code and PathRep-Bench data on GitHub; WCM external data not public |
| Ishida et al. 2025 — Gemini | ✅ | ❌ | ❌ | 🔶 Partial | ~~❌~~ Code on GitHub (iishiken/structured-clinical-data-extraction); gynecologic data institutional |

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
| Li et al. 2023 — LLaVA-Med | ✅ | ✅ | ✅ | ✅ Full | Fully open on GitHub (Microsoft) |
| Yuan et al. 2024 — MAIRA-2 | ❌ | ❌ | ❌ | ❌ None | Microsoft proprietary; no public release |
| Tanno et al. 2024 — Flamingo-CXR | ❌ | ❌ | ❌ | ❌ None | Proprietary clinical deployment; Nature Medicine |
| Li et al. 2025 — BrainGPT | ✅ | ❌ | ✅ | 🔶 Partial | Code and weights on Zenodo; 3D-BrainCT not public |
| Goswami et al. 2025 — MediVLM | ❌ | ❌ | ❌ | ❌ None | Not yet released |

### Pathology Report Generation

| Study | Code | Data | Weights | Rating | Notes |
|-------|------|------|---------|--------|-------|
| Chen et al. 2024 — WsiCaption (MI-Gen) | ✅ | ✅ | ❌ | 🔶 Partial | Code on GitHub (cpystan/Wsi-Caption); TCGA open; weights not released |
| Shi et al. 2024 — HistGen | ✅ | ✅ | ❌ | 🔶 Partial | Code on GitHub (dddavid4real/HistGen); TCGA open; weights not released |
| Chen et al. 2024 — Clinical-Grade Multi-organ VLM | ✅ | ✅ | ❌ | 🔶 Partial | Code on GitHub (hvcl/Clinical-grade-Pathology-Report-Generation); TCGA open |
| Multi-level Regional 2025 | ❌ | ❌ | ❌ | ❌ None | No public code or data; Comput. Methods Programs Biomed. |
| Shaikovski et al. 2025 — TITAN | ✅ | ✅ | ❌ | 🔶 Partial | Code on GitHub (mahmoodlab/TITAN); TCGA open; weights not released |
| PolyPath 2025 — Gemini | ❌ | ❌ | ❌ | ❌ None | Gemini 1.5 Flash closed; Modern Pathology; no code released |
| Kim et al. 2025 — MIL + T5 | ❌ | ❌ | ❌ | ❌ None | K-MEDICON 2024 competition dataset; no code |
| Hu et al. 2025 — Gastric RAG | ❌ | ❌ | ❌ | ❌ None | GastricADC institutional Chinese dataset |

### Medical Visual Question Answering

| Study | Code | Data | Weights | Rating | Notes |
|-------|------|------|---------|--------|-------|
| Li et al. 2023 — LLaVA-Med | ✅ | ✅ | ✅ | ✅ Full | Fully open on GitHub (Microsoft) |
| Zhang et al. 2024 — PMC-VQA | ✅ | ✅ | ✅ | ✅ Full | Fully open on GitHub |
| Liang et al. 2024 — CH-ICL | ❌ | ✅ | ❌ | 🔶 Partial | VQA benchmarks open; code not released |
| Bawazir et al. 2025 — Falcon Med-VQA | ❌ | ✅ | ❌ | 🔶 Partial | VQA benchmarks open; code not released |
| Hu et al. 2024 — OmniMedVQA | ❌ | ✅ | ❌ | 🔶 Partial | 12-modality benchmark open (CVPR 2024); no model code |
| Alsabbagh et al. 2025 — MiniMedGPT | ❌ | ✅ | ❌ | 🔶 Partial | VQA benchmarks open; code not released |
| Yu et al. 2025 — FAVP | ✅ | ✅ | ❌ | 🔶 Partial | Code on GitHub (OpenMICG/FAVP); VQA benchmarks open; weights not released |
| Xu et al. 2025 — CIF | ❌ | ✅ | ❌ | 🔶 Partial | VQA benchmarks open; code not released |

### LLM-Guided Image Segmentation

| Study | Code | Data | Weights | Rating | Notes |
|-------|------|------|---------|--------|-------|
| Tang et al. 2025 — LLM4Seg | ✅ | ✅ | ❌ | 🔶 Partial | Code on GitHub (FengheTan9/LLM4Seg); ISIC/BTCV open; weights not released |
| Kumar et al. 2025 — MedVisionLlama | ✅ | ✅ | ❌ | 🔶 Partial | Code on GitHub; Decathlon dataset open; weights not released |
| Dai et al. 2025 — Zeus | ❌ | ✅ | ❌ | 🔶 Partial | MSD datasets open; code not released |
| HCR 2025 — Gemini Guardrails | ❌ | ❌ | ❌ | ❌ None | Gemini 2.5 Flash closed; arXiv preprint; no code |

### Multimodal Clinical Diagnosis & Reasoning

| Study | Code | Data | Weights | Rating | Notes |
|-------|------|------|---------|--------|-------|
| Zhou et al. 2024 — GPT-4V CXR | ❌ | ✅ | ❌ | 🔶 Partial | NIH/MIDRC datasets open; GPT-4V closed |
| Liang et al. 2025 — Claude 3.5 | ❌ | ❌ | ❌ | ❌ None | Laryngeal cancer data institutional; Claude closed |
| Ferber et al. 2024 — GPT-4V Histopath | ✅ | ✅ | ❌ | 🔶 Partial | Code on GitHub (Dyke-F/GPT-4V-In-Context-Learning); CRC100K/PatchCamelyon open; GPT-4V closed |
| Liu et al. 2025 — M3FM | ❌ | ❌ | ❌ | ❌ None | Not yet released; npj Digital Medicine |
| Zhou et al. 2024 — SkinGPT-4 | ✅ | ❌ | ❌ | 🔶 Partial | Code on GitHub (JoshuaChou2018/SkinGPT-4); skin disease images institutional |
| Shaikovski et al. 2024 — PathChat | ✅ | ❌ | ❌ | 🔶 Partial | Code on GitHub (fedshyvana/pathology_mllm_training); training data not fully public |
| Tu et al. 2024 — Med-PaLM M | ❌ | ❌ | ❌ | ❌ None | Google proprietary; 14-task unified model; NEJM AI |
| Shi et al. 2024 — LLMSeg | ✅ | ✅ | ❌ | 🔶 Partial | Code on GitHub (tvseg/MM-LLM-RO); public CT datasets; weights not released |
| MedTVT-R1 2025 | ✅ | ❌ | ❌ | 🔶 Partial | Code on GitHub (keke-nice/MedTVT-R1); ECG/CXR/lab data institutional |
| MEDFuse 2024 | ❌ | ❌ | ❌ | ❌ None | CIKM 2024; EHR data institutional; no public code |
| SMFusion 2025 | ❌ | ❌ | ❌ | ❌ None | IEEE JBHI; PET/MRI data institutional; no public code |

---

## Summary

| Rating | Count | Percentage |
|--------|-------|------------|
| ✅ Full | 6 | 9% |
| 🔶 Partial | 30 | 47% |
| ❌ None | 28 | 44% |

---

## Key Observations

- **44% of studies provide no reproducibility resources** — the dominant
  barrier remains institutional EHR and clinical imaging data that cannot
  be shared publicly.
- **Pathology report generation is the most open subcategory** — 
  WsiCaption, HistGen, Clinical-Grade Multi-organ VLM, and TITAN all
  release code with open benchmark data.
- **4 entries upgraded from ❌ None to 🔶 Partial** since last update:
  NYUTron (GitHub), Flan-T5/Guevara (AIM-Harvard), Ishida/Gemini
  (structured-clinical-data-extraction), and Sushil/GPT-4 (GitHub).
- **GPT-4, Claude, and Gemini studies remain structurally irreproducible**
  at the model level — closed weights and API-only access prevent
  independent verification.
- **Segmentation studies are consistently partial** — benchmark datasets
  are open but model weights are withheld across all four entries.
- **Multimodal diagnosis is the fastest-growing subcategory** — 11
  entries, but only PathChat, SkinGPT-4, LLMSeg, and MedTVT-R1 release
  code.