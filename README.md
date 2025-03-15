# Unsupervised-BBB-DCE
The official repository for "Unsupervised Deep Learning for Model-Free Blood‒Brain Barrier Leakage Detection with Dynamic Contrast-Enhanced MRI in Diffuse Gliomas" published on _Radiology: Artificial Intelligence_.


## Introduction

This repository provides an unsupervised learning framework for detecting blood-brain barrier leakage without relying on pharmacokinetic models or arterial input function.

**Key Points**

•	An unsupervised autoencoder-based anomaly detection model was developed for blood-brain barrier leakage signal detection on dynamic contrast-enhanced MRI in patients with diffuse glioma; the model also enabled the distinction between tumor signals and vascular signals.

•	The leakage signal obtained from the proposed method (RLS) showed high correlation with the volume transfer constant (Ktrans) (r = 0.56, P < .001) and demonstrated more robust performance across different temporal resolutions (correlation with original values [r], 0.89 vs 0.72, P < .001; peak signal-to-noise ratio, 33.09 dB vs 28.94 dB, P < .001; structural similarity index measure, 0.92 vs 0.87, P < .001).

•	RLS outperformed Ktrans in predicting IDH mutation status in diffuse glioma (AUC = 0.87 [95% CI: 0.83–0.91] vs. 0.81 [95% CI: 0.76–0.85], P = .02).

![Fig1](Figure2.png)

![Fig2](Figure4.png)

**Table: Comparison of the robustness of RLS and *_Ktrans_* to subsampling**

|            | r² (RLS) | r² (*Ktrans*) | *P value* | PSNR (mean ± SD dB, RLS) | PSNR (mean ± SD dB, *Ktrans*) | *P value* | SSIM (mean ± SD, RLS) | SSIM (mean ± SD, *Ktrans*) | *P value* |
|------------|---------|-------------|----------|----------------------|----------------------|----------|------------------|------------------|----------|
| **D_under**  | 0.90    | 0.90        | .89      | 36.19 ± 1.79         | 32.69 ± 2.96         | < .001   | 0.93 ± 0.02      | 0.92 ± 0.03      | .01      |
| **D_trunc**  | 0.89    | 0.72        | < .001   | 33.09 ± 1.91         | 28.94 ± 4.16         | < .001   | 0.92 ± 0.02      | 0.87 ± 0.05      | < .001   |
| **D_hybrid** | 0.92    | 0.91        | .45      | 37.25 ± 2.03         | 32.16 ± 3.90         | < .001   | 0.96 ± 0.02      | 0.93 ± 0.04      | < .001   |

Note:
- **SD** = standard deviation, **PSNR** = peak signal-to-noise ratio, **SSIM** = structural similarity.
- **RLS** = residual leakage signal.

## Files Description

dce.nii

## Requirements
```sh
pip install -r requirements.txt
```

## How to Run
Each Jupyter Notebook file runs sequentially to complete the full workflow.
