# 🧱 Foundation Models

A chronological catalogue of general-purpose and open-weight foundation models that underpin LLM research in clinical medicine. Part of the survey: *"Large Language Models in Clinical Medicine — A Systematic Review of Multimodal Architectures, Benchmarks, and Personalized Healthcare Applications"*.

> **Last updated:** April 2026 · **Total models listed:** 24 · **Timeline:** 2017–2025

---

## Table of Contents

- [General-Domain Models (2017–2022)](#1-general-domain-models-2017-2022)
- [Open-Weight General LLMs (2022–2024)](#2-open-weight-general-llms-2022-2024)
- [Open-Weight MoE Models](#3-open-weight-moe-models)
- [Reasoning & Multimodal Models (2025)](#4-reasoning--multimodal-models-2025)

---

## 1. General-Domain Models (2017–2022)

The foundational architectures and pre-trained models that established the transformer paradigm and scaling laws underpinning all subsequent LLM development.

| Year | Model | Modality | Parameters | Open-weight | Organization | Key Note | Reference |
|------|-------|----------|------------|:-----------:|-------------|----------|-----------|
| 2017 | Transformer | Text | — | — | Google/Brain | Self-attention architecture | [Paper](https://arxiv.org/abs/1706.03762) |
| 2018 | BERT | Text | 0.11 / 0.34 B | — | Google | Bidirectional MLM pretraining | [Paper](https://arxiv.org/abs/1810.04805) |
| 2019 | GPT-2 | Text | 1.5 B | ❌ | OpenAI | Large autoregressive LM | [Paper](https://cdn.openai.com/better-language-models/language_models_are_unsupervised_multitask_learners.pdf) |
| 2020 | GPT-3 | Text | 175 B | ❌ | OpenAI | In-context learning at scale | [Paper](https://arxiv.org/abs/2005.14165) |
| 2020 | T5 | Text | 11 B | — | Google | Text-to-text encoder–decoder | [Paper](https://jmlr.org/papers/volume21/20-074/20-074.pdf) |
| 2022 | PaLM | Text | 540 B | ❌ | Google | Scaling milestone | [Paper](https://arxiv.org/abs/2204.02311) |
| 2022 | BLOOM | Text | 176 B | ✅ | BigScience | Open multilingual LLM | [Paper](https://arxiv.org/abs/2211.05100) |

---

## 2. Open-Weight General LLMs (2022–2024)

Open-weight decoder-only models that have become the dominant backbone for medical LLM fine-tuning research.

| Year | Model | Modality | Parameters | Open-weight | Organization | Key Note | Reference |
|------|-------|----------|------------|:-----------:|-------------|----------|-----------|
| 2023 | LLaMA | Text | 7–65 B | ✅ | Meta | Open foundation family | [Paper](https://arxiv.org/abs/2302.13971) |
| 2023 | Llama 2 | Text | 7–70 B | ✅ | Meta | Chat-tuned variants | [Paper](https://arxiv.org/abs/2307.09288) |
| 2023 | Mistral 7B | Text | 7 B | ✅ | Mistral AI | Strong 7B baseline | [Blog](https://mistral.ai/news/announcing-mistral-7b) |
| 2023 | Qwen | Text | — | ✅ | Qwen (Alibaba) | Qwen LLM series | [Paper](https://arxiv.org/abs/2309.16609) |
| 2023 | DeepSeek-LLM | Text | 7 / 67 B | ✅ | DeepSeek | DeepSeek base/chat | [GitHub](https://github.com/deepseek-ai/DeepSeek-LLM) |
| 2024 | Gemma | Text | 2 / 7 B | ✅ | Google | Lightweight open models | [Blog](https://blog.google/technology/developers/gemma-open-models/) |
| 2024 | Llama 3 | Text | 8 / 70 B | ✅ | Meta | Llama 3 family | [Blog](https://ai.meta.com/blog/meta-llama-3/) |
| 2024 | Llama 3.1 | Text | 8 / 70 / 405 B | ✅ | Meta | Includes 405B release | [Blog](https://ai.meta.com/blog/meta-llama-3-1/) |
| 2024 | Qwen2 | Text | 0.5–72 B | ✅ | Qwen (Alibaba) | Qwen2 series | [Paper](https://arxiv.org/abs/2407.10671) |
| 2024 | Qwen2.5 | Text | — | ✅ | Qwen (Alibaba) | Qwen2.5 series | [Paper](https://arxiv.org/abs/2412.15115) |

---

## 3. Open-Weight MoE Models

Mixture-of-Experts architectures providing high capability at lower active-parameter inference cost — increasingly used as medical LLM backbones.

| Year | Model | Modality | Parameters | Open-weight | Organization | Key Note | Reference |
|------|-------|----------|------------|:-----------:|-------------|----------|-----------|
| 2023 | Mixtral 8×7B | Text | 8×7 B | ✅ | Mistral AI | Sparse MoE model | [Blog](https://mistral.ai/news/mixtral-of-experts) |
| 2024 | DeepSeek-V2 | Text | 236B total / 21B active | ✅ | DeepSeek | Economical MoE | [Paper](https://arxiv.org/abs/2405.04434) |
| 2024 | DeepSeek-V3 | Text | 671B total / 37B active | ✅ | DeepSeek | MoE frontier model | [Paper](https://arxiv.org/abs/2412.19437) |

---

## 4. Reasoning & Multimodal Models (2025)

Latest open-weight models introducing chain-of-thought reasoning and native multimodal capabilities, with direct relevance to clinical decision support and medical image analysis.

| Year | Model | Modality | Parameters | Open-weight | Organization | Key Note | Reference |
|------|-------|----------|------------|:-----------:|-------------|----------|-----------|
| 2025 | DeepSeek-R1 | Text | — | ✅ | DeepSeek | RL reasoning model | [Paper](https://arxiv.org/abs/2501.12948) |
| 2025 | Qwen2.5-VL | Image + Text | — | ✅ | Qwen (Alibaba) | Vision-language flagship | [Paper](https://arxiv.org/abs/2502.13923) |
| 2025 | Llama 4 Scout / Maverick | Text + Image | — | ✅ | Meta | Open-weight multimodal, Apr 2025 | [Link](https://ai.meta.com/blog/llama4/) |
| 2025 | gpt-oss (120b / 20b) | Text | 117B / 21B (MoE) | ✅ | OpenAI | Apache-2.0 open weights | [GitHub](https://github.com/openai/gpt-oss) |

---

## Contributing

To suggest additions or corrections, please open an issue using the [model addition template](../../issues/new?template=model_addition.md) or submit a pull request.

---

*Part of [`walid798/llms-in-medicine`](https://github.com/walid798/llms-in-medicine)*

# Foundation and precursor language-model families

This page is **contextual background**, not the primary quantitative study register.

The final review applies a study-level eligibility rule: standalone encoder-only PLMs (for example, BERT-family biomedical/clinical encoders) are not counted in the primary corpus when used independently. They may still be cited to explain the evolution of clinical language modeling or when embedded inside an LLM-centered clinical system.

| Paradigm | Representative models | Role in the review |
|---|---|---|
| Encoder-based clinical PLMs | BERT, BioBERT, ClinicalBERT, PubMedBERT | Historical/contextual representation learning |
| Generative biomedical/clinical LMs | BioGPT, GPT-3.5/4, Med-PaLM, medical LLaMA variants | Generation, QA, summarization, clinical reasoning |
| Multimodal medical LLMs | LLaVA-Med, Med-PaLM M, PathChat, MAIRA-2 | Image–text and heterogeneous clinical reasoning |
| Retrieval/reasoning systems | Medical RAG, Graph-RAG, multimodal RAG, reasoning-optimized LLMs | External evidence grounding and multi-step inference |
| Agentic clinical systems | Tool-using agents, multi-agent systems, memory-/workflow-enabled agents | Tool orchestration, iterative actions, workflow integration |

For the actual 145 included studies, use [`../papers/studies.md`](../papers/studies.md) or [`../data/studies.csv`](../data/studies.csv).
