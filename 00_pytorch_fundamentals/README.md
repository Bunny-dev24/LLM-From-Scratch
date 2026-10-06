# 00 · PyTorch Fundamentals

Before building an LLM, we need to be fluent in the tool that powers it: **PyTorch**.

## What's covered

- **Logistic regression forward pass** — sigmoid activation + binary cross-entropy loss
- **Autograd** — computing gradients automatically with `torch.autograd.grad`
- **Multilayer Perceptron (MLP)** — a 2-hidden-layer network using `nn.Module` and `nn.Sequential`
- **Counting parameters** — how many trainable weights a model has
- **Reproducibility** — using `torch.manual_seed` for deterministic results

## Key takeaways

- Tensors are the core data structure; autograd tracks operations to compute gradients.
- `requires_grad=True` tells PyTorch to build a computation graph for a tensor.
- Every neural network subclasses `nn.Module` and defines a `forward()` method.

## Run it

```bash
jupyter notebook pytorch_fundamentals.ipynb
```
