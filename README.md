# cultural-perspective-diversity
Experimental code and materials for studying perspective diversity in large language models under cultural-aware and pluralistic prompting.
# Cultural-Aware vs. Pluralistic Prompting

Experimental code and materials for the term paper:

**Cultural-Aware vs. Pluralistic Prompting: An Empirical Study of Perspective Diversity in Large Language Models**

## Overview

This repository contains the experimental code, configuration, data,
and result files used to investigate whether inference-time prompting
can increase the diversity of perspectives expressed by large
language models (LLMs).

The experiment compares three prompting conditions:

- **Baseline**
- **Cultural-aware**
- **Pluralistic**

The same set of 40 culturally variable questions was used across all
three conditions, resulting in 120 generated responses.

## Experimental Setup

- **Generation model:** `gpt-4o-mini`
- **Evaluation model:** `claude-sonnet-4-5-20250929`
- **Number of questions:** 40
- **Prompting conditions:** 3
- **Total generated responses:** 120
- **Generation temperature:** 0.7
- **Maximum output tokens:** 450
- **Target response length:** approximately 170–180 words
- **Response length range:** 150–200 words

## Evaluation

The generated responses were evaluated on three outcomes:

1. **Perspective diversity**
2. **Pluralistic framing**
3. **Cultural stereotyping**

A stratified sample of 20 responses was also manually annotated
for human validation of the automated evaluation.

## Repository Structure

```text
├── experiment.ipynb
├── locked_config_final.json
├── data/
│   ├── final_120_evaluated.csv
│   ├── final_120_responses.csv
│   └── human_llm_agreement_comparison_final.csv
├── figures/
│   ├── figure1_diversity_by_condition.png
│   ├── figure2_pluralistic_rate_by_condition.png
│   └── figure4_category_diversity.png
└── results/
    └── final_summary_by_condition.csv
