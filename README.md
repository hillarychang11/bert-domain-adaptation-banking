# BERT Domain Adaptation for Banking Intent Classification

**DATASCI 266 Final Project**  
Hillary Chang  

---

## Overview

This project investigates how well a pretrained BERT model transfers from Amazon product reviews to banking intent classification (BANKING77 dataset).

We analyze:
- Transfer learning performance
- Layer-wise fine-tuning
- Domain mismatch effects
- Comparison with TF-IDF baseline

---

## Key Findings

- TF-IDF baseline (87%) outperforms transfer BERT (79%)
- In-domain BERT achieves highest performance (92%)
- Evidence of **negative transfer** under domain mismatch
- Domain knowledge is distributed across multiple BERT layers

---

## Models Evaluated

- TF-IDF + Logistic Regression
- Last-layer fine-tuning
- Layer-wise fine-tuning (layers 9–11)
- Full fine-tuning
- In-domain BERT

---

## Repository Structure

- `notebooks/` → main Colab notebook
- `results/` → model outputs
- `figures/` → visualizations
- `report/` → final paper

---

## How to Run

Open the notebook in Google Colab:

1. Install dependencies:
```bash
pip install transformers datasets scikit-learn torch
```
2. Run all cells
