# Multimodal Medical LLM Papers

Detailed reference for all multimodal studies included in the survey.
For the summary table see the main [README](../README.md).

---

## Radiology Report Generation

### R2GenGPT (2023)
- **Authors:** Wang et al.
- **Venue:** Meta-Radiology
- **Model:** R2GenGPT
- **Dataset:** IU-Xray, MIMIC-CXR
- **Key Results:** Competitive SOTA; only 5M trainable parameters
- **Validation:** Benchmark
- **Personalization:** Parameter-efficient domain transfer
- **Links:** [Paper](https://arxiv.org/abs/2309.09110) · [Code](https://github.com/wang-zhanyu/R2GenGPT)

### Flamingo-CXR (2024)
- **Authors:** Tanno et al.
- **Venue:** NPJ Digital Medicine
- **Model:** Flamingo-CXR
- **Dataset:** MIMIC-CXR; IND1 (prospective deployment)
- **Key Results:** 56.1% ICU preferable; 77.7% outpatient preferable
- **Validation:** Prospective
- **Personalization:** Longitudinal patient context integration
- **Links:** [Paper](#)

### BrainGPT (2025)
- **Authors:** Li et al.
- **Venue:** Nature Communications
- **Model:** BrainGPT (CVIT)
- **Dataset:** 3D-BrainCT (18,885 scans)
- **Key Results:** FORTE F1 0.71; 74% Turing indistinguishability pass
- **Validation:** Internal + External
- **Personalization:** 3D volumetric report synthesis
- **Links:** [Paper](https://www.nature.com/articles/s41467-025-57426-0) · [Code](https://doi.org/10.5281/zenodo.14852686)

### MediVLM (2025)
- **Authors:** Goswami et al.
- **Venue:** arXiv
- **Model:** MediVLM
- **Dataset:** 3 radiology benchmarks
- **Key Results:** Annotation-free with severity scoring
- **Validation:** Benchmark
- **Personalization:** Unsupervised severity-aware reporting
- **Links:** [Paper](#)

---

## Pathology Report Generation

### MI-Gen (2024)
- **Authors:** Chen et al.
- **Venue:** Medical Image Analysis
- **Model:** MI-Gen
- **Dataset:** PathText/TCGA (~9,000 WSI-text pairs)
- **Key Results:** BRCA subtyping F1 0.838
- **Validation:** Internal
- **Personalization:** Gigapixel WSI multi-instance report generation
- **Links:** [Paper](#)

### RAG-based Gastric Pathology (2025)
- **Authors:** Hu et al.
- **Venue:** Computers in Biology and Medicine
- **Model:** Proposed method
- **Dataset:** GastricADC (991 WSIs); Gastric-3300 (3,309 WSIs)
- **Key Results:** ROUGE-L 0.690 (Gastric-3300); 0.568 (GastricADC)
- **Validation:** Internal + External
- **Personalization:** Retrieval-augmented historical case referencing
- **Links:** [Paper](#)

### MIL + T5 Bladder Reports (2025)
- **Authors:** Kim et al.
- **Venue:** MICCAI 2025
- **Model:** MIL + T5 (modular)
- **Dataset:** K-MEDICON 2024 (752 bladder WSIs)
- **Key Results:** ROUGE 0.87; BLEU-4 0.94
- **Validation:** Internal
- **Personalization:** Structured label-conditioned report generation
- **Links:** [Paper](#)

---

## Medical Visual Question Answering

### LLaVA-Med (2023)
- **Authors:** Li et al.
- **Venue:** NeurIPS 2023
- **Model:** LLaVA-Med
- **Dataset:** PMC-15M (biomedical figure-captions)
- **Key Results:** Outperforms supervised SOTA on VQA metrics
- **Validation:** Benchmark
- **Personalization:** Instruction-tuned biomedical multimodal assistant
- **Links:** [Paper](https://arxiv.org/abs/2306.00890) · [Code](https://github.com/microsoft/LLaVA-Med)

### PMC-VQA (2024)
- **Authors:** Zhang et al.
- **Venue:** Communications Medicine
- **Model:** PMC-VQA (PMC-CLIP + PMC-LLaMA)
- **Dataset:** PMC-VQA (227k pairs, 149k images)
- **Key Results:** SOTA on VQA-RAD, SLAKE, ImageClef-2019
- **Validation:** Benchmark
- **Personalization:** Open-ended generative response over fixed answer sets
- **Links:** [Paper](https://www.nature.com/articles/s43856-024-00709-2) · [Code](https://github.com/xiaoman-zhang/PMC-VQA)

### CH-ICL (2024)
- **Authors:** Liang et al.
- **Venue:** arXiv
- **Model:** CH-ICL (BioMedCLIP + PubMedCLIP)
- **Dataset:** PathVQA, VQA-RAD, SLAKE
- **Key Results:** VQA-RAD 74.28%/77.08%; SLAKE 82.19%/88.12%
- **Validation:** Benchmark
- **Personalization:** Knowledge-scope-guided retrieval for domain reasoning
- **Links:** [Paper](https://arxiv.org/abs/2408.10048)

### Falcon Med-VQA (2024)
- **Authors:** Bawazir et al.
- **Venue:** arXiv
- **Model:** Falcon Med-VQA
- **Dataset:** Medical VQA benchmarks
- **Key Results:** Confidence scores with explainability
- **Validation:** Benchmark
- **Personalization:** Uncertainty-aware clinical QA
- **Links:** [Paper](#)

### MiniMedGPT (2025)
- **Authors:** Alsabbagh et al.
- **Venue:** arXiv
- **Model:** MiniMedGPT (EVA-CLIP + LLaMA2-7B)
- **Dataset:** VQA-RAD, SLAKE
- **Key Results:** Competitive SOTA; fewest trainable params among 6 models
- **Validation:** Benchmark
- **Personalization:** Efficient parameter adaptation for resource-constrained deployment
- **Links:** [Paper](#)

### FAVP (2025)
- **Authors:** Yu et al.
- **Venue:** AAAI 2025
- **Model:** FAVP (ViT-G/14 + Vicuna-7B)
- **Dataset:** VQA-RAD, SLAKE, DME
- **Key Results:** SOTA on generative open-set VQA-RAD and SLAKE
- **Validation:** Benchmark
- **Personalization:** Organ-adaptive region-level visual prompts
- **Links:** [Paper](https://github.com/OpenMICG/FAVP) · [Code](https://github.com/OpenMICG/FAVP)

### CIF — Causal Inference Framework (2025)
- **Authors:** Xu et al.
- **Venue:** IEEE Transactions
- **Model:** CIF (CLIP ViT-B/16 + LLaMA 7B/13B)
- **Dataset:** VQA-RAD, SLAKE, PathVQA, PMC-VQA, ProbMed
- **Key Results:** Significant accuracy improvement across five datasets
- **Validation:** Benchmark
- **Personalization:** Causal deconfounding of image-question bias
- **Links:** [Paper](#)

---

## LLM-Guided Image Segmentation

### LLM4Seg (2025)
- **Authors:** Tang et al.
- **Venue:** arXiv
- **Model:** LLM4Seg (LLaMA3.2-1B / DeepSeek)
- **Dataset:** BUSI, TNSCUI, ISIC, Kvasir, BTCV
- **Key Results:** SOTA across 2D/3D modalities; minimal trainable params
- **Validation:** Internal
- **Personalization:** Generalizable LLM semantic priors across imaging modalities
- **Links:** [Paper](#) · [Code](#)
- **Note:** LLM functions as semantic prior; segmentation decoder performs pixel-level inference

### MedVisionLlama (2025)
- **Authors:** Kumar et al.
- **Venue:** arXiv
- **Model:** MedVisionLlama (Llama-3.1-8B + ViT)
- **Dataset:** Medical Segmentation Decathlon (10 tasks)
- **Key Results:** Improved Dice, Jaccard, HD95 over ViT baseline
- **Validation:** Internal
- **Personalization:** LLM-enhanced attention for data-efficient 3D segmentation
- **Links:** [Paper](#)
- **Note:** LLM provides attention priors; metrics reflect full pipeline performance

### Zeus (2025)
- **Authors:** Dai et al.
- **Venue:** arXiv
- **Model:** Zeus (Vicuna + SAM)
- **Dataset:** MSD-Brain, MSD-Prostate, CHAOS
- **Key Results:** Superior to influential baselines across multimodal settings
- **Validation:** Internal
- **Personalization:** Zero-shot LLM instruction generation without paired VL data
- **Links:** [Paper](#)
- **Note:** LLM generates instructions; SAM performs segmentation

---

## Multimodal Diagnosis & Clinical Reasoning

### M3FM (2025)
- **Authors:** Liu et al.
- **Venue:** arXiv
- **Model:** M3FM
- **Dataset:** 9 datasets; CXR + CT; English + Chinese
- **Key Results:** Zero-shot across 16 disease categories and two languages
- **Validation:** Benchmark
- **Personalization:** Rare disease and non-English population coverage
- **Links:** [Paper](#)

### GPT-4V Chest X-ray (2024)
- **Authors:** Zhou et al.
- **Venue:** Radiology
- **Model:** GPT-4V
- **Dataset:** 100 CXR (50 NIH, 50 MIDRC)
- **Key Results:** Zero-shot F1: 7.3% (NIH), 18.2% (MIDRC)
- **Validation:** Internal
- **Personalization:** Dataset-specific deployment context sensitivity
- **Links:** [Paper](#)

### Claude 3.5 Laryngeal Cancer (2025)
- **Authors:** Liang et al.
- **Venue:** Head & Neck
- **Model:** Claude 3.5 Sonnet (+ 5 MLLMs)
- **Dataset:** 169 images; 1,084 questions; 50 laryngeal cancer patients
- **Key Results:** 79.43% accuracy (95% CI: 77.02–81.84%)
- **Validation:** Internal
- **Personalization:** Multi-modality surgical decision support
- **Links:** [Paper](#)

### GPT-4V Histopathology (2024)
- **Authors:** Ferber et al.
- **Venue:** Nature Medicine
- **Model:** GPT-4V (in-context learning)
- **Dataset:** CRC100K; MHIST; PatchCamelyon
- **Key Results:** Matches or outperforms specialist networks; no parameter updates
- **Validation:** Benchmark
- **Personalization:** Annotation-free deployment for non-technical clinicians
- **Links:** [Paper](https://arxiv.org/abs/2312.02510)

### SkinGPT-4 (2024)
- **Authors:** Zhou et al.
- **Venue:** Nature Communications
- **Model:** SkinGPT-4 (LLaMA-2-13B + ViT)
- **Dataset:** 52,929 skin disease images + clinical notes; 150 real cases
- **Key Results:** Autonomous diagnosis confirmed by dermatologists
- **Validation:** Internal
- **Personalization:** Patient-uploaded photographs for point-of-care dermatology
- **Links:** [Paper](https://arxiv.org/abs/2304.10691) · [Code](https://github.com/JoshuaChou2018/SkinGPT-4)