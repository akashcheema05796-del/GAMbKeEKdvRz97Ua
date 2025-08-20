# Customer Happiness Prediction (Logistics & On-Demand Delivery)

> **Repo name:** `GAMbKeEKdvRz97Ua`  
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



---

## Project Goal

Predict **customer happiness (`Y`)** from the six survey responses (`X1…X6`).

---





```bash
# clone (use the exact repo name below)
git clone https://github.com/<your-org-or-user>/KWIEwhqDqoesO7Fq.git
cd KWIEwhqDqoesO7Fq

# create & activate a virtual env
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate

# install deps
pip install -r requirements.txt
