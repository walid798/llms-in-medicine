# 🏥 LLMs in Medicine

[![Maintained](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/walid798/llms-in-medicine)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Stars](https://img.shields.io/github/stars/walid798/llms-in-medicine?style=social)](https://github.com/walid798/llms-in-medicine)
[![Papers](https://img.shields.io/badge/Papers-56-blue)](README.md)
[![Categories](https://img.shields.io/badge/Categories-10-green)](README.md)
[![Updated](https://img.shields.io/badge/Updated-April%202025-orange)](CHANGELOG.md)

**A curated repository accompanying our systematic review:**

> **Large Language Models in Clinical Medicine: A Systematic Review of Multimodal Architectures, Benchmarks, and Personalized Healthcare Applications**
>
> Walid Mohamed, Mohamed Elsharkawy, Shahad Al Hamadani, Rafia Fayyaz, Usama Mousattat, 
> Taysir Hassan A. Soliman, Amr Mohamed Abdelaziz, 
> Ali Mahmoud, Mohamed Ghazal, Tania Tahtouh, Ayman El-Baz

## If you find this repository useful, please consider giving it a ⭐

---

## 📋 Table of Contents

<!-- - [What's New](#-whats-new) -->
- [Survey Overview](#-survey-overview)
- [Foundation Models](models/foundation-models.md)
- [Medical LLM Models](models/medical-llms.md)
- [Text-Based Applications](#-text-based-applications)
- [Multimodal Applications](#-multimodal-applications)
- [Datasets and Resources](#-datasets-and-resources)
- [Related Surveys](#-related-surveys)
- [How to Contribute](#-how-to-contribute)
- [Citation](#-citation)

---

<!-- ## 🆕 What's New

| Date | Update |
|------|--------|
| 2025-04 | 🎉 Repository launched alongside survey submission |
| 2026-03 | 56 studies added across 10 task categories |
| 2026-01 | Benchmark leaderboard added for MedQA, VQA-RAD, and SLAKE | -->

---

## 📊 Survey Overview

This repository accompanies a **PRISMA 2020-compliant systematic review**
synthesizing **56 studies** on LLMs in clinical medicine, organized around
**personalized healthcare** as a central analytical framework.

### Coverage at a Glance

| Task Category | Studies |
|---------------|---------|
| Clinical Documentation & IE | 5 |
| Literature Mining & Knowledge | 4 |
| Decision Support & QA | 5 |
| Radiology Report Classification | 5 |
| Pathology Report Classification | 4 |
| Radiology Report Generation | 6 |
| Pathology Report Generation | 5 |
| Medical Visual QA | 7 |
| LLM-Guided Segmentation | 4 |
| Multimodal Diagnosis | 11 |
| **Total** | **56** |

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

> 🧱 [**Foundation Models**](models/foundation-models.md): 24 general-purpose models from Transformer (2017) to Llama 4 (2025)  
> 🏥 [**Medical LLM Models**](models/medical-llms.md): 42 domain-adapted models across text, biomedical, and multimodal categories

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


---

### 🖼️ Multimodal Applications

#### Radiology Report Generation

| Year | Title | Model | Venue | Links |
|------|-------|-------|-------|-------|
| 2023 | **R2GenGPT: Radiology Report Generation with Frozen LLMs** | R2GenGPT | *Meta-Radiology* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://www.sciencedirect.com/science/article/pii/S2950162823000334) [![Code](https://img.shields.io/badge/Code-Available-green)](https://github.com/wang-zhanyu/R2GenGPT) |
| 2023 | **LLaVA-Med: Training a Large Language-and-Vision Assistant for Biomedicine in One Day** | LLaVA-Med (CLIP ViT + Vicuna/LLaMA) | *NeurIPS* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://neurips.cc/virtual/2023/poster/73643) [![Code](https://img.shields.io/badge/Code-Available-green)](https://github.com/microsoft/LLaVA-Med) |
| 2024 | **MAIRA-2: Grounded Radiology Report Generation** | MAIRA-2 (region-grounded VLM) | *arXiv* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://arxiv.org/abs/2406.04449) |
| 2025 | **Collaboration Between Clinicians and Vision-Language Models in Radiology Report Generation** | Flamingo-CXR (clinician-in-loop) | *Nature Medicine* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://www.nature.com/articles/s41591-024-03302-1) |
| 2025 | **Towards a Holistic Framework for Multimodal LLM in 3D Brain CT Radiology Report Generation** | BrainGPT (CVIT-based) | *Nature Communications* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://www.nature.com/articles/s41467-025-57426-0) |
| 2025 | **MediVLM: Annotation-Free Vision-Language Model for Radiology** | MediVLM | *ACL Anthology* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://aclanthology.org/2025.findings-emnlp.544/) |


---

### Pathology Report Generation

| Year | Title | Model | Venue | Links |
|------|-------|-------|-------|-------|
| 2024 | **WsiCaption: Multiple Instance Generation of Pathology Reports for Gigapixel Whole-Slide Images** | MI-Gen | *MICCAI 2024* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://link.springer.com/chapter/10.1007/978-3-031-72083-3_51) [![Code](https://img.shields.io/badge/Code-Available-green)](https://github.com/cpystan/Wsi-Caption) |
| 2024 | **HistGen: Histopathology Report Generation via Local-Global Feature Encoding and Cross-modal Context Interaction** | HistGen | *MICCAI 2024* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://link.springer.com/chapter/10.1007/978-3-031-72083-3_18) [![Code](https://img.shields.io/badge/Code-Available-green)](https://github.com/dddavid4real/HistGen) |
| 2024 | **Clinical-Grade Multi-organ Pathology Report Generation for Multi-scale WSIs via a Semantically Guided Medical Text Foundation Model** | Semantically Guided VLM | *MICCAI 2024* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://link.springer.com/chapter/10.1007/978-3-031-72083-3_3) [![Code](https://img.shields.io/badge/Code-Available-green)](https://github.com/hvcl/Clinical-grade-Pathology-Report-Generation/tree/main)| 
| 2025 | **Pathology Report Generation from Whole Slide Images with Knowledge Retrieval and Multi-level Regional Feature Selection** | Multi-level Regional + LLM refinement | *Comput. Methods Programs Biomed.* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://www.sciencedirect.com/science/article/pii/S016926072500094X) |
| 2025 | **A Multimodal Whole-Slide Foundation Model for Pathology** | TITAN (CONCH + Transformer) | *Nature Medicine* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://www.nature.com/articles/s41591-025-03982-3) [![Code](https://img.shields.io/badge/Code-Available-green)](https://github.com/mahmoodlab/TITAN) |
| 2025 | **PolyPath: Adapting a Large Multimodal Model for Multi-slide Pathology Report Generation** | Gemini 1.5 Flash (1M-token context) | *Modern Pathology* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://www.sciencedirect.com/science/article/pii/S089339522500184X) |
| 2025 | **Enhancing Pathology Report Generation Under Data Scarcity via Modular MIL + T5 Pipeline** | MIL + T5 (modular) | *IEEE Access* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://ieeexplore.ieee.org/abstract/document/11078283) |

---

#### Medical Visual Question Answering

| Year | Title | Model | Venue | Links |
|------|-------|-------|-------|-------|
| 2023 | **LLaVA-Med: Training a Large Language-and-Vision Assistant for Biomedicine** | LLaVA-Med | *NeurIPS 2023* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://arxiv.org/abs/2306.00890) [![Code](https://img.shields.io/badge/Code-Available-blue)](https://github.com/microsoft/LLaVA-Med) ![SOTA](https://img.shields.io/badge/-SOTA-red) |
| 2024 | **PMC-VQA: Visual Instruction Tuning for Medical VQA** | PMC-VQA | *Communications Medicine* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://www.nature.com/articles/s43856-024-00709-2) [![Code](https://img.shields.io/badge/Code-Available-blue)](https://github.com/xiaoman-zhang/PMC-VQA) |
| 2024 | **Candidate Answer Set Guided Medical VQA** | CH-ICL | *arXiv* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://arxiv.org/abs/2408.10048) |
| 2024 | **Falcon Med-VQA: Uncertainty-aware Clinical QA** | Falcon Med-VQA | *arXiv* | [![Paper](https://img.shields.io/badge/Paper-blue)](#) |
| 2024 | **OmniMedVQA: A New Large-Scale Comprehensive Evaluation Benchmark for Medical LVLM** | Evaluation benchmark (12 modalities) | *CVPR 2024* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://openaccess.thecvf.com/content/CVPR2024/papers/Hu_OmniMedVQA_A_New_Large-Scale_Comprehensive_Evaluation_Benchmark_for_Medical_LVLM_CVPR_2024_paper.pdf) |
| 2025 | **MiniMedGPT: Parameter-Efficient Medical VQA** | MiniMedGPT (EVA-CLIP + LLaMA2-7B) | *arXiv* | [![Paper](https://img.shields.io/badge/Paper-blue)](#) |
| 2025 | **FAVP: Fine-grained Adaptive Visual Prompts for Generative MedVQA** | FAVP (ViT-G/14 + Vicuna-7B) | *AAAI 2025* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://github.com/OpenMICG/FAVP) [![Code](https://img.shields.io/badge/Code-Available-blue)](https://github.com/OpenMICG/FAVP) |
| 2025 | **Structural Causal Models and LLMs for Medical VQA** | CIF (CLIP + LLaMA 7B/13B) | *IEEE Transactions* | [![Paper](https://img.shields.io/badge/Paper-blue)](#) |

---

### LLM-Guided Image Segmentation

| Year | Title | Model | Venue | Links |
|------|-------|-------|-------|-------|
| 2025 | **Pre-Trained LLM is a Semantic-Aware and Generalizable Segmentation Booster** | LLM4Seg (frozen LLaMA3.2-1B or DeepSeek layer + CNN encoder-decoder) | *MICCAI 2025* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://link.springer.com/chapter/10.1007/978-3-032-05127-1_39) [![Code](https://img.shields.io/badge/Code-Available-green)](https://github.com/FengheTan9/LLM4Seg) |
| 2025 | **MedVisionLlama: Leveraging Pre-Trained Large Language Model Layers to Enhance Medical Image Segmentation** | MedVisionLlama (frozen Llama-3.1-8B blocks + ViT encoder; LoRA) | *ICCV 2025 Workshop (CVAMD)* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://arxiv.org/abs/2410.02458) [![Code](https://img.shields.io/badge/Code-Available-green)](https://github.com/AS-Lab/Marthi-et-al-2025-MedVisionLlama-Pre-Trained-LLM-Layers-to-Enhance-Medical-Image-Segmentation) |
| 2025 | **Zeus: Zero-Shot LLM Instruction for Union Segmentation in Multimodal Medical Imaging** | Zeus (frozen Vicuna as instruction generator + SAM mask decoder) | *International Journal of Machine Learning and Cybernetics* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://link.springer.com/article/10.1007/s13042-025-02742-6) |
| 2025 | **Beyond Pixel Agreement: Large Language Models as Clinical Guardrails for Reliable Medical Image Segmentation** | HCR (Gemini 2.5 Flash; hierarchical multi-stage prompting) | *arXiv* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://arxiv.org/abs/2506.01841) |

---

### Multimodal Clinical Diagnosis and Reasoning

| Year | Title | Model | Venue | Links |
|------|-------|-------|-------|-------|
| 2024 | **Evaluating GPT-4V on Chest Radiograph Interpretation: Zero-Shot and Few-Shot Performance** | GPT-4V (zero-shot / few-shot) | *Radiology: Artificial Intelligence* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://pubmed.ncbi.nlm.nih.gov/38713028/) |
| 2025 | **Multimodal Large Language Models for Laryngeal Cancer Diagnosis: A Comparative Study** | Claude 3.5 Sonnet + 5 MLLMs | *arXiv* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://journals.lww.com/international-journal-of-surgery/fulltext/2025/03000/multimodal_large_language_models_address_clinical.36.aspx) |
| 2024 | **In-Context Learning Enables Multimodal Large Language Models to Classify Cancer Pathology Images** | GPT-4V (in-context; no fine-tuning) | *Nature Communications* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://www.nature.com/articles/s41467-024-51465-9) [![Code](https://img.shields.io/badge/Code-Available-blue)](https://github.com/Dyke-F/GPT-4V-In-Context-Learning) |
| 2025 | **A multimodal multidomain multilingual medical foundation model for zero shot clinical diagnosis** | M3FM | *npj digital medicine* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://www.nature.com/articles/s41746-024-01339-7) |
| 2024 | **Pre-trained multimodal large language model enhances dermatological diagnosis using SkinGPT-4** | SkinGPT-4 (LLaMA-2-13B + ViT) | *Nature Communications* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://www.nature.com/articles/s41467-024-50043-3) [![Code](https://img.shields.io/badge/Code-Available-green)](https://github.com/JoshuaChou2018/SkinGPT-4) |
| 2024 | **A multimodal generative AI copilot for human pathology** | PathChat (UNI ViT + LLaMA 13B; projection fusion) | *Nature* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://www.nature.com/articles/s41586-024-07618-3) [![Code](https://img.shields.io/badge/Code-Available-green)](https://github.com/fedshyvana/pathology_mllm_training) |
| 2024 | **Towards Generalist Biomedical AI** | Med-PaLM M (PaLM-E + ViT; 14-task unified) | *NEJM AI* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://ai.nejm.org/doi/full/10.1056/AIoa2300138) |
| 2024 | **LLM-Driven Multimodal Target Volume Contouring in Radiation Oncology** | LLMSeg (3D CT + clinical text; cross-attention) | *Nature Communications* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://www.nature.com/articles/s41467-024-53387-y) [![Code](https://img.shields.io/badge/Code-Available-green)](https://github.com/tvseg/MM-LLM-RO)|
| 2025 | **MedTVT-R1: A Multimodal LLM Empowering Medical Reasoning and Diagnosis** | MedTVT-R1 (LLaMA3.2 + ECG + CXR + Lab; adaptive cross-modal attention) | *arXiv* | [![Paper](https://img.shields.io/badge/Paper-blue)](MedTVT-R1: A Multimodal LLM Empowering Medical Reasoning and Diagnosis) [![Code](https://img.shields.io/badge/Code-Available-green)](https://github.com/keke-nice/MedTVT-R1) |
| 2024 | **MEDFuse: Multimodal EHR Data Fusion with Masked Lab-Test Modeling and Large Language Models** | MEDFuse (lab-test transformer + LLM notes; cross-attention intermediate fusion) | *CIKM 2024* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://dl.acm.org/doi/10.1145/3627673.3679962) |
| 2025 | **SMFusion: Semantic-Preserving Fusion of Multimodal Medical Images for Enhanced Clinical Diagnosis** | SMFusion (BiomedGPT text + cross-attention + PET/MRI) | *IEEE JBHI* | [![Paper](https://img.shields.io/badge/Paper-blue)](https://ieeexplore.ieee.org/abstract/document/11319543) |


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

## Star History

<a href="https://www.star-history.com/?repos=walid798%2Fllms-in-medicine&type=date&legend=bottom-right">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/chart?repos=walid798/llms-in-medicine&type=date&theme=dark&legend=bottom-right" />
   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/chart?repos=walid798/llms-in-medicine&type=date&legend=bottom-right" />
   <img alt="Star History Chart" src="https://api.star-history.com/chart?repos=walid798/llms-in-medicine&type=date&legend=bottom-right" />
 </picture>
</a>

