# PCA from Scratch

Starter repository for the **Linear Algebra for ML** capstone on [DutchEngineer](https://dutchengineer.org).

## What you will build

A PCA implementation built from the linear algebra primitives you studied in this module — no dimensionality reduction libraries. A CLI that takes a dataset and a number of components, reports explained variance, and validates that reconstruction error behaves correctly.

## Requirements

1. **Centering** — the data must be centered before any decomposition, so the analysis captures variance rather than offset from the origin.
2. **Decomposition** — find the principal directions of the data using only NumPy operations on the data matrix or its covariances. The choice of method is yours.
3. **Projection** — transform data into the reduced-dimension space and back. Full-rank reconstruction must recover the original data within numerical precision.
4. **Explained variance** — report how much of the total variance each component captures. The ratios must sum to 1.
5. **Monotonicity check** — reconstruction error must decrease as the number of components increases. The CLI validates this automatically.

## Getting started

1. **Fork this repository** — click **Fork** at the top of [this page](https://github.com/dutchengineer-org/pca-from-scratch-starter) to create your own copy.
2. Clone your fork:
   ```
   git clone https://github.com/<your-username>/pca-from-scratch-starter
   cd pca-from-scratch-starter
   ```
3. Install dependencies: `uv sync`
4. Build and run: `uv run python pca.py data.csv --n-components 3`

## Submitting

When your work is ready, paste your repository URL into the submission form on your [capstone page](https://dutchengineer.org/foundations/linear-algebra-for-ml/capstone-pca-from-scratch/).
