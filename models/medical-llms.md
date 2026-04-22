# 🏥 Medical LLM Models

A curated catalogue of domain-adapted language models for clinical and biomedical applications, organized by category. Part of the survey: *"Large Language Models in Clinical Medicine — A Systematic Review of Multimodal Architectures, Benchmarks, and Personalized Healthcare Applications"*.

> **Last updated:** April 2026 · **Total models listed:** 42

---

## Table of Contents

- [Medical LLMs — Clinical Text & Instruction-Tuned](#1-medical-llms--clinical-text--instruction-tuned)
- [Biomedical Text Language Models](#2-biomedical-text-language-models)
- [Multimodal Medical LMMs](#3-multimodal-medical-lmms)
- [General-Domain Open Models Used in Medical Research](#4-general-domain-open-models-used-in-medical-research)

---

## 1. Medical LLMs — Clinical Text & Instruction-Tuned

Models fine-tuned or instruction-tuned on clinical/medical corpora, designed for medical QA, clinical reasoning, and healthcare dialogue.

| Model | Backbone | Params (B) | Fine-tuning Method | Open Source | Year | Training Data Size |
|-------|----------|------------|-------------------|:-----------:|------|--------------------|
| [Med-PaLM](https://arxiv.org/abs/2212.13138) | PaLM | 540 | Prompt Tuning | ❌ | 2023 | 65 items |
| [ChatDoctor](https://arxiv.org/abs/2303.14070) | LLaMA | 7 | Full Param. | ✅ | 2023 | 152K items |
| [Med-PaLM 2](https://arxiv.org/abs/2305.09617) | PaLM2 | 340 | — | ❌ | 2023 | 193K items |
| [Clinical Camel](https://arxiv.org/abs/2305.12031) | LLaMA2 | 13, 70 | QLoRA | ✅ | 2023 | 174K items |
| [MedicalGPT](https://github.com/shibing624/MedicalGPT) | Ziya/Baichuan | 13 | LoRA | ✅ | 2023 | 361K+2.07M+3.8K |
| [AlpaCare](https://arxiv.org/abs/2310.14558) | LLaMA | 7, 13 | Full Param. | ✅ | 2023 | 52K items |
| [Taiyi](https://arxiv.org/abs/2311.11608) | Qwen | 7 | QLoRA | ✅ | 2023 | 1,114K items |
| [MediTron](https://arxiv.org/abs/2311.16079) | LLaMA2 | 7, 70 | Full Param. | ✅ | 2023 | 48B tok; 369K |
| [AntGLM-Med](https://arxiv.org/abs/2309.13027) | GLM | 10 | Full/LoRA/Cpoly | ❌ | 2023 | 15.39B; 632K |
| [EpilepsyLLM](https://arxiv.org/abs/2406.10018) | LLM-JP/LLaMA | 1.3, 7 | LoRA | ✅ | 2024 | 52.2K items |
| [BioMistral](https://arxiv.org/abs/2402.10373) | Mistral-Instruct | 7 | QLoRA | ✅ | 2024 | 3B tok; 405K |
| [MMedLM](https://arxiv.org/abs/2402.13963) | InternLM | 7 | Full/LoRA | ✅ | 2024 | 25.5B; 45K |
| [InMD-X](https://arxiv.org/abs/2402.16749) | Neural-Chat | 7 | Full/LoRA | ❌ | 2024 | 150M tok; 1,701K |
| [Me-LLaMA](https://arxiv.org/abs/2402.12749) | LLaMA2 | 13, 70 | LoRA | ✅ | 2024 | 129B; 214K |
| JMLR | LLaMA2 | 7, 13 | — | ❌ | 2024 | — |
| [BiMediX](https://arxiv.org/abs/2402.13253) | Mixtral-8x7B | 8×7 | QLoRA | ✅ | 2024 | 1,311K items |
| [OncoGPT](https://arxiv.org/abs/2402.16810) | LLaMA | 7 | LoRA | ✅ | 2024 | 332K items |
| [Apollo](https://arxiv.org/abs/2403.03562) | Qwen/Gemma/Yi | 0.5–7 | Full Param. | ✅ | 2024 | 2B tok; 481M |
| [MING-MOE](https://arxiv.org/abs/2404.09027) | Qwen1.5-Chat | 1.8–14 | LoRA | ✅ | 2024 | 300K items |
| [LingDan](https://arxiv.org/abs/2404.13340) | Baichuan2 | 13 | QLoRA | ✅ | 2024 | 304M; 201.5K |
| [UltraMedical](https://arxiv.org/abs/2406.03949) | LLaMA3 | 8, 70 | — | ✅ | 2024 | 600K; 100K |
| [Aloe](https://arxiv.org/abs/2405.01886) | Mistral/LLaMA3 | 7, 8 | Full Param. | ✅ | 2024 | 872K; 12K |
| [Med42-v2](https://arxiv.org/abs/2408.06142) | LLaMA3.1 | 8, 70 | Full Param. | ✅ | 2024 | 1,296K; 120K |
| [MMedIns-Llama 3](https://arxiv.org/abs/2402.13963) | MMed-Llama 3 | 8 | — | ✅ | 2024 | 5M items |
| [FineMedLM-o1](https://arxiv.org/abs/2501.09056) | LLaMA3.1 | 8 | Full Param. | ✅ | 2025 | 300K; 33K |
| [ClinicalGPT-R1](https://arxiv.org/abs/2503.00700) | Qwen2.5-Instruct | 7 | — | ✅ | 2025 | — |

---

## 2. Biomedical Text Language Models

BERT-family and encoder-decoder models pre-trained or continually pre-trained on biomedical and clinical text corpora.

| Model | Backbone | Params (B) | Training Strategy | Open Source | Year | Training Corpus | Reference |
|-------|----------|------------|------------------|:-----------:|------|-----------------|-----------|
| BioBERT | BERT | 0.11/0.34 | Continued pretraining | ✅ | 2019 | PubMed + PMC | [Link](https://academic.oup.com/bioinformatics/article/36/4/1234/5566506) |
| ClinicalBERT | BERT | 0.11/0.34 | Continued pretraining | ✅ | 2019 | MIMIC-III notes | [Link](https://aclanthology.org/W19-1909/) |
| PubMedBERT | BERT (from scratch) | 0.11/0.34 | Pretraining from scratch | ✅ | 2020 | PubMed abstracts | [Link](https://arxiv.org/abs/2007.15779) |
| SciFive | T5 | 0.22/0.77/3/11 | Continued pretraining | ✅ | 2021 | PubMed + PMC | [Link](https://arxiv.org/abs/2106.03598) |
| BioGPT | GPT-2 style | 0.35 | Pretraining + finetune | ✅ | 2022 | PubMed abstracts | [Link](https://academic.oup.com/bib/article/23/6/bbac409/6713511) |

---

## 3. Multimodal Medical LMMs

Large multimodal models (LMMs) adapted for clinical imaging tasks including radiology, pathology, and general medical visual QA.

| Model | Backbone | Modality | Training Strategy | Open Source | Year | Training Data | Reference |
|-------|----------|----------|------------------|:-----------:|------|---------------|-----------|
| LLaVA-Med | LLaVA/Vicuna + biomedical VLM | Image + Text | Instruction tuning | ✅ | 2023 | PMC + GPT-4 self-instruct | [Link](https://arxiv.org/abs/2306.00890) |
| Med-Flamingo | Flamingo | Image + Text | Instruction tuning | ❌ | 2023 | Multi-domain medical VQA | [Link](https://arxiv.org/abs/2307.15189) |
| RadFM | Multimodal foundation model | Image + Text | Pretraining + instruction tuning | ✅ | 2023 | Radiology images + text | [Link](https://arxiv.org/abs/2308.02463) |
| PLIP | CLIP-style | Image + Text | Pretraining | ✅ | 2023 | Pathology image-text pairs | [Link](https://pubmed.ncbi.nlm.nih.gov/37592105/) |
| PathChat | LLaVA-based | Image + Text | Instruction tuning | — | 2024 | Pathology corpora | [Link](https://arxiv.org/abs/2312.07814) |
| CheXagent | LMM for CXR | Image + Text | Instruction tuning | ✅ | 2024 | CheXinstruct | [Link](https://arxiv.org/abs/2401.12208) |
| Med-Gemini | Gemini | Image + Text + Video (+omics) | Multimodal adaptation | ❌ | 2024 | Multi-modal medical data | [Link](https://arxiv.org/abs/2405.03162) |

---

## 4. General-Domain Open Models Used in Medical Research

Recent open-weight general models leveraged in clinical NLP and medical AI research.

| Model | Backbone | Modality | Key Note | Open Source | Year | Reference |
|-------|----------|----------|----------|:-----------:|------|-----------|
| DeepSeek-R1 | DeepSeek | Text | RL for reasoning | ✅ | 2025 | [Link](https://arxiv.org/abs/2501.12948) |
| Qwen2.5-VL | Qwen | Image + Text | VLM training | ✅ | 2025 | [Link](https://arxiv.org/abs/2502.13923) |
| gpt-oss-120b / gpt-oss-20b | OpenAI | Text | Open-weight release (Apache 2.0) | ✅ | 2025 | [Link](https://github.com/openai/gpt-oss) |
| Llama 4 Scout / Maverick | Llama 4 | Text + Image | Open-weight multimodal | ✅ | 2025 | [Link](https://ai.meta.com/blog/llama4/) |

---

## Contributing

To suggest additions or corrections, please open an issue using the [model addition template](../../issues/new?template=model_addition.md) or submit a pull request.

---

*Part of [`walid798/llms-in-medicine`](https://github.com/walid798/llms-in-medicine)*