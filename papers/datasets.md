# Datasets and Benchmarks

Full annotated reference of datasets used across the 47 included studies,
organized by modality. Access labels indicate data availability.

**Access codes:**
- **Open** — freely downloadable without restriction
- **Credentialed** — free upon registration and data use agreement (PhysioNet or NCI)
- **Registration** — free upon institutional registration

---

## Text QA and Biomedical Knowledge

| Dataset | Clinical Domain | Scale | Primary Tasks | Access | Link |
|---------|----------------|-------|---------------|--------|------|
| MedQA (USMLE) | General medicine | Train 10,178 / Dev 1,272 / Test 1,273 | Multiple-choice professional exam QA | Open | [Paper](https://arxiv.org/abs/2009.13081) |
| MedMCQA | General medicine | Train 182,822 / Dev 4,183 / Test 6,150 | Multiple-choice exam QA; 21 subjects | Open | [Paper](https://arxiv.org/abs/2203.14371) |
| PubMedQA | Biomedical research | 1k expert-labeled | Yes/No/Maybe QA over abstracts | Open | [Paper](https://arxiv.org/abs/1909.06146) |
| BioASQ-QA | Biomedical research | Annual shared-task releases | Biomedical QA with evidence retrieval | Open | [Link](http://bioasq.org/) |
| MultiMedQA | Multi-domain | 7-dataset suite | Aggregated professional and consumer QA | Open | [Paper](https://www.nature.com/articles/s41586-023-06291-2) |

---

## Clinical NLP and Inference

| Dataset | Clinical Domain | Scale | Primary Tasks | Access | Link |
|---------|----------------|-------|---------------|--------|------|
| MedNLI | Clinical notes | ~14k premise-hypothesis pairs | Clinical NLI: entailment / neutral / contradiction | Credentialed | [PhysioNet](https://physionet.org/content/mednli/) |

---

## EHR: Structured Data and Clinical Notes

| Dataset | Clinical Domain | Scale | Primary Tasks | Access | Link |
|---------|----------------|-------|---------------|--------|------|
| MIMIC-III | ICU / hospital EHR | 58,000+ ICU admissions | Clinical notes, labs, vitals; phenotyping | Credentialed | [PhysioNet](https://physionet.org/content/mimiciii/) |
| MIMIC-IV | ICU / hospital EHR | 299,712 admissions | Clinical notes, labs, vitals; outcome prediction | Credentialed | [PhysioNet](https://physionet.org/content/mimiciv/) |

---

## Radiology: Image-Text Benchmarks

| Dataset | Clinical Domain | Scale | Primary Tasks | Access | Link |
|---------|----------------|-------|---------------|--------|------|
| MIMIC-CXR | Thoracic radiology | 377,110 images; 227,835 studies | Report generation, retrieval, CXR interpretation | Credentialed | [PhysioNet](https://physionet.org/content/mimic-cxr/) |
| CheXpert | Thoracic radiology | 224,316 radiographs; 65,240 patients | Multi-label CXR classification | Registration | [Stanford](https://stanfordmlgroup.github.io/competitions/chexpert/) |
| IU X-Ray (OpenI) | Thoracic radiology | ~7k studies | CXR report generation and retrieval | Open | [Link](https://openi.nlm.nih.gov/) |

---

## Medical Visual Question Answering

| Dataset | Clinical Domain | Scale | Primary Tasks | Access | Link |
|---------|----------------|-------|---------------|--------|------|
| VQA-RAD | Radiology | 315 images; 3,515 QA pairs | Radiology VQA; closed and open-ended | Open | [Paper](https://www.nature.com/articles/sdata2018251) |
| SLAKE | Multi-organ radiology | 642 images; 14,028 QA pairs; EN/ZH | Bilingual medical VQA; 12 diseases; 39 organs | Open | [GitHub](https://github.com/med-vqa/SLAKE) |
| PathVQA | Pathology | 4,998 images; 32,799 QA pairs | Open and closed-ended pathology VQA | Open | [GitHub](https://github.com/UCSD-AI4H/PathVQA) |
| PMC-VQA | Multi-domain | 227k QA pairs; 149k images | Large-scale multiple-choice medical VQA | Open | [GitHub](https://github.com/xiaoman-zhang/PMC-VQA) |

---

## Biomedical Image-Text Pretraining Corpora

| Dataset | Clinical Domain | Scale | Primary Tasks | Access | Link |
|---------|----------------|-------|---------------|--------|------|
| PMC-15M | Biomedical figures | 15M figure-caption pairs | VLM pretraining | Open | [GitHub](https://github.com/microsoft/BiomedCLIP) |
| QUILT-1M | Histopathology | ~1M image-text pairs | Histopathology VLM pretraining | Open | [GitHub](https://quilt1m.github.io/) |

---

## Medical Image Segmentation

| Dataset | Clinical Domain | Scale | Primary Tasks | Access | Link |
|---------|----------------|-------|---------------|--------|------|
| Medical Segmentation Decathlon | Multi-organ (CT + MRI) | 10 tasks; brain, liver, prostate, spleen | Multi-organ and tumor segmentation | Open | [Link](http://medicaldecathlon.com/) |
| ISIC | Dermatology | 25,000+ dermoscopy images | Skin lesion segmentation and classification | Open | [Link](https://www.isic-archive.com/) |

---

## Multi-Omics and Oncology

| Dataset | Clinical Domain | Scale | Primary Tasks | Access | Link |
|---------|----------------|-------|---------------|--------|------|
| TCGA | Oncology | 33 cancer types; >11k cases | Cancer subtyping, survival modeling, multimodal representation | Open† | [GDC](https://gdc.cancer.gov/) |

†Clinical, expression, mutation, and WSI data are openly available.
Raw sequencing reads require dbGaP controlled-access authorization.