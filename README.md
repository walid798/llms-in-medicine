# 🏥 LLMs in Medicine

[![Maintained](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/walid798/llms-in-medicine)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Stars](https://img.shields.io/github/stars/walid798/llms-in-medicine?style=social)](https://github.com/walid798/llms-in-medicine)

**A curated repository accompanying our systematic survey:**

> **Large Language Models in Clinical Medicine — A Systematic Review of
> Multimodal Architectures, Benchmarks, and Personalized Healthcare Applications**
>
> Walid Mohamed
>

## If you find this repository useful, please consider giving it a ⭐

---

## 📋 Table of Contents

- [What's New](#-whats-new)
- [Survey Overview](#-survey-overview)
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
| 2022 | **GatorTron: A Large Clinical Language Model to Unlock Patient Information from Unstructured EHRs** | GatorTron (8.9B) | *npj Digital Medicine* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://www.nature.com/articles/s41746-022-00742-2) [![Code](https://img.shields.io/badge/Code-Available-blue)](https://github.com/uf-hobi-informatics-lab/GatorTron) |
| 2023 | **Health System-Scale Language Models Are All-Purpose Prediction Engines** | NYUTron | *Nature* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://www.nature.com/articles/s41586-023-06160-y) ![Prospective](https://img.shields.io/badge/Val-Prospective-purple) |
| 2024 | **Large Language Models to Identify Social Determinants of Health in EHRs** | Flan-T5 XL/XXL | *npj Digital Medicine* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://www.nature.com/articles/s41746-023-00970-0) ![External](https://img.shields.io/badge/Val-External-orange) |
| 2025 | **Open-Source LLM for Treatment Pathway Reconstruction** | Hybrid LLM (UMLS) | *J. Biomedical Informatics* | [![Paper](https://img.shields.io/badge/Paper-blue)](#) ![External](https://img.shields.io/badge/Val-External-orange) |
| 2025 | **Automated Extraction from German Discharge Letters** | GPT-4 | *Preprint* | [![Paper](https://img.shields.io/badge/Paper-blue)](#) |


---

#### Biomedical Literature Mining & Knowledge Synthesis

| Year | Title | Model | Venue | Links |
|------|-------|-------|-------|-------|
| 2020 | **BioBERT: A Pre-trained Biomedical Language Representation Model** | BioBERT | *Bioinformatics* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://academic.oup.com/bioinformatics/article/36/4/1234/5566506) [![Code](https://img.shields.io/badge/Code-Available-blue)](https://github.com/dmis-lab/biobert) |
| 2022 | **BioGPT: Generative Pre-trained Transformer for Biomedical Text Generation** | BioGPT | *Briefings in Bioinformatics* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://academic.oup.com/bib/article/23/6/bbac409/6713511) [![Code](https://img.shields.io/badge/Code-Available-blue)](https://github.com/microsoft/BioGPT) |
| 2025 | **BiomedRAG: A Retrieval-Augmented LLM for Biomedicine** | BiomedRAG (LLaMA2 / MedLLaMA-13B) | *Preprint* | [![Paper](https://img.shields.io/badge/Paper-blue)](#) [![Code](https://img.shields.io/badge/Code-Available-blue)](#) |



---

#### Clinical Decision Support & Question Answering

| Year | Title | Model | Venue | Links |
|------|-------|-------|-------|-------|
| 2023 | **Large Language Models Encode Clinical Knowledge** | Med-PaLM (Flan-PaLM) | *Nature* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://www.nature.com/articles/s41586-023-06291-2) ![SOTA](https://img.shields.io/badge/-SOTA-red) |
| 2023 | **Can Generalist Foundation Models Outcompete Special-Purpose Tuning?** | GPT-4 | *arXiv* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://arxiv.org/abs/2311.16452) |
| 2023 | **ChatDoctor: A Medical Chat Model Fine-Tuned on LLaMA** | ChatDoctor (LLaMA-7B) | *Cureus* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://www.cureus.com/articles/152858) [![Code](https://img.shields.io/badge/Code-Available-blue)](https://github.com/Kent0n-Li/ChatDoctor) |
| 2024 | **Mental-LLM: Leveraging LLMs for Mental Health Prediction** | Mental-LLM | *ACM SIGCHI* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://arxiv.org/abs/2307.14385) [![Code](https://img.shields.io/badge/Code-Available-blue)](https://github.com/neuhai/Mental-LLM) |
| 2025 | **Evaluating GPT-4 for Radiology Patient Education** | GPT-4 | *European Radiology* | [![Paper](https://img.shields.io/badge/Paper-blue)](#) |


---

#### Report Classification — Radiology & Pathology

| Year | Title | Model | Venue | Links |
|------|-------|-------|-------|-------|
| 2023 | **Exploring the Boundaries of GPT-4 in Radiology** | GPT-4 | *arXiv* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://arxiv.org/abs/2310.14573) |
| 2024 | **Language Models for Italian Neoplastic CT Report Classification** | Italian BERT / GPT-4 | *Diagnostics* | [![Paper](https://img.shields.io/badge/Paper-blue)](#) |
| 2024 | **GPT-3.5 for Multilingual TNM Staging** | GPT-3.5-turbo | *Japanese Journal of Radiology* | [![Paper](https://img.shields.io/badge/Paper-blue)](#) |
| 2024 | **Automated Treatment Classification from Japanese Brain MRI Reports** | Japanese BERT | *Radiology: AI* | [![Paper](https://img.shields.io/badge/Paper-blue)](#) |
| 2024 | **Generalizable TNM Staging via BigBird** | BB-TEN (BigBird) | *NPJ Precision Oncology* | [![Paper](https://img.shields.io/badge/Paper-blue)](#) ![External](https://img.shields.io/badge/Val-External-orange) |
| 2024 | **Zero-shot Breast Cancer Subtype Classification** | GPT-4 | *Modern Pathology* | [![Paper](https://img.shields.io/badge/Paper-blue)](#) |
| 2025 | **Cancer Type and Staging from Pathology Reports** | Path-llama3.1 | *J. Pathology Informatics* | [![Paper](https://img.shields.io/badge/Paper-blue)](#) ![External](https://img.shields.io/badge/Val-External-orange) |
| 2025 | **Gynecologic Oncology Registry Automation** | Gemini 1.5 / Qwen2.5 72B | *Gynecologic Oncology* | [![Paper](https://img.shields.io/badge/Paper-blue)](#) ![External](https://img.shields.io/badge/Val-External-orange) |

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

