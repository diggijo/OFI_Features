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

- `ofi_constructor.py` — Python class implementing OFI feature calculations  
- `example_data.csv` — Sample dataset (replace with your own data)  
- `ofi_analysis.pdf` — PDF with conceptual questions and explanations  
- `README.md` — This file  

---

## Usage

1. Load your order book data into a pandas DataFrame with appropriate columns (`bid_sz_00`, `ask_sz_00`, ..., `symbol`, `ts_event`, etc.).

2. Instantiate the `OFIConstructor` class with your DataFrame.

3. Call the methods to calculate OFI features:

```python
ofi = OFIConstructor(df)
best_level_ofi = ofi.calculate_best_level_ofi()
multi_level_ofi = ofi.calculate_multi_level_ofi()
integrated_ofi = ofi.calculate_integrated_ofi()
cross_asset_ofi = ofi.calculate_cross_asset_ofi()
