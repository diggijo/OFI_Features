# Order Flow Imbalance (OFI) Feature Extraction and Analysis

This repository contains Python code for calculating Order Flow Imbalance (OFI) features from market order book data. It includes implementations for:

- **Best-Level OFI**  
- **Multi-Level OFI**  
- **Integrated OFI** using Principal Component Analysis (PCA)  
- **Cross-Asset OFI** analysis  

---

## Overview

Order Flow Imbalance (OFI) is a useful metric in quantitative finance for measuring buying and selling pressure in the order book. This project demonstrates how to construct OFI features at multiple depth levels and integrate them for improved market insight.

Alongside the code, this repository contains a **LaTeX-generated PDF** summarizing key conceptual questions and answers related to OFI, including:

- Motivation for measuring OFI at multiple levels  
- Why Lasso regression is preferred over OLS for cross-impact estimation  
- Why OFI outperforms trade volume as a short-term return predictor  

---

## Contents

- `OFI_Features.ipyb` — Notebook implementing OFI feature calculations 
- `first_25000_rows.csv` — Sample dataset
- `OFI Conceptual Questions.pdf` — PDF with conceptual questions and explanations  
- `README.md` — This file  

---
