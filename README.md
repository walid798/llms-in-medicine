# 🏥 LLMs in Medicine

[![Maintained](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/walid798/llms-in-medicine)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Stars](https://img.shields.io/github/stars/walid798/llms-in-medicine?style=social)](https://github.com/walid798/llms-in-medicine)
[![Papers](https://img.shields.io/badge/Papers-47-blue)](README.md)  <!-- Need to be updated after adding extra papers -->
[![Categories](https://img.shields.io/badge/Categories-9-green)](README.md)
[![Updated](https://img.shields.io/badge/Updated-April%202025-orange)](CHANGELOG.md)

**A curated repository accompanying our systematic survey:**

> **Large Language Models in Clinical Medicine — A Systematic Review of
> Multimodal Architectures, Benchmarks, and Personalized Healthcare Applications**
>
> Walid Mohamed · Rafia Fayyaz · Usama Mousattat · Shahad Al Hamadani ·
> Taysir Soliman · Amr Mohamed Abdelaziz · Mohamed Elsharkawy ·
> Ali Mahmoud · Mohamed Ghazal

## If you find this repository useful, please consider giving it a ⭐

---

## 📋 Table of Contents

- [What's New](#-whats-new)
- [Survey Overview](#-survey-overview)
- [Foundation Models](models/foundation-models.md) 🧱
- [Medical LLM Models](models/medical-llms.md) 🏥
- [Text-Based Applications](#-text-based-applications)
- [Multimodal Applications](#-multimodal-applications)
- [Benchmark Leaderboard](#-benchmark-leaderboard)
- [Datasets and Resources](#-datasets-and-resources)
- [Related Surveys](#-related-surveys)
- [How to Contribute](#-how-to-contribute)
- [Citation](#-citation)

---

## 🆕 What's New

| Date | Update |
|------|--------|
| 2025-04 | 🎉 Repository launched alongside survey submission to AI Review (Springer) |
| 2026-03 | 47 studies added across 9 task categories |
| 2026-01 | Benchmark leaderboard added for MedQA, VQA-RAD, and SLAKE |

---

## 📊 Survey Overview

This repository accompanies a **PRISMA 2020-compliant systematic review**
synthesizing **47 studies** on LLMs in clinical medicine, organized around
**personalized healthcare** as a central analytical framework.

### Coverage at a Glance

| Section | Task Category | Studies |
|---------|---------------|---------|
| IV-A | Clinical Documentation & IE | 5 |
| IV-B | Literature Mining & Knowledge | 3 |
| IV-C | Decision Support & QA | 5 |
| IV-D | Report Classification | 8 |
| IV-E | Clinical Text Summarization | 4 |
| V-A | Radiology Report Generation | 4 |
| V-B | Pathology Report Generation | 3 |
| V-C | Medical Visual QA | 6 |
| V-D | LLM-Guided Segmentation | 3 |
| V-E | Multimodal Diagnosis | 5 |
| | **Total** | **47** |

<!-- ### Publication Trend -->

---

[Foundation Models](models/foundation-models.md) — 24 general-purpose models from Transformer (2017) to Llama 4 (2025)  
[Medical LLM Models](models/medical-llms.md) — 42 domain-adapted models across text, biomedical, and multimodal categories

## 📄 Paper Categories

### Legend

| Badge | Meaning |
|-------|---------|
| ![Code](https://img.shields.io/badge/Code-Available-blue) | Public code repository available |
| ![Open](https://img.shields.io/badge/Data-Open-green) | Open access dataset used |
| ![SOTA](https://img.shields.io/badge/-SOTA-red) | State-of-the-art at publication time |
| ![Prospective](https://img.shields.io/badge/Val-Prospective-purple) | Prospective clinical validation |
| ![External](https://img.shields.io/badge/Val-External-orange) | External multi-site validation |

---

### 📝 Text-Based Applications

#### Clinical Documentation & Information Extraction

| Year | Title | Model | Venue | Links |
|------|-------|-------|-------|-------|
| 2022 | **A Large Clinical Language Model to Unlock Patient Information from Unstructured EHRs** | GatorTron (8.9B) | *npj Digital Medicine* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://www.nature.com/articles/s41746-022-00742-2) [![Code](https://img.shields.io/badge/Code-Available-blue)](https://github.com/NVIDIA/Megatron-LM) |
| 2023 | **Health system-scale language models are all-purpose prediction engines** | NYUTron | *Nature* |  [![Paper](https://img.shields.io/badge/Paper-blue)](https://www.nature.com/articles/s41586-023-06160-y) [![Code](https://img.shields.io/badge/Code-Available-blue)](https://github.com/nyuolab/NYUTron) ![Prospective](https://img.shields.io/badge/Val-Prospective-purple) | Prospective clinical validation |
| 2024 | **Large language models to identify social determinants of health in electronic health records** | Flan-T5 XL/XXL | *npj Digital Medicine* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://www.nature.com/articles/s41746-023-00970-0) [![Code](https://img.shields.io/badge/Code-Available-blue)](https://github.com/AIM-Harvard/SDoH) ![External](https://img.shields.io/badge/Val-External-orange) |
| 2025 | **Open-Source Hybrid Large Language Model Integrated System for Extraction of Breast Cancer Treatment Pathway From Free-Text Clinical Notes** | Hybrid LLM (UMLS) | *J. Biomedical Informatics* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://ascopubs.org/doi/full/10.1200/CCI-25-00002) ![External](https://img.shields.io/badge/Val-External-orange) |
| 2025 | **An automated information extraction model for unstructured discharge letters using large language models and GPT-4** | GPT-4 | *Healthcare Analytics* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://www.sciencedirect.com/science/article/pii/S2772442524000807) |


---

#### Biomedical Literature Mining & Knowledge Synthesis

| Year | Title | Model | Venue | Links |
|------|-------|-------|-------|-------| 
| 2020 | **BioBERT: a pre-trained biomedical language representation model for biomedical text mining** | BioBERT | *Bioinformatics* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://academic.oup.com/bioinformatics/article/36/4/1234/5566506) [![Code](https://img.shields.io/badge/Code-Available-blue)](https://github.com/dmis-lab/biobert) |
| 2022 | **BioGPT: generative pre-trained transformer for biomedical text generation and mining** | BioGPT | *Briefings in Bioinformatics* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://academic.oup.com/bib/article/23/6/bbac409/6713511?guestAccessKey=) [![Code](https://img.shields.io/badge/Code-Available-blue)](https://github.com/microsoft/BioGPT) |
| 2025 | **BiomedRAG: A retrieval augmented large language model for biomedicine** | BiomedRAG (LLaMA2 / MedLLaMA-13B) | *Journal of Biomedical Informatics* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://www.sciencedirect.com/science/article/pii/S1532046424001874) [![Code](https://img.shields.io/badge/Code-Available-blue)](https://github.com/ToneLi/BIoMedRAG/tree/main) |
| 2025 | **A large language model framework for literature-based disease–gene association prediction** | LORE (GPT-3.5-turbo + text-embedding-3-large) | *Briefings in Bioinformatics* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://doi.org/10.1093/bib/bbaf070) [![Code](https://img.shields.io/badge/Code-Available-blue)](https://github.com/ailabstw/LORE) |
---

#### Clinical Decision Support & Question Answering

| Year | Title | Model | Venue | Links |
|------|-------|-------|-------|-------|
| 2023 | **Large language models encode clinical knowledge** | Med-PaLM (Flan-PaLM) | *Nature* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://www.nature.com/articles/s41586-023-06291-2) |
| 2023 | **ChatDoctor: A Medical Chat Model Fine-Tuned ona Large Language Model Meta-AI (LLaMA) UsingMedical Domain Knowledge** | ChatDoctor (LLaMA-7B) | *Cureus* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://assets.cureus.com/uploads/original_article/pdf/152858/20230724-24731-1v47a9.pdf) [![Code](https://img.shields.io/badge/Code-Available-blue)](https://github.com/Kent0n-Li/ChatDoctor) |
| 2024 | **Evaluating capabilities of large language models: Performance of GPT-4 on surgical knowledge assessments** | GPT-4 | *Surgery* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://www.sciencedirect.com/science/article/pii/S0039606023009546) |
| 2024 | **Mental-LLM: Leveraging Large Language Models for Mental Health Prediction via Online Text Data** | Mental-LLM | *ACM SIGCHI* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://dl.acm.org/doi/pdf/10.1145/3643540) [![Code](https://img.shields.io/badge/Code-Available-blue)](https://github.com/neuhai/Mental-LLM) |https://github.com/neuhai/Mental-LLM



---

#### Radiology Reports Classification

| Year | Title | Model | Venue | Links |
|------|-------|-------|-------|-------|
| 2023 | **Exploring the Boundaries of GPT-4 in Radiology** | GPT-4 | *EMNLP* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://aclanthology.org/2023.emnlp-main.891/) ![SOTA](https://img.shields.io/badge/-SOTA-red) | State-of-the-art at publication time |
| 2024 | **Language Models for Hierarchical Classification of Radiology Reports With Attention Mechanisms, BERT, and GPT-4** | Italian BERT / GPT-4 | *IEEE Access* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://ieeexplore.ieee.org/abstract/document/10531266) |
| 2024 | **Exploring Multilingual Large Language Models for Enhanced TNM Classification of Radiology Report in Lung Cancer Staging** | GPT-3.5-turbo | *Cancers* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://www.mdpi.com/2072-6694/16/21/3621) |
| 2024 | **Automated classification of brain MRI reports using fine-tuned large language models** | BERT | *Neuroradiology* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://link.springer.com/article/10.1007/s00234-024-03427-7) |
| 2025 | **Mistral in Radiology: AI-Powered Classification of Normal and Abnormal Reports** | Mistral  | *IMA* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://onlinelibrary.wiley.com/doi/abs/10.1002/ima.70251) |


#### Pathology Reports Classification 

| Year | Title | Model | Venue | Links |
|------|-------|-------|-------|-------|
| 2025 | **Cancer type, stage and prognosis assessment from pathology reports using LLMs** | Path-llama3.1-8B and Path-GPT-4o-mini-FT | *Scientific Reports* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://www.nature.com/articles/s41598-025-10709-4)  [![Code](https://img.shields.io/badge/Code-Available-blue)](https://github.com/rachitsaluja/PathRep-Bench) |
| 2025 | **Real-world application of large language models for automated TNM staging using unstructured gynecologic oncology reports** | Gemini 1.5, Qwen2.5 72B | *npj precision oncology* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://www.nature.com/articles/s41698-025-01157-4)  | [![Code](https://img.shields.io/badge/Code-Available-blue)](https://github.com/iishiken/structured-clinical-data-extraction)
| 2024 | **Generalizable and automated classification of TNM stage from pathology reports with external validation** | Path-llama3.1 | *Nature Communications* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://www.nature.com/articles/s41467-024-53190-9) |
| 2025 | **A comparative study of large language model-based zero-shot inference and task-specific supervised classification of breast cancer pathology reports** | GPT-4, GPT-3.5, Starling, and ClinicalCamel | *JAMIA* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://academic.oup.com/jamia/article/31/10/2315/7696538) [![Code](https://img.shields.io/badge/Code-Available-blue)](https://github.com/MadhumitaSushil/BreastCaPathClassification)|


---

#### Clinical Text Summarization

| Year | Title | Model | Venue | Links |
|------|-------|-------|-------|-------|
| 2023 | **GPT-4 for Lung Cancer Phenotype Extraction** | GPT-4 | *JAMIA* | [![Paper](https://img.shields.io/badge/Paper-blue)](#) |
| 2024 | **Integration of LLMs for Clinical Note Summarization** | Domain-adapted LLM | *npj Digital Medicine* | [![Paper](https://img.shields.io/badge/Paper-blue)](#) |
| 2024 | **PEFT for Patient History-Aware Radiology Summarization** | PEFT LLM | *Radiology* | [![Paper](https://img.shields.io/badge/Paper-blue)](#) |
| 2025 | **Physician-Quality Discharge Summary Generation** | GPT-4 | *NEJM AI* | [![Paper](https://img.shields.io/badge/Paper-blue)](#) |

---

### 🖼️ Multimodal Applications

#### Radiology Report Generation

| Year | Title | Model | Venue | Links |
|------|-------|-------|-------|-------|
| 2023 | **R2GenGPT: Radiology Report Generation with Frozen LLMs** | R2GenGPT | *Meta-Radiology* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://arxiv.org/abs/2309.09110) [![Code](https://img.shields.io/badge/Code-Available-blue)](https://github.com/wang-zhanyu/R2GenGPT) |
| 2024 | **Collaboration Between Clinicians and AI for Radiology Reports** | Flamingo-CXR | *NPJ Digital Medicine* | [![Paper](https://img.shields.io/badge/Paper-blue)](#) ![Prospective](https://img.shields.io/badge/Val-Prospective-purple) |
| 2025 | **BrainGPT: 3D Brain CT Report Generation** | BrainGPT (CVIT) | *Nature Communications* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://www.nature.com/articles/s41467-025-57426-0) [![Code](https://img.shields.io/badge/Code-Available-blue)](https://doi.org/10.5281/zenodo.14852686) |
| 2025 | **MediVLM: Annotation-free Severity-aware Radiology Reporting** | MediVLM | *arXiv* | [![Paper](https://img.shields.io/badge/Paper-blue)](#) |

---

#### Pathology Report Generation

| Year | Title | Model | Venue | Links |
|------|-------|-------|-------|-------|
| 2024 | **MI-Gen: Gigapixel WSI Report Generation** | MI-Gen | *Medical Image Analysis* | [![Paper](https://img.shields.io/badge/Paper-blue)](#) |
| 2025 | **RAG-based Gastric Pathology Report Generation** | Proposed method | *Computers in Biology and Medicine* | [![Paper](https://img.shields.io/badge/Paper-blue)](#) |
| 2025 | **Structured Label-Conditioned Bladder Pathology Reports** | MIL + T5 | *MICCAI 2025* | [![Paper](https://img.shields.io/badge/Paper-blue)](#) |

---

#### Medical Visual Question Answering

| Year | Title | Model | Venue | Links |
|------|-------|-------|-------|-------|
| 2023 | **LLaVA-Med: Training a Large Language-and-Vision Assistant for Biomedicine** | LLaVA-Med | *NeurIPS 2023* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://arxiv.org/abs/2306.00890) [![Code](https://img.shields.io/badge/Code-Available-blue)](https://github.com/microsoft/LLaVA-Med) ![SOTA](https://img.shields.io/badge/-SOTA-red) |
| 2024 | **PMC-VQA: Visual Instruction Tuning for Medical VQA** | PMC-VQA | *Communications Medicine* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://www.nature.com/articles/s43856-024-00709-2) [![Code](https://img.shields.io/badge/Code-Available-blue)](https://github.com/xiaoman-zhang/PMC-VQA) |
| 2024 | **Candidate Answer Set Guided Medical VQA** | CH-ICL | *arXiv* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://arxiv.org/abs/2408.10048) |
| 2024 | **Falcon Med-VQA: Uncertainty-aware Clinical QA** | Falcon Med-VQA | *arXiv* | [![Paper](https://img.shields.io/badge/Paper-blue)](#) |
| 2025 | **MiniMedGPT: Parameter-Efficient Medical VQA** | MiniMedGPT (EVA-CLIP + LLaMA2-7B) | *arXiv* | [![Paper](https://img.shields.io/badge/Paper-blue)](#) |
| 2025 | **FAVP: Fine-grained Adaptive Visual Prompts for Generative MedVQA** | FAVP (ViT-G/14 + Vicuna-7B) | *AAAI 2025* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://github.com/OpenMICG/FAVP) [![Code](https://img.shields.io/badge/Code-Available-blue)](https://github.com/OpenMICG/FAVP) |
| 2025 | **Structural Causal Models and LLMs for Medical VQA** | CIF (CLIP + LLaMA 7B/13B) | *IEEE Transactions* | [![Paper](https://img.shields.io/badge/Paper-blue)](#) |

---

#### LLM-Guided Image Segmentation

| Year | Title | Model | Venue | Links |
|------|-------|-------|-------|-------|
| 2025 | **LLM4Seg: Pre-trained LLM Layers for Medical Segmentation** | LLM4Seg (LLaMA3.2-1B / DeepSeek) | *arXiv* | [![Paper](https://img.shields.io/badge/Paper-blue)](#) [![Code](https://img.shields.io/badge/Code-Available-blue)](#) |
| 2025 | **MedVisionLlama: LLM-Enhanced ViT for 3D Segmentation** | MedVisionLlama (Llama-3.1-8B + ViT) | *arXiv* | [![Paper](https://img.shields.io/badge/Paper-blue)](#) |
| 2025 | **Zeus: Zero-shot LLM Instructions for SAM-based Segmentation** | Zeus (Vicuna + SAM) | *arXiv* | [![Paper](https://img.shields.io/badge/Paper-blue)](#) |

---

#### Multimodal Diagnosis & Clinical Reasoning

| Year | Title | Model | Venue | Links |
|------|-------|-------|-------|-------|
| 2024 | **GPT-4V for Zero-shot Chest X-ray Interpretation** | GPT-4V | *Radiology* | [![Paper](https://img.shields.io/badge/Paper-blue)](#) |
| 2024 | **In-context Learning for Histopathology Classification** | GPT-4V | *Nature Medicine* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://arxiv.org/abs/2312.02510) |
| 2024 | **SkinGPT-4: Dermatological Diagnosis from Patient Photos** | SkinGPT-4 (LLaMA-2-13B + ViT) | *Nature Communications* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://arxiv.org/abs/2304.10691) [![Code](https://img.shields.io/badge/Code-Available-blue)](https://github.com/JoshuaChou2018/SkinGPT-4) |
| 2025 | **M3FM: Multilingual Multimodal Medical Foundation Model** | M3FM | *arXiv* | [![Paper](https://img.shields.io/badge/Paper-blue)](#) |
| 2025 | **Multimodal LLMs for Laryngeal Cancer Surgical Decision Support** | Claude 3.5 Sonnet + 5 MLLMs | *Head & Neck* | [![Paper](https://img.shields.io/badge/Paper-blue)](#) |


---

## 🏆 Benchmark Leaderboard

> Results extracted from included studies.
> To update, please submit a PR — see [CONTRIBUTING.md](CONTRIBUTING.md).

### MedQA (USMLE) — Text QA

| Rank | Model | Accuracy | Year | Reference |
|------|-------|----------|------|-----------|
| 🥇 | GPT-4 | 86.7% | 2023 | [Nori et al.](https://arxiv.org/abs/2311.16452) |
| 🥈 | Med-PaLM 2 | 86.5% | 2023 | [Singhal et al.](https://arxiv.org/abs/2305.09617) |
| 🥉 | Med-PaLM | 67.6% | 2022 | [Singhal et al.](https://www.nature.com/articles/s41586-023-06291-2) |

### VQA-RAD — Closed-ended Accuracy

| Rank | Model | Accuracy | Year | Reference |
|------|-------|----------|------|-----------|
| 🥇 | CH-ICL | 77.08% | 2024 | [Liang et al.](#) |
| 🥈 | PMC-VQA | ~78% | 2024 | [Zhang et al.](#) |
| 🥉 | MiniMedGPT | ~75% | 2025 | [Alsabbagh et al.](#) |

### SLAKE — Open-ended Accuracy

| Rank | Model | Accuracy | Year | Reference |
|------|-------|----------|------|-----------|
| 🥇 | CH-ICL | 88.12% | 2024 | [Liang et al.](#) |
| 🥈 | PMC-VQA | ~84% | 2024 | [Zhang et al.](#) |
| 🥉 | MiniMedGPT | ~82% | 2025 | [Alsabbagh et al.](#) |

### MIMIC-CXR — Radiology Report Generation

| Rank | Model | ROUGE-L | Year | Reference |
|------|-------|---------|------|-----------|
| 🥇 | Flamingo-CXR | 77.7% pref. | 2024 | [Tanno et al.](#) |
| 🥈 | R2GenGPT | Competitive SOTA | 2023 | [Wang et al.](#) |


---

## 📦 Datasets and Resources

Full annotated table with access labels in [papers/datasets.md](papers/datasets.md).

| Dataset | Task | Modality | Access |
|---------|------|----------|--------|
| MedQA (USMLE) | QA / Reasoning | Text | Open |
| MedMCQA | QA / Reasoning | Text | Open |
| PubMedQA | QA | Text | Open |
| MultiMedQA | QA Suite | Text | Open |
| MedNLI | NLI | Text | Credentialed |
| MIMIC-III / IV | EHR Phenotyping | Text + Structured | Credentialed |
| MIMIC-CXR | Report Generation | Image + Text | Credentialed |
| CheXpert | Classification | Image | Registration |
| IU X-Ray | Report Generation | Image + Text | Open |
| VQA-RAD | Medical VQA | Image + Text | Open |
| SLAKE | Medical VQA | Image + Text | Open |
| PathVQA | Medical VQA | Image + Text | Open |
| PMC-VQA | Medical VQA | Image + Text | Open |
| PMC-15M | VLM Pretraining | Image + Text | Open |
| QUILT-1M | VLM Pretraining | Image + Text | Open |
| ISIC | Skin Lesion Seg. | Image | Open |
| Med. Seg. Decathlon | Multi-organ Seg. | Image | Open |
| TCGA | Cancer Subtyping | Multi-omics + Clinical | Open |

---

## 📚 Related Surveys

| Title | Venue | Year | Link |
|-------|-------|------|------|
| Large language models in medicine | *Nature Medicine* | 2023 | [Paper](https://www.nature.com/articles/s41591-023-02448-8) |
| Foundation models for generalist medical AI | *Nature* | 2023 | [Paper](https://www.nature.com/articles/s41586-023-05881-4) |
| Precision and Personalization: LLMs in Diagnostic Accuracy | *IEEE JBHI* | 2025 | [Paper](https://doi.org/10.1109/JBHI.2025.3584179) |
| A survey of large language models in medicine | *arXiv* | 2023 | [Paper](https://arxiv.org/abs/2311.05112) |
| The future landscape of LLMs in medicine | *Communications Medicine* | 2023 | [Paper](https://www.nature.com/articles/s43856-023-00370-1) |


---

## 🤝 How to Contribute

We welcome contributions from the community. To add a new paper:

1. **Fork** this repository
2. **Add** the paper to the correct section following the table format
3. **Submit** a Pull Request with title: `Add: [Paper Title]`

Or open an [Issue](.github/ISSUE_TEMPLATE/add_paper.md) using
the Add Paper template.

Full guidelines in [CONTRIBUTING.md](CONTRIBUTING.md).


---

## 📖 Citation

If this repository or survey is useful for your research, please cite:
```bibtex
@article{,
  
}
```

---



⭐ **Star this repo if you find it useful**

[![GitHub stars](https://img.shields.io/github/stars/walid798/llms-in-medicine?style=social)](https://github.com/walid798/llms-in-medicine)

