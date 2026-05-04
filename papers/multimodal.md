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
- **Links:** [Paper](https://www.sciencedirect.com/science/article/pii/S2950162823000334) · 
[Code](https://github.com/wang-zhanyu/R2GenGPT)

### LLaVA-Med (2023)
- **Authors:** Li et al.
- **Venue:** NeurIPS 2023
- **Model:** LLaVA-Med (CLIP ViT + Vicuna/LLaMA)
- **Dataset:** PMC-15M (biomedical figure–captions)
- **Key Results:** Outperforms supervised SOTA on biomedical VQA metrics
- **Validation:** Benchmark
- **Personalization:** Instruction-tuned biomedical multimodal assistant
- **Links:** [Paper](https://neurips.cc/virtual/2023/poster/73643) · 
[Code](https://github.com/microsoft/LLaVA-Med)

### MAIRA-2 (2024)
- **Authors:** Yuan et al.
- **Venue:** arXiv
- **Model:** MAIRA-2 (region-grounded VLM)
- **Dataset:** MIMIC-CXR
- **Key Results:** Grounded radiology report generation with spatial localization
- **Validation:** Benchmark
- **Personalization:** Region-level grounded findings generation
- **Links:** [Paper](https://arxiv.org/abs/2406.04449)

### Flamingo-CXR (2024)
- **Authors:** Tanno et al.
- **Venue:** Nature Medicine
- **Model:** Flamingo-CXR (clinician-in-loop)
- **Dataset:** MIMIC-CXR; IND1 (prospective deployment)
- **Key Results:** 56.1% ICU preferable; 77.7% outpatient preferable
- **Validation:** Prospective
- **Personalization:** Longitudinal patient context integration
- **Links:** [Paper](https://www.nature.com/articles/s41591-024-03302-1)

### BrainGPT (2025)
- **Authors:** Li et al.
- **Venue:** Nature Communications
- **Model:** BrainGPT (CVIT-based)
- **Dataset:** 3D-BrainCT (18,885 scans)
- **Key Results:** FORTE F1 0.71; 74% Turing indistinguishability pass
- **Validation:** Internal + External
- **Personalization:** 3D volumetric report synthesis
- **Links:** [Paper](https://www.nature.com/articles/s41467-025-57426-0) · 
[Code](https://doi.org/10.5281/zenodo.14852686)

### MediVLM (2025)
- **Authors:** Goswami et al.
- **Venue:** ACL Anthology (EMNLP Findings)
- **Model:** MediVLM
- **Dataset:** 3 radiology benchmarks
- **Key Results:** Annotation-free with severity scoring
- **Validation:** Benchmark
- **Personalization:** Unsupervised severity-aware reporting
- **Links:** [Paper](https://aclanthology.org/2025.findings-emnlp.544/)

---

## Pathology Report Generation

### WsiCaption — MI-Gen (2024)
- **Authors:** Chen et al.
- **Venue:** MICCAI 2024
- **Model:** MI-Gen (multiple-instance generation)
- **Dataset:** PathText/TCGA (~9,000 WSI–text pairs)
- **Key Results:** BRCA subtyping F1 0.838
- **Validation:** Internal
- **Personalization:** Gigapixel WSI multi-instance report generation
- **Links:** [Paper](https://link.springer.com/chapter/10.1007/978-3-031-72083-3_51) · 
[Code](https://github.com/cpystan/Wsi-Caption)

### HistGen (2024)
- **Authors:** Shi et al.
- **Venue:** MICCAI 2024
- **Model:** HistGen (local-global feature encoding + cross-modal context)
- **Dataset:** TCGA histopathology WSIs
- **Key Results:** Improved BLEU and ROUGE over prior report generation baselines
- **Validation:** Internal
- **Personalization:** Local-global hierarchical feature fusion for WSI reporting
- **Links:** [Paper](https://link.springer.com/chapter/10.1007/978-3-031-72083-3_18) · 
[Code](https://github.com/dddavid4real/HistGen)

### Clinical-Grade Multi-organ VLM (2024)
- **Authors:** Chen et al.
- **Venue:** MICCAI 2024
- **Model:** Semantically Guided Medical Text Foundation Model
- **Dataset:** Multi-organ TCGA WSIs
- **Key Results:** Clinical-grade reporting across multiple organ types
- **Validation:** Internal
- **Personalization:** Semantically guided multi-organ report synthesis
- **Links:** [Paper](https://link.springer.com/chapter/10.1007/978-3-031-72083-3_3) · 
[Code](https://github.com/hvcl/Clinical-grade-Pathology-Report-Generation/tree/main)

### Multi-level Regional + LLM Refinement (2025)
- **Authors:** (Multi-level Regional)
- **Venue:** Computer Methods and Programs in Biomedicine
- **Model:** Multi-level regional feature selection + LLM refinement
- **Dataset:** TCGA WSIs
- **Key Results:** Improved report generation via knowledge retrieval and 
regional feature selection
- **Validation:** Internal
- **Links:** [Paper](https://www.sciencedirect.com/science/article/pii/S016926072500094X)

### TITAN (2025)
- **Authors:** Shaikovski et al.
- **Venue:** Nature Medicine
- **Model:** TITAN (CONCH + Transformer)
- **Dataset:** TCGA multi-cancer WSIs
- **Key Results:** Multimodal whole-slide foundation model; SOTA across 
pathology generation and retrieval tasks
- **Validation:** Benchmark
- **Personalization:** Whole-slide foundation model for diverse cancer types
- **Links:** [Paper](https://www.nature.com/articles/s41591-025-03982-3) · 
[Code](https://github.com/mahmoodlab/TITAN)

### PolyPath — Gemini 1.5 Flash (2025)
- **Authors:** (PolyPath)
- **Venue:** Modern Pathology
- **Model:** Gemini 1.5 Flash (1M-token context)
- **Dataset:** Multi-slide pathology cases
- **Key Results:** Multi-slide pathology report generation using 1M-token 
context window
- **Validation:** Internal
- **Personalization:** Long-context multi-slide reasoning for complex cases
- **Links:** [Paper](https://www.sciencedirect.com/science/article/pii/S089339522500184X)

### MIL + T5 Bladder Reports (2025)
- **Authors:** Kim et al.
- **Venue:** IEEE Access
- **Model:** MIL + T5 (modular pipeline)
- **Dataset:** K-MEDICON 2024 (752 bladder WSIs)
- **Key Results:** ROUGE 0.87; BLEU-4 0.94
- **Validation:** Internal
- **Personalization:** Structured label-conditioned report generation
- **Links:** [Paper](https://ieeexplore.ieee.org/abstract/document/11078283)

### RAG-based Gastric Pathology (2025)
- **Authors:** Hu et al.
- **Venue:** Computers in Biology and Medicine
- **Model:** RAG + LLM pipeline
- **Dataset:** GastricADC (991 WSIs); Gastric-3300 (3,309 WSIs)
- **Key Results:** ROUGE-L 0.690 (Gastric-3300); 0.568 (GastricADC)
- **Validation:** Internal + External
- **Personalization:** Retrieval-augmented historical case referencing
- **Links:** [Paper](https://www.sciencedirect.com/science/article/pii/S016926072500094X)

---

## Medical Visual Question Answering

### LLaVA-Med (2023)
- **Authors:** Li et al.
- **Venue:** NeurIPS 2023
- **Model:** LLaVA-Med
- **Dataset:** PMC-15M (biomedical figure–captions)
- **Key Results:** Outperforms supervised SOTA on VQA metrics
- **Validation:** Benchmark
- **Personalization:** Instruction-tuned biomedical multimodal assistant
- **Links:** [Paper](https://arxiv.org/abs/2306.00890) · 
[Code](https://github.com/microsoft/LLaVA-Med)

### PMC-VQA (2024)
- **Authors:** Zhang et al.
- **Venue:** Communications Medicine
- **Model:** PMC-VQA (PMC-CLIP + PMC-LLaMA)
- **Dataset:** PMC-VQA (227k pairs, 149k images)
- **Key Results:** SOTA on VQA-RAD, SLAKE, ImageClef-2019
- **Validation:** Benchmark
- **Personalization:** Open-ended generative response over fixed answer sets
- **Links:** [Paper](https://www.nature.com/articles/s43856-024-00709-2) · 
[Code](https://github.com/xiaoman-zhang/PMC-VQA)

### CH-ICL (2024)
- **Authors:** Liang et al.
- **Venue:** Information Processing & Management
- **Model:** CH-ICL (BioMedCLIP + PubMedCLIP)
- **Dataset:** PathVQA, VQA-RAD, SLAKE
- **Key Results:** VQA-RAD 74.28% / 77.08%; SLAKE 82.19% / 88.12%
- **Validation:** Benchmark
- **Personalization:** Knowledge-scope-guided retrieval for domain reasoning
- **Links:** [Paper](https://www.sciencedirect.com/science/article/pii/S030645732400164X)

### OmniMedVQA (2024)
- **Authors:** Hu et al.
- **Venue:** CVPR 2024
- **Model:** Evaluation benchmark (12 modalities)
- **Dataset:** Large-scale multi-modality medical VQA benchmark
- **Key Results:** Comprehensive evaluation of medical LVLMs across 12 imaging 
modalities and diverse disease types
- **Validation:** Benchmark
- **Links:** [Paper](https://openaccess.thecvf.com/content/CVPR2024/papers/Hu_OmniMedVQA_A_New_Large-Scale_Comprehensive_Evaluation_Benchmark_for_Medical_LVLM_CVPR_2024_paper.pdf)

### Falcon Med-VQA (2024)
- **Authors:** Bawazir et al.
- **Venue:** Proceedings of the AAAI Conference on Artificial Intelligence
- **Model:** Falcon Med-VQA
- **Dataset:** Medical VQA benchmarks
- **Key Results:** Uncertainty-aware QA with confidence scores and explainability
- **Validation:** Benchmark
- **Personalization:** Uncertainty-aware clinical QA
- **Links:** [Paper](https://ojs.aaai.org/index.php/AAAI/article/view/35346)

### MiniMedGPT (2025)
- **Authors:** Alsabbagh et al.
- **Venue:** Pattern Recognition Letters
- **Model:** MiniMedGPT (EVA-CLIP + LLaMA2-7B)
- **Dataset:** VQA-RAD, SLAKE
- **Key Results:** Competitive SOTA; fewest trainable params among 6 models
- **Validation:** Benchmark
- **Personalization:** Efficient parameter adaptation for resource-constrained 
deployment
- **Links:** [Paper](https://www.sciencedirect.com/science/article/pii/S0167865525000017)

### FAVP (2025)
- **Authors:** Yu et al.
- **Venue:** AAAI 2025
- **Model:** FAVP (ViT-G/14 + Vicuna-7B)
- **Dataset:** VQA-RAD, SLAKE, DME
- **Key Results:** SOTA on generative open-set VQA-RAD and SLAKE
- **Validation:** Benchmark
- **Personalization:** Organ-adaptive region-level visual prompts
- **Links:** [Paper](https://github.com/OpenMICG/FAVP) · 
[Code](https://github.com/OpenMICG/FAVP)

### CIF — Causal Inference Framework (2025)
- **Authors:** ...
- **Venue:** IEEE Transactions
- **Model:** CIF (CLIP ViT-B/16 + LLaMA 7B/13B)
- **Dataset:** VQA-RAD, SLAKE, PathVQA, PMC-VQA, ProbMed
- **Key Results:** Significant accuracy improvement across five datasets
- **Validation:** Benchmark
- **Personalization:** Causal deconfounding of image–question bias
- **Links:** [Paper](https://arxiv.org/html/2512.09433v2)

---

## LLM-Guided Image Segmentation

### LLM4Seg (2025)
- **Authors:** Tang et al.
- **Venue:** MICCAI 2025
- **Model:** LLM4Seg (frozen LLaMA3.2-1B or DeepSeek layer + CNN encoder-decoder)
- **Dataset:** BUSI, TNSCUI, ISIC, Kvasir, BTCV
- **Key Results:** SOTA across 2D/3D modalities; minimal trainable params
- **Validation:** Internal
- **Personalization:** Generalizable LLM semantic priors across imaging modalities
- **Links:** [Paper](https://link.springer.com/chapter/10.1007/978-3-032-05127-1_39) · 
[Code](https://github.com/FengheTan9/LLM4Seg)
- **Note:** LLM functions as semantic prior; segmentation decoder performs 
pixel-level inference

### MedVisionLlama (2025)
- **Authors:** Kumar et al.
- **Venue:** ICCV 2025 Workshop (CVAMD)
- **Model:** MedVisionLlama (frozen Llama-3.1-8B blocks + ViT encoder; LoRA)
- **Dataset:** Medical Segmentation Decathlon (10 tasks)
- **Key Results:** Improved Dice, Jaccard, HD95 over ViT baseline
- **Validation:** Internal
- **Personalization:** LLM-enhanced attention for data-efficient 3D segmentation
- **Links:** [Paper](https://arxiv.org/abs/2410.02458) · 
[Code](https://github.com/AS-Lab/Marthi-et-al-2025-MedVisionLlama-Pre-Trained-LLM-Layers-to-Enhance-Medical-Image-Segmentation)
- **Note:** LLM provides attention priors; metrics reflect full pipeline performance

### Zeus (2025)
- **Authors:** Dai et al.
- **Venue:** International Journal of Machine Learning and Cybernetics
- **Model:** Zeus (frozen Vicuna as instruction generator + SAM mask decoder)
- **Dataset:** MSD-Brain, MSD-Prostate, CHAOS
- **Key Results:** Superior to influential baselines across multimodal settings
- **Validation:** Internal
- **Personalization:** Zero-shot LLM instruction generation without paired VL data
- **Links:** [Paper](https://link.springer.com/article/10.1007/s13042-025-02742-6)
- **Note:** LLM generates instructions; SAM performs segmentation

### HCR — LLM Clinical Guardrails (2025)
- **Authors:** (HCR)
- **Venue:** arXiv
- **Model:** HCR (Gemini 2.5 Flash; hierarchical multi-stage prompting)
- **Dataset:** Medical image segmentation benchmarks
- **Key Results:** LLM-based clinical guardrails improve segmentation reliability 
beyond pixel agreement
- **Validation:** Benchmark
- **Personalization:** Hierarchical clinical consistency checking for safe deployment
- **Links:** [Paper](https://arxiv.org/abs/2506.01841)
- **Note:** LLM acts as clinical validator; segmentation model performs pixel inference

---

## Multimodal Clinical Diagnosis & Reasoning

### GPT-4V Chest X-Ray (2024)
- **Authors:** Zhou et al.
- **Venue:** Radiology: Artificial Intelligence
- **Model:** GPT-4V (zero-shot / few-shot)
- **Dataset:** 100 CXR (50 NIH, 50 MIDRC)
- **Key Results:** Zero-shot F1: 7.3% (NIH), 18.2% (MIDRC)
- **Validation:** Internal
- **Personalization:** Dataset-specific deployment context sensitivity
- **Links:** [Paper](https://pubmed.ncbi.nlm.nih.gov/38713028/)

### GPT-4V Histopathology (2024)
- **Authors:** Ferber et al.
- **Venue:** Nature Communications
- **Model:** GPT-4V (in-context learning; no fine-tuning)
- **Dataset:** CRC100K; MHIST; PatchCamelyon
- **Key Results:** Matches or outperforms specialist networks; no parameter updates
- **Validation:** Benchmark
- **Personalization:** Annotation-free deployment for non-technical clinicians
- **Links:** [Paper](https://www.nature.com/articles/s41467-024-51465-9) · 
[Code](https://github.com/Dyke-F/GPT-4V-In-Context-Learning)

### SkinGPT-4 (2024)
- **Authors:** Zhou et al.
- **Venue:** Nature Communications
- **Model:** SkinGPT-4 (LLaMA-2-13B + ViT)
- **Dataset:** 52,929 skin disease images + clinical notes; 150 real cases
- **Key Results:** Autonomous diagnosis confirmed by dermatologists
- **Validation:** Internal
- **Personalization:** Patient-uploaded photographs for point-of-care dermatology
- **Links:** [Paper](https://www.nature.com/articles/s41467-024-50043-3) · 
[Code](https://github.com/JoshuaChou2018/SkinGPT-4)

### PathChat (2024)
- **Authors:** Shaikovski et al.
- **Venue:** Nature
- **Model:** PathChat (UNI ViT + LLaMA 13B; projection fusion)
- **Dataset:** Pathology images + clinical QA pairs
- **Key Results:** Multimodal generative AI copilot for human pathology
- **Validation:** Benchmark + Clinician evaluation
- **Personalization:** Pathology-specific multimodal dialogue
- **Links:** [Paper](https://www.nature.com/articles/s41586-024-07618-3) · 
[Code](https://github.com/fedshyvana/pathology_mllm_training)

### Med-PaLM M (2024)
- **Authors:** Tu et al.
- **Venue:** NEJM AI
- **Model:** Med-PaLM M (PaLM-E + ViT; 14-task unified)
- **Dataset:** 14 biomedical tasks across imaging and text
- **Key Results:** Generalist biomedical AI; SOTA across radiology, 
pathology, genomics, and clinical NLP tasks
- **Validation:** Benchmark
- **Personalization:** Unified generalist model covering rare and 
multi-domain clinical tasks
- **Links:** [Paper](https://ai.nejm.org/doi/full/10.1056/AIoa2300138)

### LLMSeg — Radiation Oncology Contouring (2024)
- **Authors:** Shi et al.
- **Venue:** Nature Communications
- **Model:** LLMSeg (3D CT + clinical text; cross-attention)
- **Dataset:** Radiation oncology CT volumes + clinical reports
- **Key Results:** LLM-driven multimodal target volume contouring 
outperforms image-only baselines
- **Validation:** Internal
- **Personalization:** Clinical-text-guided contouring for patient-specific 
treatment planning
- **Links:** [Paper](https://www.nature.com/articles/s41467-024-53387-y) · 
[Code](https://github.com/tvseg/MM-LLM-RO)

### M3FM (2025)
- **Authors:** Liu et al.
- **Venue:** npj Digital Medicine
- **Model:** M3FM (multimodal multidomain multilingual)
- **Dataset:** 9 datasets; CXR + CT; English + Chinese
- **Key Results:** Zero-shot across 16 disease categories and two languages
- **Validation:** Benchmark
- **Personalization:** Rare disease and non-English population coverage
- **Links:** [Paper](https://www.nature.com/articles/s41746-024-01339-7)

### Claude 3.5 Laryngeal Cancer (2025)
- **Authors:** Liang et al.
- **Venue:** International Journal of Surgery
- **Model:** Claude 3.5 Sonnet (+ 5 MLLMs)
- **Dataset:** 169 images; 1,084 questions; 50 laryngeal cancer patients
- **Key Results:** 79.43% accuracy (95% CI: 77.02–81.84%)
- **Validation:** Internal
- **Personalization:** Multi-modality surgical decision support
- **Links:** [Paper](https://journals.lww.com/international-journal-of-surgery/fulltext/2025/03000/multimodal_large_language_models_address_clinical.36.aspx)

### MedTVT-R1 (2025)
- **Authors:** (MedTVT-R1)
- **Venue:** arXiv
- **Model:** MedTVT-R1 (LLaMA3.2 + ECG + CXR + Lab; adaptive 
cross-modal attention)
- **Dataset:** Multi-modal EHR (ECG, CXR, lab values)
- **Key Results:** Multimodal LLM empowering medical reasoning and diagnosis 
across heterogeneous clinical inputs
- **Validation:** Benchmark
- **Personalization:** Adaptive cross-modal attention for patient-specific 
physiological reasoning
- **Links:** [Paper](https://arxiv.org/abs/2506.18512) · 
[Code](https://github.com/keke-nice/MedTVT-R1)

### MEDFuse (2024)
- **Authors:** (MEDFuse)
- **Venue:** CIKM 2024
- **Model:** MEDFuse (lab-test transformer + LLM notes; cross-attention 
intermediate fusion)
- **Dataset:** MIMIC-III EHR (lab tests + clinical notes)
- **Key Results:** Multimodal EHR fusion with masked lab-test modeling 
outperforms unimodal baselines
- **Validation:** Benchmark
- **Personalization:** Masked lab-test modeling for missing data robustness
- **Links:** [Paper](https://dl.acm.org/doi/10.1145/3627673.3679962)

### SMFusion (2025)
- **Authors:** (SMFusion)
- **Venue:** IEEE JBHI
- **Model:** SMFusion (BiomedGPT text + cross-attention + PET/MRI)
- **Dataset:** PET/MRI multi-modal clinical imaging
- **Key Results:** Semantic-preserving fusion of multimodal medical images 
for enhanced clinical diagnosis
- **Validation:** Internal
- **Personalization:** Semantically guided cross-modal fusion for 
multi-scanner clinical data
- **Links:** [Paper](https://ieeexplore.ieee.org/abstract/document/11319543)