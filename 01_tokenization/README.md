# 01 · Tokenization & Data

LLMs don't read text — they read **numbers**. This chapter is about turning raw text into token IDs, and token IDs into training batches.

## What's covered

- **Text preprocessing** — splitting raw text into tokens with regex
- **Building a vocabulary** — mapping every unique token to an integer ID
- **`SimpleTokenizerV1`** — a from-scratch encoder/decoder with special tokens (`<|unk|>`, `<|endoftext|>`)
- **Byte Pair Encoding (BPE)** — using OpenAI's `tiktoken` (GPT-2 encoding)
- **Input–target pairs** — the sliding-window trick that teaches the model to predict the next token
- **`GPTDatasetV1` + DataLoader** — batching sequences for training
- **Token embeddings** — turning token IDs into dense vectors with `nn.Embedding`

## Key takeaways

- A tokenizer is just a **two-way dictionary** between text and integers.
- BPE handles unknown words by breaking them into subword pieces — no `<|unk|>` needed.
- Next-token prediction: given `[40, 367, 2885]`, predict `1464`. That's the whole game.
- Embeddings give each token a learnable vector representation.

## Data

Uses `../data/the-verdict.txt` (a short public-domain story). The first cell auto-downloads it if missing.

## Run it

```bash
jupyter notebook tokenizer.ipynb
```
