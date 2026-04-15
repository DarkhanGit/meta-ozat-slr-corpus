# Search Protocol — Meta_Ozat SLR (AP25796141)

**Protocol version:** 1.0
**Date registered:** March 2026
**Search executed:** March–April 2026
**Project ID:** AP25796141

---

## 1. Research Questions

| RQ | Full question |
|----|---------------|
| RQ1 | Which machine learning and deep learning architectures are most commonly applied to generate personalized learning pathways in higher education, and what are their reported performance metrics? |
| RQ2 | How do AI-integrated gamification systems affect student engagement and learning outcomes compared with non-gamified adaptive learning environments? |
| RQ3 | How effective are large language model (LLM)-based tools in supporting or assessing critical thinking skills in higher education settings? |
| RQ4 | Which recommender and predictive algorithms demonstrate the highest accuracy for academic performance prediction, and what are the key input features? |
| RQ5 | What is the current state of AI-in-education research in Kazakhstan and Central Asia, and what gaps remain compared with global trends? |

---

## 2. Databases Searched

| Database | Role | Records retrieved |
|----------|------|-------------------|
| Scopus | Primary | 4,547 |
| Web of Science | Validation / supplementary | — |

---

## 3. Search Query

### 3.1 Scopus Master Query

```
TITLE-ABS-KEY (
  ("machine learning" OR "deep learning" OR "artificial intelligence" OR "neural network"
   OR "large language model" OR "LLM" OR "generative AI" OR "ChatGPT" OR "GPT-4"
   OR "recommender system" OR "adaptive learning" OR "personalized learning")
  AND
  ("higher education" OR "university" OR "e-learning" OR "online learning"
   OR "educational technology" OR "student performance" OR "learning outcomes")
  AND
  ("gamification" OR "game-based learning" OR "critical thinking" OR "engagement"
   OR "motivation" OR "learning path" OR "learning trajectory")
)
AND PUBYEAR > 2015
AND DOCTYPE (ar OR re)
AND LANGUAGE (english)
```

### 3.2 Kazakhstan/Central Asia Supplementary Query (RQ5)

```
TITLE-ABS-KEY (
  ("Kazakhstan" OR "Central Asia" OR "Uzbekistan" OR "Kyrgyzstan" OR "Tajikistan")
  AND
  ("artificial intelligence" OR "machine learning" OR "e-learning" OR "educational technology")
  AND
  ("education" OR "higher education" OR "university" OR "school")
)
AND PUBYEAR > 2015
AND DOCTYPE (ar OR re)
AND LANGUAGE (english)
```

---

## 4. Inclusion Criteria

| Criterion | Rule |
|-----------|------|
| **I1** | Publication year 2016–2026 |
| **I2** | Document type: Article or Review (peer-reviewed) |
| **I3** | Language: English |
| **I4** | Addresses at least one of: ML/DL for personalized learning (RQ1), gamification + AI (RQ2), LLM + critical thinking (RQ3), recommender/predictive algorithms for academic performance (RQ4), AI in education in Kazakhstan/Central Asia (RQ5) |
| **I5** | Reports empirical results, a systematic review, or a validated framework |

---

## 5. Exclusion Criteria

| Criterion | Rule |
|-----------|------|
| **E1** | Full text permanently inaccessible (closed-access with no preprint or repository alternative); retained at Tier 3 with abstract-proxy quality scoring only |
| **E2** | Not an educational context (pure industrial or clinical ML with no educational application) |
| **E3** | Purely theoretical/mathematical paper with no empirical validation |
| **E4** | Conference abstract or poster (not full peer-reviewed paper) |
| **E5** | Exact duplicate of another included study |
| **E6** | Not in English |
| **E7** | Published before 2016 |

---

## 6. Screening Process

### Stage 1 — Title and Abstract Screening

All 4,547 records (after deduplication: 4,121) were screened by title and abstract using the criteria above. Decisions: **Include**, **Exclude**, **Maybe** (requires full-text), **Pending**.

Stage 1 results:
- Include: 392
- Maybe: 44 (reviewed at Stage 2)
- Exclude: 3,685

### Stage 2 — Full-Text Eligibility

392 papers progressed to full-text review. Stage 2 applied all inclusion/exclusion criteria in detail.

Final eligible: **75 papers** (73 synthesis + 2 background references)

---

## 7. Quality Assessment — MMAT 2018

**Tool:** Mixed Methods Appraisal Tool 2018 (Hong et al., 2018)
**Rater:** Single rater (primary reviewer), with spot-check on 15% of papers

### Scoring

Each paper was scored on five study-type-specific criteria:
- YES = 1 point
- NO or Cannot tell = 0 points
- Total: 0–5

### Quality Tiers

| Tier | Criteria | n |
|------|----------|---|
| Tier 1 | Full text reviewed; MMAT ≥ 4 | 42 |
| Tier 2 | Full text reviewed; MMAT 2–3 | 29 |
| Tier 3 | Closed-access; abstract-proxy score applied | 2 |
| Tier R | Background reference; excluded from synthesis | 2 |

Mean MMAT score (synthesis corpus, n=73): **3.95**

### Sensitivity Analysis

A sensitivity analysis restricted the synthesis to Tier 1+2 papers (n=71; 97.3% of the 73-paper synthesis corpus). Findings across all five RQs were substantively identical, confirming that the two Tier 3 abstract-proxy papers introduced negligible quality bias.

---

## 8. Data Extraction

For each included paper the following fields were extracted:

- DOI
- Title, Year, Journal
- Assigned RQ (one primary)
- MMAT score and tier
- Study type (RCT, quasi-experimental, descriptive, review, LLM benchmark, qualitative, mixed, conceptual)
- Key ML/AI method
- Sample (participants, dataset size, context)
- Key finding relevant to assigned RQ
- Citation count at time of screening (Scopus)

---

## 9. Software and Tools

| Tool | Purpose |
|------|---------|
| Scopus Advanced Search | Database query |
| Microsoft Excel / OpenPyXL | Screening workbooks |
| Python 3.10 (pandas, openpyxl) | Data processing and corpus management |
| PRISMA 2020 checklist | Reporting standard |
| MMAT 2018 | Quality appraisal |

---

## 10. PRISMA 2020 Flow Numbers

| Stage | n |
|-------|---|
| Records identified (Scopus) | 4,547 |
| After deduplication | 4,121 |
| Stage 1 screened | 4,121 |
| Stage 1 excluded | 3,729 |
| Stage 2 assessed for eligibility | 392 |
| Stage 2 excluded | 317 |
| **Included in synthesis** | **75** |

---

## 11. Reference

Hong, Q. N., Fàbregues, S., Bartlett, G., Boardman, F., Cargo, M., Dagenais, P., … Pluye, P. (2018). The Mixed Methods Appraisal Tool (MMAT) version 2018 for information professionals and researchers. *Education for Information*, 34(4), 285–291. https://doi.org/10.3233/EFI-180221
