# When Do Diffusion Transformers Outperform U-Nets?

**Arshvir Sandhu, Gunbir Baveja, Parvin Aliyeva** - UBC CPSC 440/550, April 2026

## Overview
A controlled comparison of a convolutional U-Net and a patch-based Diffusion Transformer
(DiT) as denoisers in a DDPM-style diffusion model trained on CIFAR-10. We evaluate both
architectures under standard denoising and structured corruptions designed to probe
long-range spatial reasoning.

## Repository Structure
- `notebook/` — Colab training notebook
- `report/`   — LaTeX and PDF source for the paper
- `figs/`     — figures and sample images

## Results Summary
| Model | FID ↓ | Masked MSE ↓ |
|-------|-------|--------------|
| U-Net | 247.45 | 0.754 |
| DiT   | 340.18 | 1.462 |

## How to Run
1. Open `notebook/diffusion_comparison.ipynb` in Google Colab
2. Set runtime to T4 GPU
3. Run all cells top to bottom

## Requirements
See the first notebook cell - all dependencies are installed via `pip` inside the notebook.