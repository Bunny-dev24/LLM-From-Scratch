# 🧠 Building an LLM from Scratch

> A hands-on, chapter-by-chapter journey where I build a Large Language Model **from the ground up** — no magic, no black boxes. Just raw PyTorch, math, and a lot of curiosity.
>
> 📅 **One complete concept, every single day.** I learn a concept, code it up, commit it here, and publish a matching **Medium article** — so this repo grows daily, in public.

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10+-blue.svg" alt="Python">
  <img src="https://img.shields.io/badge/PyTorch-2.x-ee4c2c.svg" alt="PyTorch">
  <img src="https://img.shields.io/badge/Status-In%20Progress-yellow.svg" alt="Status">
  <img src="https://img.shields.io/badge/License-MIT-green.svg" alt="License">
  <img src="https://img.shields.io/badge/Updated-Daily-brightgreen.svg" alt="Updated Daily">
</p>

---

## 📖 About

This repository documents my journey of building a GPT-style Large Language Model **from scratch**, one concept at a time. Every chapter is a self-contained notebook that explains the *what*, the *why*, and the *how* — with runnable code and clear notes.

The goal: understand **every single component** of a modern LLM, from turning text into numbers all the way to a working transformer.

---

## 📅 Build in Public — Daily

This is a **learn-in-public** project. My daily rhythm:

1. 📚 **Learn** one complete concept (one focused topic per day)
2. 💻 **Code** it from scratch in a notebook and push it here
3. ✍️ **Write** a matching article on **Medium** explaining it in simple terms
4. ✅ **Commit** daily — so progress is visible, consistent, and accountable

> New code and a new article land here almost every day. Follow along, and feel free to learn alongside me!

📝 **Medium articles:** _coming soon — link will be added here_

---

## 🗺️ Roadmap

| #  | Chapter | What's inside | Status |
|----|---------|---------------|--------|
| 00 | [PyTorch Fundamentals](./00_pytorch_fundamentals) | Tensors, autograd, building an MLP, parameters & seeds | ✅ Done |
| 01 | [Tokenization & Data](./01_tokenization) | Simple tokenizer, BPE (tiktoken), dataloaders, embeddings | ✅ Done |
| 02 | [Attention Mechanisms](./02_attention) | Self-attention from scratch, attention scores | 🚧 In progress |
| 03 | Transformer Block | Multi-head attention, layer norm, feed-forward | ⏳ Planned |
| 04 | GPT Model | Assembling the full GPT architecture | ⏳ Planned |
| 05 | Pretraining | Training loop, loss, text generation | ⏳ Planned |
| 06 | Fine-tuning | Classification & instruction fine-tuning | ⏳ Planned |

---

## 📂 Repository Structure

```
LLM-From-Scratch/
├── data/                        # Shared datasets (the-verdict.txt)
├── 00_pytorch_fundamentals/     # PyTorch basics: autograd, MLPs
├── 01_tokenization/             # Tokenizers, BPE, dataloaders, embeddings
├── 02_attention/                # Attention mechanisms from scratch
├── assets/                      # Images & diagrams for notes
├── requirements.txt            # Python dependencies
└── README.md
```

---

## 🚀 Getting Started

```bash
# 1. Clone the repo
git clone https://github.com/Bunny-dev24/LLM-From-Scratch.git
cd LLM-From-Scratch

# 2. (Recommended) Create a virtual environment
python -m venv .venv
source .venv/bin/activate      # Windows: .venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Launch Jupyter and start from chapter 00
jupyter notebook
```

---

## 🛠️ Tech Stack

- **PyTorch** — tensors, autograd, neural network building blocks
- **tiktoken** — OpenAI's fast BPE tokenizer (GPT-2 encoding)
- **Jupyter** — interactive, explained notebooks

---

## 🙏 Acknowledgements

This series is inspired by Sebastian Raschka's excellent book *"Build a Large Language Model (From Scratch)"*. The code here is my own re-implementation and notes written while learning.

---

## 📜 License

This project is licensed under the [MIT License](./LICENSE).

---

<p align="center">⭐ If you find this helpful, consider starring the repo — it keeps me motivated to ship the next chapter!</p>
