# Contributing to LLMs in Medicine

Thank you for helping keep this list current and accurate.

---

## How to Add a Paper

### Option 1 — Pull Request (preferred)

1. **Fork** this repository
2. **Add** your paper to the correct section in `README.md`
3. **Follow** the format below exactly
4. **Submit** a Pull Request with title: `Add: [Paper Title]`

### Option 2 — Issue

Open a [new issue](../../issues/new?template=add_paper.md) using
the Add Paper template. A maintainer will add it within a week.

---

## Paper Format
```markdown
| YEAR | **Full Paper Title** | Model Name | *Venue* | [![Paper](https://img.shields.io/badge/Paper-blue)](URL) [![Code](https://img.shields.io/badge/Code-Available-blue)](URL) ![Badge] |
```

### Badges

| Badge | When to use |
|-------|-------------|
| `![Code](https://img.shields.io/badge/Code-Available-blue)` | Public code available |
| `![SOTA](https://img.shields.io/badge/-SOTA-red)` | SOTA at publication time |
| `![Prospective](https://img.shields.io/badge/Val-Prospective-purple)` | Prospective clinical validation |
| `![External](https://img.shields.io/badge/Val-External-orange)` | External multi-site validation |

---

## Inclusion Criteria

A paper must satisfy ALL of the following:

- [ ] LLM is the **primary methodological contribution**
- [ ] Applied to **clinical medicine or healthcare**
- [ ] Reports **quantitative evaluation** on a named dataset
- [ ] Published in a **peer-reviewed venue** or rigorous preprint
  with full methodology and institutional affiliation

## Exclusion Criteria

- Imaging-only pipelines with no language model component
- Molecular or protein sequence modeling without clinical application
- Opinion pieces without empirical evaluation
- Duplicate publications

---

## Section Guide

| Your paper covers | Add to section |
|-------------------|----------------|
| EHR, clinical notes, NLP | Text-Based → Clinical Documentation |
| PubMed, literature, knowledge graphs | Text-Based → Literature Mining |
| QA, decision support, chatbots | Text-Based → Decision Support |
| Radiology or pathology text classification | Text-Based → Report Classification |
| Summarization, discharge notes | Text-Based → Summarization |
| Radiology report generation (image + text) | Multimodal → Radiology Reports |
| Pathology report generation (WSI + text) | Multimodal → Pathology Reports |
| Medical VQA | Multimodal → Visual QA |
| Segmentation with LLM component | Multimodal → Segmentation |
| Multimodal fusion for diagnosis | Multimodal → Diagnosis |

---

## Leaderboard Updates

To update a benchmark leaderboard entry, include:

- Benchmark name (e.g., VQA-RAD, MedQA)
- Metric and value (e.g., Accuracy 89.3%)
- Model name and paper link
- Closed-set or open-set evaluation

---

## Code of Conduct

Be respectful. All contributions are welcome regardless of institutional affiliation or geographic origin.
