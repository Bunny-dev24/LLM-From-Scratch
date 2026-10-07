# 02 · Attention Mechanisms

The heart of the transformer. This chapter builds **self-attention** from scratch — the mechanism that lets a model weigh how much each word should "pay attention" to every other word.

## What's covered

- **Attention scores** — computing raw similarity between a query token and every input token via dot products
- *(Coming next)* Normalizing scores with softmax → attention weights
- *(Coming next)* Context vectors, trainable weights (W_q, W_k, W_v)
- *(Coming next)* Causal masking & multi-head attention

## Key takeaways

- Attention = "for each token, how relevant is every other token?"
- The dot product is a simple measure of similarity between two vectors.

## Run it

```bash
jupyter notebook attention.ipynb
```

> 🚧 This chapter is a work in progress — more to come!
