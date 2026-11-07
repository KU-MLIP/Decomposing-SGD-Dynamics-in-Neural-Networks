# Decomposing SGD Dynamics in Neural Networks: Teacher-Induced Spikes and Variance Inflation

Code for the [NeurIPS 2026 paper](https://openreview.net/forum?id=pCMDLPWcuw) by Samet Demir and Zafer Dogan.

Each figure is produced by one self-contained Jupyter notebook. No datasets are needed:
inputs are synthetic Gaussians drawn inside each notebook. Executed outputs, including the
figures, are kept in the notebooks, so results can be inspected without re-running.

## Contents

| Notebook | Produces | Related result |
|---|---|---|
| `Fig1ab-accumulator.ipynb` | Fig. 1(a)–(b): Frobenius norm and spectral density of the driver accumulator $C_t$ | Lemma 3.1 |
| `Fig1c-gram-spectrum.ipynb` | Fig. 1(c): spectral density of the complement Gram matrix $n_\perp G_t$ | Lemma 3.2, Remark 3.3 |
| `Spike-size.ipynb` | Numbers in "How large are the spikes?" (Sec. 3.1) | Remark 3.3 |
| `Fig2-equivalence.ipynb` | Fig. 2(a)–(c): SGD vs. Decomposed Dynamics across learning rates, widths, and activations | Theorem 3.4 |
| `Fig3-4-comparison.ipynb` | Figs. 3–4: random features, one-step feature learning, SGD, and Decomposed Dynamics; alignment of the layers; reduced parameterization | Sec. 4, Props. 3.5–3.6 |

## Requirements

Python ≥ 3.10 with `numpy`, `matplotlib`, `tqdm`, and `scienceplots`:

```
pip install -r requirements.txt
```

## Citation

```bibtex
@inproceedings{demir2026decomposing,
  title     = {Decomposing {SGD} Dynamics in Neural Networks: Teacher-Induced Spikes and Variance Inflation},
  author    = {Demir, Samet and Dogan, Zafer},
  booktitle = {Advances in Neural Information Processing Systems},
  year      = {2026},
  url       = {https://openreview.net/forum?id=pCMDLPWcuw}
}
```
