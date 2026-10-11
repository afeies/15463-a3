# 15-463 Assignment 3: Flash/No-Flash Photography

All code is in `assgn3.ipynb`, organized by problem:

1. **Bilateral filtering** (lamp images): basic and joint bilateral filtering, detail transfer, and shadow/specular masking.
2. **Gradient-domain processing** (museum images): re-integration with a conjugate gradient Poisson solver, then gradient-field fusion.
3. **Own flash/no-flash pairs**: Pair 1 (denoising) and Pair 2 (gradient-domain fusion).

## Requirements

Python 3 with `numpy`, `scipy`, `matplotlib`, `opencv-python`, and `Pillow`.

## Data layout

Run the notebook from `src/`. All paths are relative to it:

- `../data/lamp/`, `../data/museum/`: the course-provided images (not included in the submission; copy them here to re-run Problems 1 and 2).
- `../data/pair1/`, `../data/pair2/`: our own flash/no-flash JPEGs.
- `../data/results/`: the output images, and `../data/results/figures/` the figures used in the report.

## Running

Run the cells top to bottom. The slow steps (full-resolution filters, parameter sweeps, Poisson solves) are commented out and load their saved results from `../data/results/` instead. Uncomment them to recompute.
