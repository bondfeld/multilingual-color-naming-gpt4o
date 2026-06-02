# Multilingual Color Naming with GPT-4o

Code and data accompanying:

**Lexical Availability and Human Distributional Agreement in GPT-4o's Color Naming**

## Repository Structure

```text
ABC/
├── expABC_pipeline.ipynb
└── Archive.zip

D/
├── D.ipynb
├── metrics_all_languages.csv
├── human_subject_counts_per_language.csv
├── stimuli_master.csv
├── human_bins/
├── raw_llm_outputs/
└── figures/
```

## ABC

Experiments A–C:

* Experiment A: open-vocabulary synthetic hue wheels
* Experiment B: fixed basic-color categories
* Experiment C: human low-chroma hue-line evaluation

`Archive.zip` contains the processed human color-naming files used in these experiments.

## D

Experiment D:

* multilingual full-grid CIELAB evaluation
* nine languages
* Jensen–Shannon divergence
* vocabulary compression
* human category concentration
* cross-linguistic comparisons

## Human Data

Human color-naming data are derived from:

Kim et al. (2019), *Color Names Across Languages: Salient Colors and Term Translation in Multilingual Color Naming Models*.

## Notes

* API credentials have been removed.
* Results can be reproduced from the included notebooks and processed data files.
