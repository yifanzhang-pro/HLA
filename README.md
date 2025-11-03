# HLA: Higher-order Linear Attention

[![arXiv](https://img.shields.io/badge/arXiv-2510.27258-b31b1b.svg)](https://arxiv.org/abs/2510.27258) 
[![Website](https://img.shields.io/badge/Project-Website-blue)](https://yifanzhang-pro.github.io/HLA) 
[![License: CC-BY](https://img.shields.io/badge/License-CC_BY_4.0-yellow.svg)](https://creativecommons.org/licenses/by/4.0) 

### Higher-order Linear Attention

A causal, streaming attention mechanism that realizes higher‑order interactions via compact prefix statistics, with exact masked identities and associative scans enabling parallel training that matches recurrent computations.

## Abstract

The quadratic cost of scaled dot-product attention is a central obstacle to scaling autoregressive language models to long contexts. Linear-time attention and State Space Models (SSMs) provide scalable alternatives but are typically restricted to first-order or kernel-based approximations, which can limit expressivity. We introduce **Higher-order Linear Attention** (**HLA**), a causal, streaming mechanism that realizes higher interactions via compact prefix sufficient statistics. In the second-order case, HLA maintains a constant-size state and computes per-token outputs in linear time without materializing any $n \times n$ matrices. We give closed-form streaming identities, a strictly causal masked variant using two additional summaries, and a chunk-parallel training scheme based on associative scans that reproduces the activations of a serial recurrence exactly. We further outline extensions to third and higher orders. Collectively, these results position HLA as a principled, scalable building block that combines attention-like, data-dependent mixing with the efficiency of modern recurrent architectures.

## Citation

```bibtex
@article{zhang2025higher,
   title   = {Higher-order Linear Attention},
   author  = {Zhang, Yifan and Qin, Zhen and Gu, Quanquan},
   journal = {arXiv preprint arXiv:2510.27258},
   year    = {2025}
}
```
