# Empirical Dynamic Modeling (EDM)

<img src="assets/logo-lorenz.svg" align="right" height="200px" width="200px" alt="logo" />

Welcome to the home of **Empirical Dynamic Modeling (EDM)** — a suite of statistical software packages for **causal analysis of time series data** using modern nonlinear techniques like **Convergent Cross Mapping (CCM)**.

These packages are available in:

<p style="display: flex; gap: 1rem; flex-wrap: wrap;">
  <a href="https://edm-developers.github.io/edm-stata/" class="md-button md-button">📘 Stata</a>
  <a href="https://edm-developers.github.io/fastEDM-python/" class="md-button">🐍 Python</a>
  <a href="https://edm-developers.github.io/fastEDM-r/" class="md-button">📊 R</a>
</p>

All three are built on a shared high-performance **C++ backend**, ensuring consistent behavior across platforms.

---

## 🧠 What is EDM?

EDM is a framework for modeling **complex dynamic systems** directly from data — no need for linear assumptions or fixed model structures. Instead, it reconstructs system dynamics using time-delay embeddings and evaluates causal links using tools like **CCM**.

For the theoretical background and methods, we recommend:

- 📄 [Stata Journal paper (Li et al., 2021)](https://jinjingli.github.io/edm/edm-wp.pdf),
- 🎥 [QMNET Seminar (YouTube)](https://youtu.be/kZv85k1YUVE),
- 📝 [Slides from the talk](https://edm-developers.github.io/edm-stata/pdfs/EDM-talk-QMNET.pdf).

---

## 🚀 Installation

You can install each package using the instructions below:

???+ note "Stata"
    ```stata
    ssc install edm, replace
    edm update, development replace
    ```

???+ note "Python"
    ```bash
    pip install 'fastEDM @ git+https://github.com/EDM-Developers/fastEDM-python'
    ```

???+ note "R"
    ```r
    # install.packages("devtools")
    devtools::install_github("EDM-Developers/fastEDM-r")
    ```

---

## 🔍 Where to Learn More?

Each language has its own documentation site:

- [**Stata package**](https://edm-developers.github.io/edm-stata/): Most comprehensive, includes GPU support and multiple distance functions.
- [**Python package**](https://edm-developers.github.io/fastEDM-python/): Simple to use, minimal interface.
- [**R package**](https://edm-developers.github.io/fastEDM-r/): R-native wrapper around the same backend.

The Stata package currently offers the most complete feature set, so we recommend starting there if you're new to EDM.

---

## 📚 Citation

If you use any of these packages, please cite the following paper:

``` bibtex
@article{edm-stata,
  title={Beyond linearity, stability, and equilibrium: The edm package for empirical dynamic modeling and convergent cross-mapping in {S}tata},
  author={Li, Jinjing and Zyphur, Michael J and Sugihara, George and Laub, Patrick J},
  journal={The Stata Journal},
  volume={21},
  number={1},
  pages={220--258},
  year={2021},
}
```