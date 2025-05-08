# **Judging It, Washing It: Scoring and Greenwashing Corporate Climate Disclosures Using Large Language Models**

## **Table of Contents**
- [Project Overview](#project-overview)
- [Data](#data)
- [Usage](#usage)
- [Methodology](#methodology)
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

## **Usage**
To run the analysis, follow these steps:

---

## **Methodology**
1. **Preprocessing:** Cleaning raw CDP data, filtering for **European companies**, and structuring responses.
2. **Scoring:** Using LLMs to assign **numerical ratings** or **pairwise comparisons** to disclosures.
3. **Greenwashing Analysis:** Rewriting disclosures using an LLM while preserving factual accuracy.
4. **Evaluation:** Comparing original vs. greenwashed responses to identify potential biases.

---

## **Key Files**

| File | Description |
|------|------------|
| `company_information.ipynb` | Counts companies that respond to one/both/neither questions, counts A List companies with invalid responses, Filters out (and counts) European companies with valid responses, and saves it into new files. |
| `preprocessing.ipynb` | This file filters companies with N/A or empty values, filters out European countries, and also provides information on number of companies in each sector/industry |
| `rating_companies.ipynb` | idk |
| `pairwise_new_prompting.ipynb` | Compares company disclosures using ...  |
| `greenwashing_postprocessing.ipynb` | Applies LLM-based modifications to "greenwash" corporate disclosures. |
| `pairwise_postprocessing.ipynb` | Analyzes pairwise comparison results after greenwashing modifications. |
| `pairwise_postprocessing.ipynb` | Analyzes pairwise comparison results after greenwashing modifications. |
| `rating_over_years.ipynb` | idk. |
| `industry_counts.ipynb` |  |
| `malicious_greenwashing.ipynb` |  |

---

## **Contributing**


---

## **License**


---
