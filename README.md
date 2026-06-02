# Multilingual Color Naming with GPT-4o

Code, data, and analysis accompanying:

**Lexical Availability and Human Distributional Agreement in GPT-4o's Color Naming**

This repository contains materials used to evaluate GPT-4o on multilingual color naming tasks ranging from synthetic hue wheels to human color-naming distributions.

---

## Repository Structure

```text
multilingual-color-naming-gpt4o/
│
├── ABC/
│   ├── README.md
│   ├── expABC_pipeline.ipynb
│   ├── color_names.csv
│   ├── english_names.csv
│   ├── russian_names.csv
│   ├── english-cielab.csv
│   └── russian-cielab.csv
│
├── D/
│   ├── README.md
│   ├── D.ipynb
│   ├── metrics_all_languages.csv
│   ├── human_subject_counts_per_language.csv
│   ├── stimuli_master.csv
│   │
│   ├── human_bins/
│   │   ├── human_bins_chinese.csv
│   │   ├── human_bins_english.csv
│   │   ├── human_bins_french.csv
│   │   ├── human_bins_german.csv
│   │   ├── human_bins_korean.csv
│   │   ├── human_bins_polish.csv
│   │   ├── human_bins_portuguese.csv
│   │   ├── human_bins_russian.csv
│   │   └── human_bins_spanish.csv
│   │
│   ├── raw_llm_outputs/
│   │   ├── llm_raw_chinese.csv
│   │   ├── llm_raw_english.csv
│   │   ├── llm_raw_french.csv
│   │   ├── llm_raw_german.csv
│   │   ├── llm_raw_korean.csv
│   │   ├── llm_raw_polish.csv
│   │   ├── llm_raw_portuguese.csv
│   │   ├── llm_raw_russian.csv
│   │   └── llm_raw_spanish.csv
│   │
│   └── figures/
│       └── expD_fullgrid_patches.png
│
└── README.md
```

---

## Experiments A–C (ABC)

The `ABC` directory contains the synthetic hue-wheel and hue-line experiments.

### Experiment A

Open-vocabulary color naming on synthetic hue wheels.

* Languages: English, Russian
* 36 synthetic hue bins
* 100 samples per hue
* Temperatures: 0.3 and 0.9

### Experiment B

Fixed basic-color category naming.

* Languages: English, Russian
* Fixed color inventories
* 20 samples per hue
* Temperature: 0.1

### Experiment C

Human low-chroma hue-line evaluation.

* Languages: English, Russian
* Human naming distributions
* 20 samples per stimulus
* Temperature: 0.7

---

## Experiment D

The `D` directory contains the multilingual full-grid evaluation.

### Languages

* English
* Russian
* Chinese
* Korean
* German
* French
* Spanish
* Polish
* Portuguese

### Main Outputs

* Jensen–Shannon divergence
* Head-level distributions
* Vocabulary compression
* Human category concentration
* Cross-linguistic comparisons

---

## Human Data

Human color-naming data are derived from the multilingual color-naming dataset introduced by:

Kim, Y., Thayer, K., Gorsky, G. S., & Heer, J. (2019). *Color Names Across Languages: Salient Colors and Term Translation in Multilingual Color Naming Models.*

The original corpus is not redistributed in full. Included files contain only the processed subsets required for the experiments reported in the paper.

---

## Notes

* GPT-4o was accessed through the OpenAI API.
* Any API credentials have been removed from the released code.
* Notebook outputs may be cleared to reduce repository size.
* Results reported in the paper can be reproduced from the provided notebooks and processed data files.
