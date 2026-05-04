# Text-Based Medical LLM Papers

Detailed reference for all text-based studies included in the survey.
For the summary table see the main [README](../README.md).

---

## Clinical Documentation & Information Extraction

### GatorTron (2022)
- **Authors:** Yang et al.
- **Venue:** npj Digital Medicine
- **Model:** GatorTron (8.9B parameters)
- **Dataset:** UF Health EHR (90B tokens; 82B clinical)
- **Key Results:** +9.6% NLI, +9.5% MQA accuracy over prior SOTA
- **Validation:** Internal
- **Personalization:** Institution-level EHR adaptation
- **Links:** [Paper](https://www.nature.com/articles/s41746-022-00742-2) · 
[Code](https://github.com/uf-hobi-informatics-lab/GatorTron)

### NYUTron (2023)
- **Authors:** Jiang et al.
- **Venue:** Nature
- **Model:** NYUTron
- **Dataset:** 387,144 patients (NYU Langone EHR)
- **Key Results:** AUC 78.7–94.9% across five clinical outcomes
- **Validation:** Internal + Prospective
- **Personalization:** All-purpose prediction from patient notes
- **Links:** [Paper](https://www.nature.com/articles/s41586-023-06160-y) · 
[Code](https://github.com/nyuolab/NYUTron)

### Flan-T5 for SDoH Profiling (2024)
- **Authors:** Guevara et al.
- **Venue:** npj Digital Medicine
- **Model:** Flan-T5 XL/XXL
- **Dataset:** Multi-site EHR clinical notes
- **Key Results:** Macro-F1 0.71; 93.8% vs 2.0% ICD-10 code accuracy
- **Validation:** Internal
- **Personalization:** Patient SDoH profiling; reduced demographic bias (p<0.05)
- **Links:** [Paper](https://www.nature.com/articles/s41746-023-00970-0) · 
[Code](https://github.com/AIM-Harvard/SDoH)

### Hybrid LLM for Treatment Pathways (2025)
- **Authors:** Tariq et al.
- **Venue:** Journal of Biomedical Informatics
- **Model:** Hybrid LLM (UMLS + fine-tuned)
- **Dataset:** Mayo Clinic / Stanford (26,692 + 162 patients)
- **Key Results:** AUROC 0.942 internal; 0.924 external
- **Validation:** External
- **Personalization:** Individual treatment pathway reconstruction
- **Links:** [Paper](https://ascopubs.org/doi/full/10.1200/CCI-25-00002)

### GPT-4 German Discharge Extraction (2025)
- **Authors:** Siepmann et al.
- **Venue:** Healthcare Analytics
- **Model:** GPT-4
- **Dataset:** German discharge letters (20 pts, 2 sites)
- **Key Results:** 85% → 95% primary diagnosis accuracy post prompt tuning
- **Validation:** Internal
- **Personalization:** Multilingual discharge record extraction
- **Links:** [Paper](https://www.sciencedirect.com/science/article/pii/S2772442524000807)

---

## Biomedical Literature Mining & Knowledge Synthesis

### BioBERT (2020)
- **Authors:** Lee et al.
- **Venue:** Bioinformatics
- **Model:** BioBERT
- **Dataset:** PubMed/PMC (18B tokens)
- **Key Results:** Token-F1 0.9003 (disease NER, BC5CDR)
- **Validation:** Benchmark
- **Personalization:** Evidence-grounded clinical recommendations
- **Links:** [Paper](https://academic.oup.com/bioinformatics/article/36/4/1234/5566506) · 
[Code](https://github.com/dmis-lab/biobert)

### BioGPT (2022)
- **Authors:** Luo et al.
- **Venue:** Briefings in Bioinformatics
- **Model:** BioGPT
- **Dataset:** PubMed abstracts (15M)
- **Key Results:** F1 44.98% BC5CDR; 78.2% PubMedQA accuracy
- **Validation:** Benchmark
- **Personalization:** Generative biomedical knowledge synthesis
- **Links:** [Paper](https://academic.oup.com/bib/article/23/6/bbac409/6713511) · 
[Code](https://github.com/microsoft/BioGPT)

### BiomedRAG (2025)
- **Authors:** Li et al.
- **Venue:** Journal of Biomedical Informatics
- **Model:** BiomedRAG (LLaMA2 / MedLLaMA-13B)
- **Dataset:** Eight biomedical NLP datasets
- **Key Results:** +9.95% over base LLMs; +4.97% over RAG baselines
- **Validation:** Benchmark
- **Personalization:** Precision-grounded evidence retrieval
- **Links:** [Paper](https://www.sciencedirect.com/science/article/pii/S1532046424001874) · 
[Code](https://github.com/ToneLi/BIoMedRAG/tree/main)

### LORE — Disease–Gene Association Prediction (2025)
- **Authors:** Liu et al.
- **Venue:** Briefings in Bioinformatics
- **Model:** LORE (GPT-3.5-turbo + text-embedding-3-large)
- **Dataset:** Literature-derived disease–gene associations (PubMed)
- **Key Results:** LLM-driven framework outperforms prior literature mining baselines
- **Validation:** Benchmark
- **Personalization:** Literature-based knowledge retrieval for gene–disease reasoning
- **Links:** [Paper](https://doi.org/10.1093/bib/bbaf070) · 
[Code](https://github.com/ailabstw/LORE)

---

## Clinical Decision Support & Question Answering

### Med-PaLM (2023)
- **Authors:** Singhal et al.
- **Venue:** Nature
- **Model:** Med-PaLM (Flan-PaLM)
- **Dataset:** MultiMedQA
- **Key Results:** 67.6% MedQA; 92.6% clinician agreement rate
- **Validation:** Benchmark
- **Personalization:** Safety-aligned QA with clinician-level consensus
- **Links:** [Paper](https://www.nature.com/articles/s41586-023-06291-2)

### GPT-4 on USMLE (2023)
- **Authors:** Nori et al.
- **Venue:** arXiv
- **Model:** GPT-4
- **Dataset:** USMLE / MedQA
- **Key Results:** 86.7% MedQA; 20+ pts above passing threshold
- **Validation:** Benchmark
- **Personalization:** Calibrated uncertainty; personalized explanations
- **Links:** [Paper](https://arxiv.org/abs/2311.16452)

### ChatDoctor (2023)
- **Authors:** Li et al.
- **Venue:** Cureus
- **Model:** ChatDoctor (LLaMA-7B)
- **Dataset:** 100K patient–physician dialogues
- **Key Results:** Improved patient inquiry understanding
- **Validation:** Internal
- **Personalization:** Personalized patient dialogue adaptation
- **Links:** [Paper](https://assets.cureus.com/uploads/original_article/pdf/152858/20230724-24731-1v47a9.pdf) · 
[Code](https://github.com/Kent0n-Li/ChatDoctor)

### GPT-4 Surgical Knowledge Assessment (2024)
- **Authors:** Evaluating capabilities of large language models (LLMs)
- **Venue:** Surgery
- **Model:** GPT-4
- **Dataset:** Surgical board examination questions
- **Key Results:** GPT-4 achieves passing-level performance on surgical knowledge assessments
- **Validation:** Benchmark
- **Personalization:** Domain-specific QA for surgical education
- **Links:** [Paper](https://www.sciencedirect.com/science/article/pii/S0039606023009546)

### Mental-LLM (2024)
- **Authors:** Xu et al.
- **Venue:** ACM SIGCHI
- **Model:** Mental-LLM
- **Dataset:** Reddit mental health datasets
- **Key Results:** +10.9% accuracy over GPT-3.5
- **Validation:** Benchmark
- **Personalization:** Individual mental health state monitoring
- **Links:** [Paper](https://dl.acm.org/doi/pdf/10.1145/3643540) · 
[Code](https://github.com/neuhai/Mental-LLM)

### GPT-4 Radiology Patient Education (2025)
- **Authors:** Einspänner et al.
- **Venue:** Healthcare Analytics
- **Model:** GPT-4
- **Dataset:** Radiology consent forms (CT/MRI/DSA)
- **Key Results:** GPT-4 significantly outperforms GPT-3.5 (p<0.001)
- **Validation:** Internal
- **Personalization:** Modality-specific patient education
- **Links:** [Paper](https://www.sciencedirect.com/science/article/pii/S2772442524000807)

---

## Radiology Report Classification

### GPT-4 Radiology Boundaries (2023)
- **Authors:** Liu et al.
- **Venue:** EMNLP
- **Model:** GPT-4
- **Dataset:** Multiple radiology datasets
- **Key Results:** ~10% accuracy gain; SOTA on 5/6 tasks
- **Validation:** Benchmark
- **Links:** [Paper](https://aclanthology.org/2023.emnlp-main.891/)

### Italian BERT / GPT-4 (2024)
- **Authors:** Olivato et al.
- **Venue:** IEEE Access
- **Model:** Italian BERT / GPT-4
- **Dataset:** Italian CT reports (10K)
- **Key Results:** BERT outperforms; GPT-4 promising on open tasks
- **Validation:** Internal
- **Personalization:** Cross-lingual neoplastic report classification
- **Links:** [Paper](https://ieeexplore.ieee.org/abstract/document/10531266)

### GPT-3.5 Multilingual TNM (2024)
- **Authors:** Matsuo et al.
- **Venue:** Cancers
- **Model:** GPT-3.5-turbo
- **Dataset:** Lung cancer CT reports (162, EN/JA)
- **Key Results:** M-stage 94%, N-stage 80% (EN + full definition)
- **Validation:** Internal
- **Personalization:** Multilingual TNM staging
- **Links:** [Paper](https://www.mdpi.com/2072-6694/16/21/3621)

### Japanese BERT Brain MRI (2024)
- **Authors:** Kanzawa et al.
- **Venue:** Neuroradiology
- **Model:** BERT (Japanese fine-tuned)
- **Dataset:** Brain MRI reports (164 test, Japanese)
- **Key Results:** 97.0% accuracy; AUC 0.994/0.992; 20–26× faster
- **Validation:** Internal
- **Links:** [Paper](https://link.springer.com/article/10.1007/s00234-024-03427-7)

### Mistral Radiology Classification (2025)
- **Authors:** (Mistral in Radiology)
- **Venue:** International Journal of Imaging and Mathematical Analysis (IMA)
- **Model:** Mistral
- **Dataset:** Radiology reports (normal vs abnormal)
- **Key Results:** AI-powered classification of normal and abnormal reports
- **Validation:** Internal
- **Links:** [Paper](https://onlinelibrary.wiley.com/doi/abs/10.1002/ima.70251)

---

## Pathology Report Classification

### BB-TEN TNM Staging (2024)
- **Authors:** Kefeli et al.
- **Venue:** NPJ Precision Oncology
- **Model:** BB-TEN (BigBird)
- **Dataset:** TCGA (7K) + Columbia external (8K)
- **Key Results:** AUROC 0.815–0.942 (external)
- **Validation:** External
- **Links:** [Paper](https://www.nature.com/articles/s41467-024-53190-9)

### GPT-4 Breast Cancer Zero-shot (2024)
- **Authors:** Sushil et al.
- **Venue:** JAMIA
- **Model:** GPT-4, GPT-3.5, Starling, ClinicalCamel
- **Dataset:** UCSF breast pathology (769)
- **Key Results:** Macro-F1 0.86 vs 0.75 supervised
- **Validation:** Internal
- **Links:** [Paper](https://academic.oup.com/jamia/article/31/10/2315/7696538) · 
[Code](https://github.com/MadhumitaSushil/BreastCaPathClassification)

### Path-llama3.1 Cancer Staging (2025)
- **Authors:** Saluja et al.
- **Venue:** Scientific Reports
- **Model:** Path-llama3.1-8B / Path-GPT-4o-mini-FT
- **Dataset:** TCGA (9,523) + WCM external (60)
- **Key Results:** 89% cancer type; 70% AJCC staging (external)
- **Validation:** External
- **Links:** [Paper](https://www.nature.com/articles/s41598-025-10709-4) · 
[Code](https://github.com/rachitsaluja/PathRep-Bench)

### Gemini Gynecologic Registry (2025)
- **Authors:** Ishida et al.
- **Venue:** npj Precision Oncology
- **Model:** Gemini 1.5 / Qwen2.5 72B
- **Dataset:** Gynecologic oncology reports (150)
- **Key Results:** T/N accuracy 0.994/0.993; beats manual entry
- **Validation:** External
- **Links:** [Paper](https://www.nature.com/articles/s41698-025-01157-4) · 
[Code](https://github.com/iishiken/structured-clinical-data-extraction)

---