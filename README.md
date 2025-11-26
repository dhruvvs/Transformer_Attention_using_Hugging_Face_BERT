<h1 align="center">📘 Transformer Attention Visualization using Hugging Face BERT</h1>

<p align="center">
  <em>Visualizing self-attention patterns across BERT’s layers and heads using Transformers, PyTorch, BertViz, and Matplotlib.</em>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Transformers-HuggingFace-blue?style=for-the-badge&logo=huggingface" />
  <img src="https://img.shields.io/badge/PyTorch-Deep%20Learning-orange?style=for-the-badge&logo=pytorch" />
  <img src="https://img.shields.io/badge/BertViz-Attention%20Visualization-brightgreen?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Matplotlib-Heatmaps-red?style=for-the-badge&logo=python" />
</p>

---

## 📘 Overview

This project demonstrates how to **extract and visualize the self-attention** mechanism of the BERT model.  
You will explore how tokens attend to one another, how meaning is formed across layers, and how to interpret the internal working of Transformer models.

It includes **interactive visualizations** (via BertViz) and **static heatmaps**, making it ideal for NLP interpretability, research, and educational use.

---

## 🚀 Objectives

- Load BERT and extract **attention tensors** from all 12 layers × 12 heads.
- Visualize self-attention interactively using **BertViz**.
- Plot static heatmaps showing token-to-token attention flow.
- Examine how specific tokens (e.g., “bank”) attend to disambiguating context.
- Understand the behavior of Transformer layers for NLP tasks.

---

## 🛠️ Tech Stack

| Category           | Tools & Libraries                                      |
|-------------------|---------------------------------------------------------|
| Language           | Python                                                 |
| Model              | BERT (bert-base-uncased)                               |
| Framework          | PyTorch                                                |
| Visualization      | BertViz, Matplotlib, NumPy                             |
| Tokenization       | Hugging Face Tokenizers                                |
| Development        | Jupyter Notebook / Google Colab                        |
| Environment        | GPU-supported runtime recommended                      |

---

## 🧾 Features

- Extract attention tensors from all BERT layers  
- Full **interactive attention viewer** (BertViz)  
- Static **heatmaps** for any head/layer combination  
- Token-specific attention analysis  
- Support for custom sentences and experimentation  

---

## 📊 Visualizations Included

### ✔ Interactive Attention (BertViz)
- Explore attention for all 12 layers × 12 heads  
- Click on heads to view token-to-token links  
- Visualize cross-token influence and dependencies  

### ✔ Static Heatmaps (Matplotlib)
- Heatmaps showing which tokens attend to which  
- Customizable layer/head selection  
- Intuitive interpretation of attention intensities  

### ✔ Token-Specific Attention Plots
- Extract attention distribution from a selected token  
- Useful for interpretability and report generation  

---
