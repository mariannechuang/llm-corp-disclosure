# **Judging It, Washing It: Scoring and Greenwashing Corporate Climate Disclosures Using Large Language Models**

## **Table of Contents**
- [Project Overview](#project-overview)
- [Data](#data)
- [Key Files](#key-files)
- [Contributing](#contributing)
- [License](#license)

---

## **Project Overview**
This project studies the use of **Large Language Models (LLMs)** to both evaluate and greenwash corporate climate disclosures. We employ two LLM-based scoring methods:
1. **Numerical Rating** – Assigning a score to climate disclosures on a scale (e.g., 1–5).
2. **Pairwise Comparison** – Comparing two disclosures to determine which is more environmentally responsible.

Additionally, we analyze how an LLM modifies disclosures when prompted to **greenwash** responses under accuracy and length constraints.

---

## **Data**
We use data from the **Carbon Disclosure Project (CDP)**, which collects voluntary climate disclosures annually. Since 2013, CDP has maintained an “A-List” of companies demonstrating leadership in climate transparency and action.

We focus on responses to two key questions from the **"Targets and Performance"** section of the CDP Climate Change Questionnaire:
- **4.1a:** Provide details of your absolute emissions target(s) and progress.
- **4.1b:** Provide details of your emissions intensity target(s) and progress.

**Dataset Details:**
- **Source:** CDP 2022
- **Total Companies:** 8,385 (globally)
- **European Companies:** 2,398
- **Subset Used:** 1,416 European companies that responded to **Q4.1a** and/or **Q4.1b**
- **A-List Companies:** 147

---


## **Key Files**

| File | Description |
|------|------------|
| `sample_dataset.csv` | Sample dataset with 5 companies and their responses |
| `sample_a_list.csv` | Sample List of A List Companies |
| `sample_non_a_list.csv` | Sample List of Non A List Companies |
| `pairwise_comparisons.ipynb` | Compares company responses using pairwise method  |
| `pairwise_postprocessing.ipynb` | Analyze pairwise comparison results (TVD, EMD, KS) |
| `greenwashing_prompts.ipynb` | Greenwashes company responses 3 different ways |
| `greenwashing_postprocessing.ipynb` | Analyzes results before vs after greenwashing modifications |

---
