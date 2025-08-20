# Customer Happiness Prediction (Logistics & On-Demand Delivery)

> **Repo name:** `KWIEwhqDqoesO7Fq`  
> **Goal:** Predict whether a customer is **happy (1)** or **unhappy (0)** from a short post-order survey.

---

## Background

We are one of the fastest-growing startups in the logistics and delivery space. We partner with multiple providers to deliver on demand. As we scale globally, we face new operational challenges every day—and we believe the most reliable compass is **customer happiness**.

To improve operations, we must **measure** and **predict** how happy each customer is so we can act before issues escalate. We regularly seek feedback, and recently surveyed a select customer cohort. This repository contains a **public subset** of that survey; the rest remains a **private test set** for evaluation.

---

## Data Description

Each row represents one customer’s responses to a short Likert-scale survey (1–5). Higher numbers indicate stronger agreement/greater satisfaction.

| Column | Meaning |
| --- | --- |
| `Y` | Target label: `0 = unhappy`, `1 = happy` |
| `X1` | “My order was delivered on time.” |
| `X2` | “Contents of my order were as I expected.” |
| `X3` | “I ordered everything I wanted to order.” |
| `X4` | “I paid a good price for my order.” |
| `X5` | “I am satisfied with my courier.” |
| `X6` | “The app makes ordering easy for me.” |

**Scale:** 1 (low) → 5 (high)

### Download
Public subset (CSV):  
https://drive.google.com/open?id=1KWE3J0uU_sFIJnZ74Id3FDBcejELI7FD

> We will evaluate on a **private hold-out** split.

---

## Project Goal

Predict **customer happiness (`Y`)** from the six survey responses (`X1…X6`).

### Success Metric

- **Primary:** Accuracy ≥ **73%** on our private test set **or** a compelling argument—with evidence—why your approach is superior (e.g., better calibration, fairness, stability, interpretability, or business impact).

---

## Bonus: Feature Importance & Minimal Question Set

We’re especially interested in **which questions matter most**.  
Please explore and report:

- **Feature importance** (e.g., permutation importance, SHAP, model-specific importances).  
- A **minimal subset** of questions that preserves predictive power while reducing survey length.  
- Clear recommendations: *Which question(s) could be removed in future surveys?* What trade-offs (accuracy vs. survey length) do you observe?

---

## Getting Started

### Requirements (suggested)
- Python 3.9+
- [`pandas`](https://pandas.pydata.org/)
- [`numpy`](https://numpy.org/)
- [`scikit-learn`](https://scikit-learn.org/stable/)
- Optional: `matplotlib`, `shap`

```bash
# clone (use the exact repo name below)
git clone https://github.com/<your-org-or-user>/KWIEwhqDqoesO7Fq.git
cd KWIEwhqDqoesO7Fq

# create & activate a virtual env
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate

# install deps
pip install -r requirements.txt
