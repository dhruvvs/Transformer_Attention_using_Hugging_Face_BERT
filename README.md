📘 Transformer Attention Visualization using Hugging Face BERT

Understanding Self-Attention Through Interactive & Static Visualizations

This project demonstrates how to extract, analyze, and visualize self-attention from a pre-trained BERT model using Hugging Face Transformers, PyTorch, BertViz, and Matplotlib.
You learn how BERT “looks” at different tokens, how attention changes across layers and heads, and how to build meaningful visualizations for NLP interpretability.

🚀 Overview

Transformers power most modern NLP systems, and self-attention is their core mechanism.
In this project, you will:

Load a BERT base model (bert-base-uncased)

Extract its attention tensors

Visualize attention using:
✔ BertViz (interactive)
✔ Matplotlib heatmaps
✔ Token-focused attention plots

Interpret why certain words attend to others

Understand how BERT processes context and meaning

This project is based on my notebook and documentation:
“Visualize Transformer Attention using Hugging Face BERT”.

📂 Tech Stack
Layer	Tools Used	Purpose
Model Hub	Hugging Face Transformers	Load BERT, return attentions
Backend	PyTorch	Model inference
Visualization (Interactive)	BertViz	Explore layers × heads
Visualization (Static)	Matplotlib, NumPy	Heatmaps & token-level charts
Runtime	Google Colab / Local Python	GPU support & easy execution
📦 Installation
Install Requirements
pip install -U transformers torch bertviz matplotlib numpy

🧠 Key Concepts You Learn
✔ BERT’s attention structure

Each attention tensor has shape:
(layers, heads, seq_len, seq_len)

✔ Understanding attention

Row i → where token i sends attention

Column j → how much token j is attended to

Deeper layers = more semantic patterns

Heads specialize (syntax, position, disambiguation)

✔ Visualizing attention

Interactive graph for each head

Heatmap per layer/head

Token-specific attention distribution (e.g., “bank” → “deposit”, “money”)

📓 Notebook Walkthrough
1️⃣ Install & import dependencies
2️⃣ Load tokenizer & model with output_attentions=True
3️⃣ Tokenize sample sentence

Example:

"He went to the bank to deposit money."

4️⃣ Run BERT forward pass

Extract:

attentions[layer][batch, head, from, to]

5️⃣ Interactive Visualization (BertViz)

Explore 12 layers × 12 heads
Click any head to view token-to-token attention links.

6️⃣ Static Heatmaps

Plot attention matrices using Matplotlib.

7️⃣ Token-specific attention

See which tokens a specific word (e.g., bank) attends to strongly.

📊 Example Outcomes
✔ Find which tokens clarify meaning

For ambiguous words like bank, attention highlights contextual words:
deposit, money

✔ Visualize global context

Special tokens like [CLS] gather global sentence information.

✔ Understand specialization

Some heads track structure, others track long-range dependencies.

▶️ Running Instructions
Google Colab (Recommended)

Upload .ipynb

Run cells sequentially

Explore attention using BertViz

Local Python
python Transformer_Attention.ipynb


(open in Jupyter or VS Code)

📁 Suggested Repository Structure
📦 transformer-attention-bert
 ┣ 📄 README.md
 ┣ 📓 Transformer_Attention.ipynb
 ┣ 📄 Transformers-attention.docx
 ┗ 📁 images/ (optional example screenshots)

🚀 Future Enhancements

Add RoBERTa, DistilBERT, ALBERT comparisons

Combine attention across layers

Visualize attention before vs after fine-tuning

Export visualizations automatically

📜 License

MIT License — free to use, modify, and share.
