# Classification results

The `efsa` and `pubmed` directories contain classification results for 50 randomly chosen articles from each dataset.

Each directory contains the following files:
- `testcases.csv` – identifiers and titles of articles used to perform the classification. The full abstracts are not included due to licensing concerns.
- `0`–`49.csv` – classification results for each article. Columns:
  - `uri` – the URI of the found entity
  - `lemma` – lemmatized forms of mentions in the abstract that led to identifying the entity.
  - `lemma_nunique` – number of unique mention lemmas for the entity.
  - `lemma_count` – number of all mentions in the abstract for the entity.
  - `score_max` – out of all identified mentions, the maximum similarity score between it and the entity.
  - `score_mean` – mean similarity score between the mentions and the entity.
  - `score2` – the final combined score for the entity.
  - The remaining columns (e.g., `label`, `chebi_formula`) correspond to text properties of the entity.