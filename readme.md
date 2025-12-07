# RNN & Gradient Flow Teaching Notebook - Refactored

## Refactoring Documentation

This notebook has been refactored to follow software engineering best practices while preserving its pedagogical value.

## Project Structure

| File | Description |
|------|-------------|
| `q_rnn_and_grad.ipynb` | Original teaching notebook |
| `q_rnn_and_grad_refactored.ipynb` | Refactored version with improved code quality |
| `img/` | Supporting figures (1a.png, 1c.png, 1h.png) |

## Notebook Contents

| Section | Topic | Learning Objective |
|---------|-------|-------------------|
| **1.A** | RNNLayer | Implement single-layer RNN: `h_t = σ(W^h h_{t-1} + W^x x_t + b)` |
| **1.B** | RecurrentRegressionModel | Add output layer: `ŷ_t = W^f h_t + b^f` |
| **1.C** | Dataset & Loss | Cumulative average prediction task |
| **1.D** | Gradient Visualization | Explore vanishing/exploding gradients |
| **1.K** | Multi-layer RNN | Stack RNN layers for deeper networks |

## Changes Made

| Category | Change | Reference |
|----------|--------|----------|
| **Formatting** | 2-space → 4-space indentation | [PEP 8](https://peps.python.org/pep-0008/#indentation) |
| **Naming** | `th` → `torch`, `h_list` → `hidden_states` | [PEP 8 - Naming Conventions](https://peps.python.org/pep-0008/#naming-conventions) |
| **Type Hints** | Added to function signatures | [PEP 484](https://peps.python.org/pep-0484/) |
| **Docstrings** | NumPy-style with math formulas | [PEP 257](https://peps.python.org/pep-0257/), [NumPy Docstring Guide](https://numpydoc.readthedocs.io/en/latest/format.html) |
| **Shape Comments** | Added after tensor operations | [PyTorch Best Practices](https://pytorch.org/docs/stable/notes/broadcasting.html) |
| **Constants** | Grouped with documentation | [PEP 8 - Constants](https://peps.python.org/pep-0008/#constants) |
| **Assertions** | Educational messages explaining parameter counts | Improved debugging experience |
| **Environment** | Colab/local compatibility wrapper | Cross-platform support |
| **Reproducibility** | Added random seed | [PyTorch Reproducibility](https://pytorch.org/docs/stable/notes/randomness.html) |

## Style Guides Referenced

- [PEP 8 – Style Guide for Python Code](https://peps.python.org/pep-0008/)
- [PEP 257 – Docstring Conventions](https://peps.python.org/pep-0257/)
- [PEP 484 – Type Hints](https://peps.python.org/pep-0484/)
- [Google Python Style Guide](https://google.github.io/styleguide/pyguide.html)
- [PyTorch Documentation Best Practices](https://pytorch.org/docs/stable/community/design.html)

---

*This refactoring was performed with AI assistance (Claude).*

