# Multimodal fusion evidence

The final corpus contains **72/145 (49.7%)** fusion-active studies (F1–F5). Deep, decision-level, or hybrid fusion (F3–F5) occurs in **44/145 (30.3%)** studies.

| ID | Year | Model/System | Domain | Modal inputs | Stage | Operator | Direction | Temporal fusion |
|---|---:|---|---|---|---|---|---|---|
| S015 | 2026 | ChatHealthAI | EHR / Clinical Prediction | Text + EHR + Structured clinical + Labs | F2 | Task-aware resampling / latent EHR-to-LLM alignment + refined event text | Unidirectional | Longitudinal |
| S016 | 2026 | AgentRx | Critical Care / Multimodal EHR | Text + 2D image + EHR + Structured clinical + Labs | F5 | Input/context concatenation; modality-specialized agents; majority vote/debate/coordination | Iterative | Prior-current |
| S018 | 2026 | MoMA | Multimodal EHR / Trauma / Substance Use | Text + 2D image + EHR + Structured clinical + Labs | F5 | Textual transformation; concatenation; hierarchical LLM aggregation | Iterative | Prior-current |
| S020 | 2025 | Autonomous oncology AI agent | Oncology / Precision Medicine | Text + 2D image + 3D image + WSI + EHR + Structured clinical + Labs | F5 | Tool-mediated multimodal fusion; textual transformation; web/knowledge retrieval | Iterative | Prior-current |
| S021 | 2026 | MIRA | Emergency Medicine / EHR | Text + EHR + Structured clinical + Labs | F5 | Agentic retrieval/action over EHR tools and structured/text evidence | Iterative | Prior-current |
| S027 | 2025 | BrainGPT | Neuroradiology / 3D CT | Text + 3D image | F3 | Cross-attention | Unidirectional | None |
| S028 | 2023 | R2GenGPT | Radiology / report generation | Text + 2D image | F2 | MLP | Unidirectional | None |
| S029 | 2023 | LLaVA-Med | Biomedical multimodal QA | Text + 2D image | F2 | MLP | Unidirectional | None |
| S030 | 2024 | MAIRA-2 | Radiology / grounded report generation | Text + 2D image | F2 | MLP | Unidirectional | None |
| S031 | 2025 | MediVLM | Radiology / report generation | Text + 2D image | F3 | Cross-attention | Unidirectional | None |
| S032 | 2024 | PMC-VQA / PMC-LLaMA | Medical VQA | Text + 2D image | F2 | Linear projection / MLP | Unidirectional | None |
| S034 | 2025 | CIF | Medical VQA / causal reasoning | Text + 2D image + Structured clinical | F3 | Cross-attention + feature injection | Unidirectional | None |
| S035 | 2025 | MiniMedGPT | Medical VQA / efficient MLLM | Text + 2D image | F2 | Linear projection | Unidirectional | None |
| S036 | 2025 | FAVP | Medical VQA / adaptive prompting | Text + 2D image | F3 | Attention weighting | Unidirectional | None |
| S037 | 2025 | Falcon Med-VQA | Medical VQA / uncertainty | Text + 2D image | F3 | Q-Former/query tokens | Unidirectional | None |
| S041 | 2024 | GPT-4V | Chest radiology / multimodal diagnosis | Text + 2D image | F3 | Other | Unidirectional | None |
| S042 | 2025 | Claude 3.5 Sonnet + 5 MLLMs | Laryngeal cancer surgery | Text + 2D image + 3D image | F3 | Other | Unidirectional | None |
| S043 | 2024 | GPT-4V | Cancer pathology | Text + 2D image | F3 | Other | Unidirectional | None |
| S044 | 2025 | M3FM | Radiology / multilingual diagnosis | Text + 2D image + 3D image | F3 | Cross-attention / model-specific | Unidirectional | None |
| S045 | 2024 | PathChat | Pathology | Text + 2D image + WSI | F2 | Linear projection / MLP | Unidirectional | None |
| S046 | 2024 | Med-PaLM M | Generalist biomedical AI | Text + 2D image + 3D image + WSI | F3 | Other | Unidirectional | None |
| S047 | 2024 | LLMSeg | Radiation oncology | Text + 3D image + Structured clinical | F3 | Bidirectional cross-attention | Bidirectional | None |
| S048 | 2026 | ClinFusion | General Medical Imaging / 2D & 3D | Text + 2D image + 3D image | F5 | Compositional encoder fusion; cascaded locality-aware fusion; 2D-anchored depth-aware 3D fusion | Iterative | None |
| S049 | 2026 | Multimodal autoregressive EHR foundation model | Longitudinal EHR / Multimodal Clinical Data | Text + 2D image + EHR + Structured clinical + Labs | F3 | Latent compression; gated cross-attention; temporal alignment masking | Unidirectional | Longitudinal |
| S050 | 2025 | mpLLM | Neuroradiology / Multiparametric MRI | Text + 3D image | F3 | Modality-level MoE; token-level MoE; prompt-conditioned routing; multi-image token fusion | Unidirectional | None |
| S051 | 2026 | 2D-to-3D Phi-3-V with TGH-MoE | 3D CT / General Medical Imaging | Text + 3D image | F5 | 2D-to-3D attention adaptation; token-level MoE; task-level hard-routed MoE; image-text concatenation | Unidirectional | None |
| S052 | 2024 | MedPLIB | General Biomedical Imaging | Text + 2D image | F5 | Feature concatenation; visual prompt injection; token-level MoE; task-specialized VL/grounding experts; [SEG]→pixel decoder | Unidirectional | None |
| S053 | 2024 | Med-2E3 | 3D CT | Text + 3D image | F3 | Dual 3D/2D feature fusion; text-guided inter-slice attention; connector alignment | Unidirectional | None |
| S054 | 2025 | MedRegion-CT | Radiology / 3D CT | Text + 3D image | F5 | Global/local SlowFast tokenization; hierarchical mask-token fusion; lesion-attribute textualization; token concatenation | Unidirectional | None |
| S055 | 2026 | MedVL-SAM2 | 3D CT / Segmentation | Text + 3D image | F5 | 3D token compression/alignment; text+visual token fusion; [SEG] hidden-state coupling to SAM2 | Unidirectional | None |
| S056 | 2026 | MLLM-HWSI | Computational Pathology / WSI | Text + WSI | F5 | Cell/patch/region/WSI hierarchical fusion; contrastive alignment; cross-scale consistency; scale-specific projection | Unidirectional | None |
| S057 | 2025 | Citrus-V | General Medical Imaging | Text + 2D image | F5 | Joint vision/text token fusion; dual image encoders; [SEG]-mediated reasoning-to-segmentation transfer | Unidirectional | None |
| S058 | 2026 | UniReason-Med | General Medical Imaging / 2D & 3D | Text + 2D image + 3D image | F3 | Self-generated box/cuboid grounding; region-token injection; interleaved text/visual reasoning tokens | Iterative | None |
| S059 | 2025 | V2T-CoT | Medical VQA / Radiology & Pathology | Text + 2D image | F3 | Phrase grounding; regional/global visual attention; cross-modal multi-head attention; iterative text refinement | Bidirectional | None |
| S060 | 2025 | PolyPath / Gemini 1.5 Flash | Pathology / WSI | Text + WSI | F3 | Other | Iterative | None |
| S061 | 2024 | SkinGPT-4 | Dermatology | Text + 2D image | F2 | Linear projection / MLP | Unidirectional | None |
| S062 | 2025 | MedTVT-R1 | Multimodal clinical diagnosis | Text + 2D image + Structured clinical + Labs | F5 | Attention weighting / gated adaptive fusion | Iterative | None |
| S064 | 2026 | EHR-RAGp | Longitudinal EHR / Clinical Prediction | Text + EHR + Structured clinical + Labs | F2 | Multi-granular longitudinal chunk retrieval + prototype-guided representation fusion | Unidirectional | Longitudinal |
| S066 | 2025 | Traj-CoA | Lung Cancer / Longitudinal EHR | Text + EHR + Structured clinical + Labs | F1 | Structured/unstructured EHR serialization + sequential memory-based agent aggregation | Iterative | Longitudinal |
| S069 | 2026 | AI4Doctor / AI4Doc-LLM | General EHR / Clinical Decision Support | Text + EHR + Structured clinical + Labs | F1 | Temporal EMR serialization + patient-specific similar-record/guideline retrieval | Iterative | Longitudinal |
| S070 | 2026 | Generative Deep Patient (GDP) | EHR / Multimodal Clinical Data | Text + EHR + Structured clinical + Labs | F3 | Structured-EHR and unstructured-text cross-attention into generative decoder | Bidirectional | Longitudinal |
| S071 | 2026 | EHRWorld | Longitudinal EHR / Digital Patient Modeling | Text + EHR + Structured clinical + Labs | F1 | Profile/event serialization and causal longitudinal state modeling | Iterative | Longitudinal |
| S072 | 2025 | DT-GPT | Longitudinal EHR / Digital Twins | Text + EHR + Structured clinical + Labs | F1 | Serialized longitudinal patient-state fusion into autoregressive LLM | Unidirectional | Longitudinal |
| S073 | 2025 | HC-LLM | Radiology / Longitudinal Imaging | Text + 2D image | F5 | Current/prior image fusion; prior-report fusion; intra-modality similarity and cross-modal consistency constraints | Bidirectional | Longitudinal |
| S074 | 2026 | Harrison.Rad 1.5 | Radiology / Multimodal Foundation Models | Text + 2D image + Structured clinical | F3 | Interleaved current images + priors + clinical-context token interaction | Bidirectional | Longitudinal |
| S075 | 2026 | ALTER | Radiology / 3D CT | Text + 3D image | F5 | Global current/prior attention; region-level historical proxy retrieval; change-aware soft prompts | Bidirectional | Longitudinal |
| S076 | 2026 | FHIR-RAG-MEDS | General Clinical Decision Support / FHIR | Text + EHR + Structured clinical + Labs | F1 | Structured patient context textualization + patient-specific evidence retrieval | Unidirectional | None |
| S078 | 2024 | ChatGPT (GPT-4 with image input) | Dermatology | Text + 2D image | F3 | Other | Unidirectional | None |
| S079 | 2023 | ChatDoctor | General medicine / dialogue | Text + 2D image | F3 | Cross-attention | Unidirectional | None |
| S080 | 2025 | Regional encoder + retrieval + LLM refinement | Pathology / WSI | Text + WSI | F5 | Attention weighting + Other | Unidirectional | None |
| S081 | 2024 | CH-ICL | Medical VQA / knowledge augmentation | Text + 2D image | F5 | Other | Iterative | None |
| S086 | 2026 | DeepRare | Rare Disease / Genomics / Multimodal Clinical Reasoning | Text + EHR + Structured clinical + Labs | F5 | Phenotype/genetic/clinical evidence integration; web/tool retrieval; specialist-agent fusion | Iterative | Longitudinal |
| S087 | 2026 | MED-COPILOT | Clinical Decision Support / EHR | Text + EHR + Structured clinical + Labs | F1 | Structured patient context + GraphRAG + semantic/keyword similar-patient retrieval | Iterative | Prior-current |
| S088 | 2026 | MED-VRAG | Medical VQA / Multimodal Retrieval | Text + 2D image | F3 | Page-image patch retrieval; visual-text interaction; iterative multimodal evidence selection | Iterative | None |
| S094 | 2026 | KG-Followup | Clinical Dialogue / Follow-Up Reasoning | Text + EHR + Structured clinical | F1 | Patient conversation/EHR serialization + concept/path retrieval from medical KG | Iterative | Prior-current |
| S097 | 2026 | MediGRAF | EHR / Patient-Specific QA | Text + EHR + Structured clinical + Labs | F1 | Structured patient-graph traversal + unstructured narrative vector retrieval | Iterative | Longitudinal |
| S098 | 2026 | AI Consult V1 | Primary Care / LMIC / Safety | Text + EHR + Structured clinical + Labs | F1 | Symptoms, vitals, history and other encounter data serialized into patient-specific clinical prompt | Unidirectional | None |
| S100 | 2025 | MMed-RAG | Medical Vision-Language / Multimodal RAG | Text + 2D image | F3 | Image/text medical retrieval; adaptive multimodal context injection | Unidirectional | None |
| S103 | 2025 | HCR / Gemini 2.5 Flash | Segmentation / safety | Text + 2D image | F4 | Decision-level LLM quality classification | Unidirectional | None |
| S113 | 2025 | CAP | Critical Care / Fairness | Text + EHR + Structured clinical + Labs | F1 | Structured patient context + retrieved corrective cases | Unidirectional | None |
| S116 | 2026 | Surgical VLM prompt-injection study | Surgery / VLM Security | Text + 2D image | F3 | Native video/image-text VLM fusion under attack | Iterative | None |
| S119 | 2026 | MedPriv-Bench | Medical QA / Privacy | Text + Structured clinical + Labs | F1 | Sensitive patient context textualization for QA | Unidirectional | None |
| S120 | 2025 | Abridge AI scribe | Ambulatory Care / Ambient AI | Text | F1 | Spoken encounter converted to structured note | Unidirectional | None |
| S126 | 2026 | OpenManus / Manus | Clinical Agents / Safety | Text + 2D image + EHR + Structured clinical + Labs | F5 | Agentic fusion of text, multimodal inputs, tools, and external information | Iterative | Prior-current |
| S127 | 2026 | AI Consult 2.0 | Primary Care / LMIC | Text + EHR + Structured clinical + Labs | F1 | Clinical variables and free-text encounter data serialized into patient-specific prompt | Unidirectional | None |
| S129 | 2026 | Xuanwu-NeuroAid | Emergency Neurology | Text + EHR + Structured clinical + Labs | F1 | Vitals, labs and imaging reports converted to standardized textual descriptors | Unidirectional | None |
| S130 | 2024 | DeepDR-LLM | Diabetes / Ophthalmology / Primary Care | Text + 2D image + EHR + Structured clinical + Labs | F5 | Retinal image analysis, lesion/DR grading, and clinical metadata integrated for individualized recommendation | Unidirectional | None |
| S132 | 2025 | Ambient AI scribe | Clinical Documentation / Ambient AI | Text | F1 | Ambient audio transformed into structured clinical documentation | Unidirectional | None |
| S133 | 2025 | Ambient AI | Clinical Documentation / Ambient AI | Text | F1 | Ambient encounter audio transformed into documentation | Unidirectional | None |
| S134 | 2025 | Abridge ambient AI scribe | Ambulatory Care / Ambient AI | Text | F1 | Encounter audio and transcript synthesized into clinical note | Unidirectional | None |
| S135 | 2025 | DAX Copilot | Ambulatory Care / Ambient AI | Text | F1 | Speech interpretation and structured note generation | Unidirectional | None |
| S137 | 2024 | GPT-4 draft replies | Patient Portal / Ambulatory Care | Text + EHR + Structured clinical | F1 | Message text, structured patient elements, and prior clinic note combined in prompt | Unidirectional | Prior-current |
