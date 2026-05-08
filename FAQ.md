# Frequently Asked Questions

---

## About the Survey

**Q: What is this repository?**

This repository accompanies our systematic review:
*Large Language Models in Clinical Medicine — A Systematic Review
of Multimodal Architectures, Benchmarks, and Personalized Healthcare
Applications* (AI Review, Springer, 2025). It provides a curated,
maintained, and machine-readable reference of all included studies,
benchmark leaderboards, dataset resources, and reproducibility ratings.

---

**Q: How were the 56 studies selected?**

Studies were identified through a PRISMA 2020-compliant search across
six bibliographic databases (PubMed, IEEE Xplore, Web of Science,
Scopus) and supplementary sources
(arXiv, citation tracking, related survey screening). All 56 included
studies satisfy three quality criteria:

- The LLM is the primary methodological contribution
- Quantitative evaluation is reported on a named medical dataset
- The work appears in a peer-reviewed venue or a rigorous preprint
  with full methodology and institutional affiliation

---

**Q: Why is paper X not included?**

The most common reasons a paper is excluded:

- The LLM is used only as a preprocessing or auxiliary component
- No quantitative evaluation is reported on a named dataset
- The study falls outside the clinical medicine scope
  (e.g., purely molecular or protein sequence modeling)
- The paper was published after our search cutoff date

If you believe a paper meets all inclusion criteria and should be
added, please open an issue using the
[Add Paper template](.github/ISSUE_TEMPLATE/add_paper.md).

---

**Q: What does "personalized healthcare" mean as an organizing
framework?**

Rather than treating personalization as a single application,
our survey uses it as an analytical lens applied across all nine
task categories. We assess each study on whether it addresses
patient-specific adaptation, population stratification, or
individualized clinical output — even when the study does not
explicitly frame itself around personalization.

---

## Using the Repository

**Q: How do I cite this survey?**
```bibtex
@article{...,
  title     = {Large Language Models in Clinical Medicine ---
               A Systematic Review of Multimodal Architectures,
               Benchmarks, and Personalized Healthcare Applications},
  author    = {Mohamed, Walid and Fayyaz, Rafia and
               Mousattat, Usama and {Al Hamadani}, Shahad and
               Soliman, Taysir and Abdelaziz, {Amr Mohamed} and
               Elsharkawy, Mohamed and Mahmoud, Ali and
               Ghazal, Mohamed},
  journal   = {},
  publisher = {},
  year      = {2025}
}
```

The full BibTeX file for all 47 included studies is available
in [`references/survey.bib`](references/survey.bib).

---

**Q: How do I download all paper references at once?**

Open [`references/survey.bib`](references/survey.bib) and download
the raw file. It is compatible with all major reference managers
including Zotero, Mendeley, EndNote, and JabRef.

---

**Q: Can I use the dataset table or leaderboard in my own work?**

Yes — this repository is MIT licensed. Please cite the survey
when using any content from this repository.

---

**Q: How do I find papers from a specific task category?**

Each paper is tagged by section in
[`data/papers.json`](data/papers.json) under the `category` and
`section` fields. You can also navigate directly:

| Category | File |
|----------|------|
| All text-based papers | [`papers/text_based.md`](papers/text_based.md) |
| All multimodal papers | [`papers/multimodal.md`](papers/multimodal.md) |
| Datasets and benchmarks | [`papers/datasets.md`](papers/datasets.md) |
| Model comparison | [`papers/model_comparison.md`](papers/model_comparison.md) |
| Reproducibility ratings | [`papers/reproducibility.md`](papers/reproducibility.md) |

---

## Contributing

**Q: How do I add a new paper?**

Two options:

1. Open a [Pull Request](../../pulls) — add the paper to the
   correct section in `README.md`, `papers/text_based.md` or
   `papers/multimodal.md`, update `data/papers.json`,
   `papers/reproducibility.md`, and `references/survey.bib`
2. Open an [Issue](../../issues/new?template=add_paper.md) —
   fill in the Add Paper template and a maintainer will add it

Full guidelines in [`CONTRIBUTING.md`](CONTRIBUTING.md).

---

**Q: What files do I need to update when adding a new paper?**

| File | What to update |
|------|---------------|
| `README.md` | Add row to correct table |
| `papers/text_based.md` or `papers/multimodal.md` | Add detailed entry |
| `data/papers.json` | Add structured JSON entry with new id |
| `papers/reproducibility.md` | Add reproducibility rating |
| `references/survey.bib` | Add BibTeX entry |
| `papers/model_comparison.md` | Add model if not already listed |
| `README.md` badges | Update paper count number |

---

**Q: How often is this repository updated?**

We update the repository when:

- New papers meeting inclusion criteria are identified
- Benchmark leaderboard results are superseded
- Broken links are reported
- The survey is revised or published

---

## Technical Questions

**Q: How do I use `data/papers.json` programmatically?**

The JSON file follows a consistent schema. Example in Python:
```python
import json

with open('data/papers.json', 'r') as f:
    data = json.load(f)

# Get all papers in a specific category
vqa_papers = [
    p for p in data['papers']
    if p['category'] == 'Medical Visual QA'
]

# Get all fully open-source papers
open_papers = [
    p for p in data['papers']
    if p['code_available'] is True
]

# Get papers by year
papers_2025 = [
    p for p in data['papers']
    if p['year'] == 2025
]

print(f"Total papers: {data['metadata']['total_studies']}")
print(f"VQA papers: {len(vqa_papers)}")
print(f"Open source: {len(open_papers)}")
```

---

**Q: How do I report a broken link or incorrect information?**

Open an [Issue](../../issues/new) with the title:
`Fix: [brief description]` and include the file name,
line number, and what the correct information should be.