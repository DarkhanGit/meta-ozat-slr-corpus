# Search Protocol — Meta_Ozat SLR (AP25796141)

**Protocol version:** 1.1
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
| Scopus | Primary (5 targeted RQ queries; deduplicated via master OR query) | 9,281 → 4,396 after dedup |
| OpenAlex | Parallel aggregator (covers Scopus, WoS, PubMed, DOAJ, Crossref) | 4,152 |
| IEEE Xplore | Supplementary — RQ5 Kazakhstan/Central Asia snowballing | Included in +9 |
| Google Scholar | Supplementary — RQ5 snowballing | Included in +9 |
| ERIC | Supplementary — RQ5 snowballing | Included in +9 |
| CyberLeninka | Supplementary — RQ5 Russian-language indexed sources | Included in +9 |

---

## 3. Search Query

### 3.1 Scopus Master Query (Primary)

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

### 3.2 RQ-Specific Scopus Queries (5 targeted strings)

**RQ1 — ML architectures for personalized learning paths:**
```
TITLE-ABS-KEY (
  ("deep learning" OR "transformer" OR "knowledge tracing" OR "graph neural network"
   OR "GNN" OR "BERT" OR "reinforcement learning" OR "NLP" OR "adaptive learning")
  AND ("personalized learning" OR "learning path" OR "learning trajectory"
       OR "student model" OR "content recommendation")
  AND ("higher education" OR "university" OR "e-learning" OR "MOOC")
)
AND PUBYEAR > 2015 AND DOCTYPE (ar OR re) AND LANGUAGE (english)
```
*Retrieved: ~3,305 records*

**RQ2 — Gamification integrated with AI:**
```
TITLE-ABS-KEY (
  ("gamification" OR "game-based learning" OR "serious games" OR "points badges leaderboards"
   OR "gamified" OR "adaptive gamification")
  AND ("artificial intelligence" OR "machine learning" OR "adaptive system"
       OR "recommender" OR "personalized")
  AND ("engagement" OR "motivation" OR "learning outcomes" OR "student performance")
)
AND PUBYEAR > 2015 AND DOCTYPE (ar OR re) AND LANGUAGE (english)
```
*Retrieved: ~984 records*

**RQ3 — LLM/NLP tools and critical thinking:**
```
TITLE-ABS-KEY (
  ("large language model" OR "LLM" OR "ChatGPT" OR "GPT-4" OR "GPT-3" OR "BERT"
   OR "natural language processing" OR "NLP" OR "argumentation mining")
  AND ("critical thinking" OR "argumentation" OR "reasoning" OR "higher-order thinking"
       OR "metacognition")
  AND ("education" OR "higher education" OR "university" OR "student")
)
AND PUBYEAR > 2015 AND DOCTYPE (ar OR re) AND LANGUAGE (english)
```
*Retrieved: ~2,319 records*

**RQ4 — Recommender/predictive algorithms for academic performance:**
```
TITLE-ABS-KEY (
  ("recommender system" OR "collaborative filtering" OR "knowledge graph"
   OR "graph neural network" OR "deep knowledge tracing" OR "random forest"
   OR "gradient boosting" OR "XGBoost" OR "neural network" OR "SVM")
  AND ("academic performance" OR "student performance" OR "learning outcome"
       OR "dropout prediction" OR "grade prediction" OR "performance prediction")
  AND ("education" OR "university" OR "e-learning" OR "LMS" OR "Moodle")
)
AND PUBYEAR > 2015 AND DOCTYPE (ar OR re) AND LANGUAGE (english)
```
*Retrieved: ~2,194 records*

**RQ5 — AI in education in Kazakhstan and Central Asia:**
```
TITLE-ABS-KEY (
  ("Kazakhstan" OR "Central Asia" OR "Uzbekistan" OR "Kyrgyzstan" OR "Tajikistan"
   OR "Turkmenistan" OR "Eurasia")
  AND ("artificial intelligence" OR "machine learning" OR "e-learning"
       OR "educational technology" OR "adaptive learning" OR "gamification")
  AND ("education" OR "higher education" OR "university" OR "school")
)
AND PUBYEAR > 2015 AND DOCTYPE (ar OR re) AND LANGUAGE (english)
```
*Retrieved: ~479 records*

*Total across 5 queries: 9,281 | After master OR deduplication: 4,396 (exported April 4, 2026)*

---

## 4. Inclusion Criteria

| Criterion | Rule |
|-----------|------|
| **I1** | Publication year 2016–2026 (search executed through April 4, 2026; Scopus export date) |
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
| **E7** | Published before 2016 or after April 4, 2026 (Scopus export date) |

---

## 6. Screening Process

### Stage 1 — Title and Abstract Screening

All 3,986 records (after combined Scopus + OpenAlex deduplication) were screened by title and abstract using the criteria above. Decisions: **Include**, **Exclude**, **Maybe** (requires full-text), **Pending**.

Stage 1 results:
- Passed (Include + Maybe): **300**
- Excluded: 3,686

### Stage 2 — Full-Text Eligibility

300 papers progressed to full-text review. Stage 2 applied all inclusion/exclusion criteria in detail.

Stage 2 results:
- Eligible from database search: **73 papers**
- Snowballing (RQ5 supplementary — IEEE Xplore, Google Scholar, ERIC, CyberLeninka): **+9 papers**
- **Final synthesis corpus: 82 papers**

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
| Tier 1 | Full open-access text reviewed; MMAT ≥ 4 | 43 |
| Tier 2 | Full-text reviewed, MMAT 2–3; OR MMAT ≥ 4 via institutional/closed access; OR supplementary snowballing additions | 37 |
| Tier 3 | Closed-access only; abstract-proxy MMAT score ≥ 3 applied | 2 |
| Tier R | Background reference; excluded from synthesis | 2 |

**Mean MMAT score (synthesis corpus, n=82): 3.88**

### Sensitivity Analysis

A sensitivity analysis restricted the synthesis to Tier 1+2 papers (n=80; 97.6% of the 82-paper synthesis corpus). Findings across all five RQs were substantively identical, confirming that the two Tier 3 abstract-proxy papers introduced negligible quality bias.

---

## 8. Data Extraction

For each included paper the following fields were extracted:

- DOI
- Title, Year, Journal
- Assigned RQ (primary; some papers assigned to two RQs)
- MMAT score (0–5) and tier
- Study type (RCT, quasi-experimental, descriptive, review, LLM benchmark, qualitative, mixed, conceptual)
- Key ML/AI method
- Sample (participants, dataset size, context)
- Key finding relevant to assigned RQ
- Citation count at time of screening (Scopus)

---

## 9. Software and Tools

| Tool | Purpose |
|------|---------|
| Scopus Advanced Search | Primary database query (5 RQ strings + master OR) |
| OpenAlex API | Parallel search and cross-validation |
| Microsoft Excel / OpenPyXL | Screening workbooks |
| Python 3.10 (pandas, openpyxl) | Data processing and corpus management |
| PRISMA 2020 checklist | Reporting standard |
| MMAT 2018 | Quality appraisal |

---

## 10. PRISMA 2020 Flow Numbers

| Stage | n |
|-------|---|
| Records identified — Scopus (5 RQ queries, before dedup) | 9,281 |
| After Scopus deduplication (master OR query) | 4,396 |
| Records identified — OpenAlex parallel | 4,152 |
| After combined deduplication | 3,986 |
| Stage 1 screened (Title/Abstract) | 3,986 |
| Stage 1 excluded | 3,686 |
| Stage 2 assessed for eligibility (Full-text) | 300 |
| Stage 2 excluded | 227 |
| Snowballing (RQ5 supplementary) | +9 |
| **Included in synthesis** | **82** |

**Cross-validation:** 85.4% of final corpus (70/82 papers) confirmed present in Scopus export (scopus_export_Apr 4-2026.csv, n=4,396 records).

---

## 11. Reference

Hong, Q. N., Fàbregues, S., Bartlett, G., Boardman, F., Cargo, M., Dagenais, P., … Pluye, P. (2018). The Mixed Methods Appraisal Tool (MMAT) version 2018 for information professionals and researchers. *Education for Information*, 34(4), 285–291. https://doi.org/10.3233/EFI-180221
