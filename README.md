# Replication Package — Meta_Ozat SLR (AP25796141)

**Title:** Machine Learning and Gamification in Higher Education: A Systematic Literature Review
**Project:** AP25796141 (Kazakhstan)
**Authors:** D. Zhaxybayev et al.
**Target venue:** Scopus Q1/Q2 journal

---

## Repository Structure

| File | Description |
|------|-------------|
| `corpus.json` | Full annotated corpus — 75 records (73 synthesis + 2 background references) |
| `MMAT_Assessment_AP25796141.xlsx` | MMAT 2018 quality scores for all 75 papers (tier, study type, sensitivity flag) |
| `PRISMA_Screening_MetaOzat.xlsx` | Complete screening workbook: title/abstract screening (Stage 1) and full-text eligibility (Stage 2); includes MMAT criteria reference sheet |
| `PRISMA_Flowchart_MetaOzat.svg` | PRISMA 2020 flow diagram (vector format, print-ready) |
| `search_protocol.md` | Registered search protocol: databases, query strings, date, inclusion/exclusion criteria |

---

## Corpus Summary

| Category | n |
|----------|---|
| **Total identified** | 4,547 |
| After deduplication | 4,121 |
| Stage 1 included | 392 |
| Stage 2 eligible | 75 |
| **Synthesis corpus (Tier 1+2)** | **71** |
| Tier 1 (MMAT ≥ 4, full text) | 42 |
| Tier 2 (MMAT 2–3, full text) | 29 |
| Tier 3 (closed-access, abstract-proxy) | 2 |
| Background references (Tier R) | 2 |
| Mean MMAT score | 3.95 |

---

## Research Questions

| RQ | Focus |
|----|-------|
| RQ1 | Which ML/DL architectures are used for personalized learning pathway generation? |
| RQ2 | How do gamification-integrated AI systems affect student engagement and learning outcomes? |
| RQ3 | How effective are LLM-based tools in supporting critical thinking in higher education? |
| RQ4 | Which recommender algorithms best predict academic performance? |
| RQ5 | What is the state of AI in education research in Kazakhstan and Central Asia? |

---

## Quality Assessment (MMAT 2018)

Quality was assessed using the Mixed Methods Appraisal Tool (MMAT) 2018 (Hong et al., 2018). Each paper was scored on five study-type-specific criteria (YES=1, NO=0, Cannot tell=0). Papers with MMAT ≥ 4 were assigned to Tier 1; MMAT 2–3 to Tier 2.

A **sensitivity analysis** restricting synthesis to Tier 1+2 papers (n=71; 97.3%) confirmed that all primary conclusions across RQ1–RQ5 are unchanged.

---

## Corpus JSON Schema

Each entry in `corpus.json` has the following fields:

| Field | Type | Description |
|-------|------|-------------|
| `tier` | int/str | Quality tier: 1, 2, 3, or "R" (background reference) |
| `tier_label` | str | Human-readable tier description |
| `doi` | str | Digital Object Identifier |
| `title` | str | Full paper title |
| `year` | str | Publication year |
| `journal` | str | Journal or conference name |
| `rq` | str | Assigned research question (RQ1–RQ5) |
| `mmat_score` | str | Total MMAT 2018 score (0–5) |
| `ml_method` | str | Key ML/AI method described in the paper |
| `sample` | str | Study sample (participants, dataset size) |
| `key_finding` | str | Primary finding relevant to the RQ |
| `cited` | str | Citation count at time of screening |

---

## Search Protocol Summary

See `search_protocol.md` for the full registered protocol.

- **Databases:** Scopus (primary), Web of Science (validation)
- **Date executed:** March–April 2026
- **Temporal scope:** 2016–2026
- **Language:** English
- **Document types:** Article, Review

---

## Citation

If you use this dataset or protocol, please cite:

> Zhaxybayev D. et al. (2026). Machine Learning and Gamification in Higher Education: A Systematic Literature Review. [Journal name pending]. DOI: [pending]

---

## License

This replication package is released under the **Creative Commons Attribution 4.0 International (CC BY 4.0)** license.
You are free to share and adapt the material for any purpose, provided appropriate credit is given.
