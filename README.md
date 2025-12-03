# Emerging AI Research Trend Analysis from arXiv for Datacraft

## Business Context

AI research output on arXiv grows at a pace that makes manual tracking unrealistic. Datacraft needs a structured, data-driven way to understand which areas of AI research are gaining momentum so the organization can anticipate technological shifts, guide R&D priorities, and support clients with timely insights.

This project provides an initial analytical foundation: a reproducible workflow that ingests arXiv metadata, cleans text, extracts meaningful linguistic signals using TF-IDF and bigram analysis, and examines publication trends over time. The goal is to surface early indicators of emerging AI themes without overcomplicating the pipeline.

---

## Technical Overview

The notebook implements a set of transparent, defensible techniques focused on metadata processing, text analysis, and temporal exploration.

### 1. Data Ingestion and Preparation
- Loaded arXiv metadata (titles, abstracts, categories, timestamps).
- Normalized date formats and cleaned missing or inconsistent entries.
- Standardized category labels to support category-level trend analysis.

### 2. Text Cleaning and Token Engineering
- Lowercased textual content and removed punctuation and stopwords.
- Tokenized abstracts to produce unigrams and bigrams.
- Prepared structured token lists suitable for statistical term analysis.

### 3. TF-IDF Term Weighting
- Constructed TF-IDF matrices from cleaned abstracts.
- Identified terms with strong discriminative power across the corpus.
- Used TF-IDF outputs to highlight terminology gaining prominence in recent papers.

### 4. Bigram Frequency Analysis
- Generated frequency distributions for bigrams.
- Surfaced recurring phrase patterns characteristic of active research areas.
- Provided interpretable lexical signals without requiring full topic modeling.

### 5. Temporal Trend Exploration
- Aggregated publication volume over time (daily and monthly).
- Visualized growth patterns in AI-related categories.
- Examined shifts in TF-IDF terms and bigrams across time windows to detect emerging conceptual trends.

---

## Impact

This analysis forms a solid baseline for detecting emerging AI research directions within arXiv. The combination of TF-IDF scoring, bigram analysis, and temporal exploration provides Datacraft with early signals of fast-moving research areas. The pipeline is reproducible, extensible, and ready to support more advanced NLP or modeling techniques in future iterations.
