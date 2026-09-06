# Retrieval, reasoning, and clinical agents

Explicit RAG is coded in **34/145 (23.4%)** studies; agent/tool use in **33/145 (22.8%)**; explicit agentic reasoning in **26/145 (17.9%)**.

| ID | Year | Model/System | Domain | RAG | Retrieval type | Tool use | Agentic reasoning | Knowledge source |
|---|---:|---|---|---|---|---|---|---|
| S007 | 2026 | DeepMed-RL-14B | General clinical medicine | Yes | Agentic retrieval | Yes | Yes | Open-web medical evidence via Search and Visit tools; sources include medical literature, clinical references, medical education, public-health sites, and other web sources |
| S010 | 2024 | GPT-3.5-turbo | Thoracic radiology / lung cancer | No | Static external context | No | No | Prompt-injected TNM staging definitions |
| S014 | 2026 | EHR-RAG | EHR / Clinical Prediction | Yes | Patient-specific RAG | No | Yes | Longitudinal structured EHR events |
| S016 | 2026 | AgentRx | Critical Care / Multimodal EHR | No | None | No | Yes | Patient summary + EHR + CXR + radiology reports |
| S017 | 2026 | MA-RAG | Medical QA | Yes | Multi-round RAG | Yes | Yes | External medical evidence retrieved iteratively |
| S018 | 2026 | MoMA | Multimodal EHR / Trauma / Substance Use | No | None | Yes | Yes | Clinical notes + chest radiographs + tabular EHR/laboratory data |
| S019 | 2026 | AgentClinic | General Clinical Diagnosis / Multimodal Agents | Yes | Agentic retrieval | Yes | Yes | Adaptive RAG (book/web), patient dialogue, measurements, images, notebook memory |
| S020 | 2025 | Autonomous oncology AI agent | Oncology / Precision Medicine | Yes | Agentic retrieval | Yes | Yes | OncoKB, PubMed, Google, oncology guidelines + multimodal tools |
| S021 | 2026 | MIRA | Emergency Medicine / EHR | No | Agentic retrieval | Yes | Yes | Sandboxed MIMIC-IV EHR with 11 tool classes and >85,000 options |
| S022 | 2025 | RaR | Radiology / Clinical QA | Yes | Multi-round RAG | Yes | Yes | Radiopaedia.org |
| S023 | 2025 | LLM-RAG for medical fitness | Perioperative Medicine | Yes | Patient-specific RAG | Yes | No | 35 local + 23 international perioperative guidelines |
| S026 | 2025 | Hybrid open-source LLM + UMLS parser | Breast oncology / EHR | No | Static external context | No | No | Longitudinal clinical notes + UMLS terminology |
| S039 | 2024 | GeneGPT | Other | No | Other | Yes | No | NCBI Web APIs / biomedical databases |
| S043 | 2024 | GPT-4V | Cancer pathology | No | Static external context | No | No | In-context labeled pathology images/examples |
| S048 | 2026 | ClinFusion | General Medical Imaging / 2D & 3D | Yes | RAG | Yes | Yes | Optional evidence-grounded retrieval/tools plus medical images |
| S063 | 2025 | MedPlan | Outpatient / Emergency EHR | Yes | Patient-specific RAG | Yes | No | Patient's own prior SOAP notes + similar patients' records |
| S064 | 2026 | EHR-RAGp | Longitudinal EHR / Clinical Prediction | Yes | Patient-specific RAG | NR | NR | Current visit query over the same patient's longitudinal EHR chunks |
| S065 | 2026 | Vital Trace | Critical Care / Longitudinal EHR | No | None | No | Yes | Persistent patient-state memory + static clinical protocol |
| S066 | 2025 | Traj-CoA | Lung Cancer / Longitudinal EHR | No | None | NR | Yes | Five-year structured and unstructured EHR trajectory stored in shared EHRMem |
| S067 | 2025 | CARE-AD | Neurology / Alzheimer's Disease | No | None | NR | Yes | Chronological patient profile extracted from longitudinal clinical notes |
| S069 | 2026 | AI4Doctor / AI4Doc-LLM | General EHR / Clinical Decision Support | Yes | Patient-specific RAG | Yes | NR | Similar EMRs and clinical guidance retrieved using the current patient's EMR context |
| S076 | 2026 | FHIR-RAG-MEDS | General Clinical Decision Support / FHIR | Yes | Patient-specific RAG | Yes | NR | Real-time HL7 FHIR patient context + disease-specific clinical guidelines |
| S077 | 2025 | BiomedRAG | Biomedical NLP / RAG | Yes | RAG | No | No | Retrieved task-relevant biomedical evidence |
| S080 | 2025 | Regional encoder + retrieval + LLM refinement | Pathology / WSI | Yes | RAG | No | No | Historically similar pathology cases |
| S081 | 2024 | CH-ICL | Medical VQA / knowledge augmentation | Yes | Static external context | No | No | 16K-term medical dictionary + retrieved candidate exemplars |
| S082 | 2024 | MedGraphRAG | General Medical QA / Knowledge Grounding | Yes | Graph-RAG | Yes | Yes | User documents + authoritative medical sources + controlled vocabularies |
| S083 | 2025 | MRD-RAG | General Clinical Diagnosis / Medical QA | Yes | Multi-round RAG | Yes | Yes | Disease knowledge retrieved iteratively from patient-specific diagnostic state |
| S084 | 2025 | Local LLM + RAG | Radiology / Contrast Media Consultation | Yes | Patient-specific RAG | Yes | NR | Authoritative radiology contrast-media references |
| S085 | 2025 | BriefContext | Medical QA / Long-Context RAG | Yes | RAG | NR | NR | Long retrieved biomedical contexts |
| S086 | 2026 | DeepRare | Rare Disease / Genomics / Multimodal Clinical Reasoning | Yes | Agentic retrieval | Yes | Yes | Phenotype/genetic databases, web-scale medical knowledge, specialist tools |
| S087 | 2026 | MED-COPILOT | Clinical Decision Support / EHR | Yes | Patient-specific RAG | Yes | Yes | WHO/NICE guideline GraphRAG + similar MIMIC-IV/Synthea patient cases |
| S088 | 2026 | MED-VRAG | Medical VQA / Multimodal Retrieval | Yes | Multimodal RAG | Yes | Yes | ~350K PMC page images with patch-level retrieval |
| S090 | 2026 | SEMA-RAG | Medical QA / Agentic RAG | Yes | Multi-round RAG | Yes | Yes | Medical evidence retrieved until sufficiency criterion is met |
| S091 | 2025 | AMG-RAG | Medical QA / Knowledge Graphs | Yes | Graph-RAG | Yes | Yes | Automatically constructed and updated medical knowledge graph + external evidence |
| S092 | 2026 | MedRAGChecker | Medical RAG Safety / Evaluation | Yes | RAG | NR | NR | Retrieved passages + DRKG medical knowledge graph for verification |
| S093 | 2026 | RAG-X | Medical RAG Evaluation / Safety | Yes | RAG | NR | NR | Task-specific retrieved medical passages/guidelines |
| S094 | 2026 | KG-Followup | Clinical Dialogue / Follow-Up Reasoning | Yes | Graph-RAG | Yes | Yes | Medical KG concepts and diagnostic reasoning paths retrieved from patient conversation/EHR entities |
| S095 | 2026 | MedClarify | Clinical Diagnosis / Interactive Reasoning | No | None | NR | Yes | Interactive patient responses elicited by clarification questions |
| S097 | 2026 | MediGRAF | EHR / Patient-Specific QA | Yes | Patient-specific RAG | Yes | Yes | Patient-specific Neo4j graph + vectorized unstructured EHR narratives |
| S099 | 2025 | Medical RAG Expert Evaluation | Medical RAG Evaluation / Human Expert Study | Yes | RAG | NR | NR | Retrieved passages for patient/USMLE-style questions |
| S100 | 2025 | MMed-RAG | Medical Vision-Language / Multimodal RAG | Yes | Multimodal RAG | NR | NR | Retrieved medical image-text evidence across radiology, ophthalmology, and pathology |
| S101 | 2025 | Gemini 1.5 / Qwen2.5-72B | Gynecologic oncology / registry | Yes | Static external context | No | No | Dialogue + Wikipedia/offline medical knowledge |
| S109 | 2026 | MS-FBI calibration | Medical VQA / Calibration | No | None | NR | NR | Medical VQA image-question evidence |
| S110 | 2026 | CARE | Clinical Summarization / Calibration | No | None | NR | NR | Clinical source documents and generated summaries |
| S113 | 2025 | CAP | Critical Care / Fairness | Yes | Patient-specific RAG | NR | NR | Similar historical misprediction cases and correct outcomes |
| S117 | 2026 | MPIB | Medical Security / Prompt Injection | Yes | RAG | NR | NR | Clinical queries plus optionally poisoned RAG context |
| S119 | 2026 | MedPriv-Bench | Medical QA / Privacy | No | RAG | NR | NR | Sensitive medical contexts with realistic privacy pressure |
| S126 | 2026 | OpenManus / Manus | Clinical Agents / Safety | Yes | Agentic retrieval | Yes | Yes | Web/tools/benchmark-specific evidence |
| S128 | 2026 | PreA | Primary-to-Specialist Care / Referral | No | None | Yes | Yes | Patient dialogue gathered adaptively before specialist consultation |
| S136 | 2026 | MedAgentBrief | Hospital Medicine / Clinical Summarization | No | None | NR | Yes | History & physical plus daily progress notes with source citations |
