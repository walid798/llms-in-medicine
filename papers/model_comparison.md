# Model Comparison Table

Structured comparison of all LLMs evaluated across the 47 included studies,
covering architecture, scale, pretraining, adaptation method, and availability.

> **Note:** This table is updated as new papers are added to the corpus.
> Current count: 47 studies · Last updated: April 2025

---

## Foundational LLMs Used in Clinical Adaptation

| Model | Base Architecture | Parameters | Pretraining Data | Fine-tuning Method | Open Source | Clinical Specialty |
|-------|------------------|------------|------------------|--------------------|-------------|-------------------|
| GPT-4 | Transformer (decoder) | Undisclosed | Undisclosed | RLHF + instruction tuning | NO | General; Radiology; Pathology |
| GPT-3.5-turbo | Transformer (decoder) | ~175B | Undisclosed | RLHF | NO | General; Radiology |
| Claude 3.5 Sonnet | Transformer (decoder) | Undisclosed | Undisclosed | Constitutional AI | NO | Multimodal diagnosis |
| Gemini 1.5 | Multimodal transformer | Undisclosed | Undisclosed | Instruction tuning | NO | Pathology; Radiology |
| Flan-PaLM | Transformer (decoder) | 540B | C4 + others | Instruction tuning | NO | Medical QA |
| Flan-T5 XL/XXL | Transformer (enc-dec) | 3B / 11B | C4 | Instruction tuning | YES | Clinical NLP |
| LLaMA-7B | Transformer (decoder) | 7B | CommonCrawl + others | SFT on dialogues | YES | Patient QA |
| LLaMA-2-13B | Transformer (decoder) | 13B | 2T tokens | RLHF | YES | Dermatology; Multimodal |
| LLaMA-3.1-8B | Transformer (decoder) | 8B | 15T tokens | Instruction tuning | YES | Segmentation |
| LLaMA3.2-1B | Transformer (decoder) | 1B | Undisclosed | Instruction tuning | YES | Segmentation |
| Vicuna-7B | Transformer (decoder) | 7B | ShareGPT dialogues | SFT on LLaMA | YES | Medical VQA; Segmentation |
| Qwen2.5 72B | Transformer (decoder) | 72B | 18T tokens | Instruction tuning | YES | Pathology classification |
| DeepSeek-R1-Distill | Transformer (decoder) | 1.5B | Undisclosed | Distillation + RL | YES | Segmentation |

---

## Biomedical Domain-Adapted LLMs

| Model | Base Model | Parameters | Pretraining / Adaptation Data | Adaptation Method | Open Source | Primary Task |
|-------|-----------|------------|-------------------------------|-------------------|-------------|-------------|
| GatorTron | From scratch | 8.9B | UF Health EHR (90B tokens) | Pretraining from scratch | YES | Clinical NLP |
| NYUTron | From scratch | Undisclosed | NYU Langone EHR | Pretraining + fine-tuning | NO | Outcome prediction |
| BioBERT | BERT | 110M | PubMed + PMC (18B tokens) | Domain-adaptive pretraining | YES | NER; RE; QA |
| BioGPT | GPT-2 | 347M | PubMed abstracts (15M) | Pretraining from scratch | YES | Biomedical text generation |
| BiomedRAG | LLaMA2 / MedLLaMA-13B | 13B | Biomedical NLP datasets | RAG + fine-tuning | YES | Evidence retrieval |
| Med-PaLM | Flan-PaLM | 540B | MultiMedQA | Instruction tuning | NO | Medical QA |
| ChatDoctor | LLaMA-7B | 7B | 100K patient-physician dialogues | SFT | YES | Patient QA |
| Mental-LLM | Multiple LLMs | Various | Reddit mental health data | Fine-tuning | YES | Mental health monitoring |
| Path-llama3.1 | LLaMA-3.1 | Undisclosed | TCGA pathology reports | Fine-tuning | NO | Cancer staging |
| Hybrid LLM (UMLS) | Fine-tuned LLM | Undisclosed | Mayo/Stanford EHR + UMLS | UMLS-augmented FT | NO | Treatment pathways |
| Japanese BERT | BERT | 110M | Japanese medical text | Fine-tuning | NO | Report classification |
| Italian BERT | BERT | 110M | Italian clinical text | Fine-tuning | NO | CT report classification |
| BB-TEN | BigBird | 166M | TCGA pathology reports | Fine-tuning | NO | TNM staging |
| Domain-adapted LLM | Undisclosed | Undisclosed | Clinical progress notes | Domain adaptation | NO | Summarization |
| PEFT LLM | Undisclosed | Undisclosed | Radiology reports (MSKCC) | PEFT / LoRA | NO | Radiology summarization |

---

## Multimodal Vision-Language Models

| Model | Vision Encoder | Language Model | Parameters | Training Data | Open Source | Primary Task |
|-------|---------------|----------------|------------|---------------|-------------|-------------|
| LLaVA-Med | CLIP ViT-L/14 | LLaMA | ~7B | PMC-15M figure-captions | YES | Biomedical VQA |
| PMC-VQA (MedVInT) | PMC-CLIP | PMC-LLaMA | Undisclosed | PMC-VQA (227k pairs) | YES | Medical VQA |
| CH-ICL | BioMedCLIP + PubMedCLIP | GPT-3.5 | Undisclosed | PathVQA; VQA-RAD; SLAKE | NO | Medical VQA |
| MiniMedGPT | EVA-CLIP | LLaMA2-7B | ~7B | Medical VQA datasets | NO | Medical VQA |
| FAVP | ViT-G/14 + Q-Former | Vicuna-7B | ~7B | VQA-RAD; SLAKE; DME | YES | Generative VQA |
| CIF | CLIP ViT-B/16 | LLaMA 7B/13B | 7B / 13B | VQA-RAD; SLAKE; PathVQA | NO | Causal VQA |
| Falcon Med-VQA | Undisclosed | Falcon | Undisclosed | Medical VQA benchmarks | NO | Uncertainty-aware VQA |
| Flamingo-CXR | Flamingo vision | Flamingo | Undisclosed | MIMIC-CXR | NO | Radiology report generation |
| R2GenGPT | Swin Transformer | GPT-2 | ~117M | IU-Xray; MIMIC-CXR | YES | Report generation |
| BrainGPT | 3D CNN encoder | LLaMA-based | Undisclosed | 3D-BrainCT (18,885 scans) | YES | 3D CT report generation |
| MediVLM | Undisclosed | Undisclosed | Undisclosed | Radiology benchmarks | NO | Severity-aware reporting |
| MI-Gen | ViT (WSI encoder) | Transformer | Undisclosed | PathText/TCGA (9,000 WSIs) | NO | Pathology report generation |
| MIL + T5 | MIL encoder | T5 | Undisclosed | K-MEDICON 2024 (752 WSIs) | NO | Pathology report generation |
| GPT-4V | Undisclosed | GPT-4 | Undisclosed | Undisclosed | NO | CXR interpretation; Histopath |
| SkinGPT-4 | ViT | LLaMA-2-13B | ~13B | 52,929 skin images | YES | Dermatology diagnosis |
| M3FM | Undisclosed | Undisclosed | Undisclosed | 9 multilingual datasets | NO | Multimodal diagnosis |
| Claude 3.5 Sonnet | Undisclosed | Claude 3.5 | Undisclosed | Undisclosed | NO | Surgical decision support |

---

## LLM-Guided Segmentation Models

| Model | LLM Component | Segmentation Component | Role of LLM | Open Source | Dataset |
|-------|--------------|----------------------|-------------|-------------|---------|
| LLM4Seg | LLaMA3.2-1B / DeepSeek | CNN encoder-decoder | Frozen layer as semantic prior | YES | BUSI; ISIC; BTCV |
| MedVisionLlama | Llama-3.1-8B | ViT + LoRA | Residual attention enhancement | NO | Med. Seg. Decathlon |
| Zeus | Vicuna | SAM (Segment Anything) | Zero-shot instruction generation | NO | MSD-Brain; CHAOS |

---

## Adaptation Methods Summary

| Method | Description | Studies Using It |
|--------|-------------|-----------------|
| Pretraining from scratch | Train entirely on medical data | GatorTron, NYUTron, BioGPT |
| Domain-adaptive pretraining | Continue pretraining on medical corpus | BioBERT, BiomedRAG |
| Supervised fine-tuning (SFT) | Fine-tune on task-specific labeled data | ChatDoctor, Path-llama3.1 |
| Instruction tuning | Fine-tune on instruction-response pairs | Med-PaLM, Flan-T5, LLaVA-Med |
| PEFT / LoRA | Parameter-efficient adaptation | FAVP, MedVisionLlama, PEFT LLM |
| RAG | Retrieval-augmented generation | BiomedRAG, Hu et al. (gastric) |
| Zero-shot prompting | No fine-tuning; prompt engineering only | GPT-4 studies, Claude 3.5, Zeus |
| RLHF | Reinforcement learning from human feedback | GPT-4, Claude 3.5 |

---

## Open Source Availability Summary

| Status | Count | Models |
|--------|-------|--------|
| YES Fully open | 16 | GatorTron, BioBERT, BioGPT, BiomedRAG, Flan-T5, LLaVA-Med, PMC-VQA, FAVP, LLM4Seg, ChatDoctor, Mental-LLM, R2GenGPT, BrainGPT, SkinGPT-4, DeepSeek-based, LLaMA-based |
| NO Closed / proprietary | 20+ | GPT-4, GPT-3.5, Claude, Gemini, NYUTron, Flamingo-CXR, most clinical fine-tunes |
