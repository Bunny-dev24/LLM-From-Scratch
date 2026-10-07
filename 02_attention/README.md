# 02 · Attention Mechanisms

The heart of the transformer. This chapter builds **self-attention** from scratch — the mechanism that lets a model weigh how much each token should "pay attention" to every other token — and works all the way up to **multi-head attention**, the exact block that powers GPT-style LLMs.

## What's covered

- **Attention scores** — raw similarity between a query token and every input token via dot products
- **Softmax weights & context vectors** — normalizing scores into weights that sum to 1, then blending inputs into a context-aware vector
- **Vectorized attention** — replacing loops with matrix multiplication to process every token at once
- **Trainable weights (Q, K, V)** — projecting inputs into query, key, and value spaces so the model *learns* what "relevant" means
- **Scaled dot-product attention** — dividing scores by √d_k for stable training
- **Causal masking** — hiding future tokens with a triangular mask so the model can't cheat at next-token prediction
- **`CausalAttention` class** — a reusable `nn.Module` with `nn.Linear` projections, a registered mask buffer, and dropout, working on batched 3D input
- **`MultiHeadAttentionWrapper`** — running several attention heads in parallel and projecting their concatenated output

## Key takeaways

- Attention = "for each token, how relevant is every other token?"
- The dot product is a simple measure of similarity between two vectors.
- Query, Key, Value: a query is what a token looks for, a key is what it offers, a value is the info it passes along.
- Scaling by √d_k keeps softmax from becoming too "peaky" and killing gradients.
- Causal masking is why GPT can only read left to right.
- Multi-head attention lets each head specialize in a different kind of relationship.

## Files

- `attention.ipynb` — the full, runnable notebook with step-by-step markdown notes
- `medium-article.md` — a beginner-friendly write-up of this chapter

## Run it

```bash
jupyter notebook attention.ipynb
```

## Next up

Chapter 03 — the **Transformer Block**: wrapping multi-head attention with layer normalization, a feed-forward network, and residual connections.
