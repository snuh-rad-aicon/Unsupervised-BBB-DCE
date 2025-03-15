# Unsupervised-BBB-DCE
The official repository for "Unsupervised Deep Learning for Model-Free Blood‒Brain Barrier Leakage Detection with Dynamic Contrast-Enhanced MRI in Diffuse Gliomas" published on _Radiology: Artificial Intelligence_.


## Introduction

This repository provides an unsupervised learning framework for detecting blood-brain barrier leakage without relying on pharmacokinetic models or arterial input function.

Key Points

•	An unsupervised autoencoder-based anomaly detection model was developed for blood-brain barrier leakage signal detection on dynamic contrast-enhanced MRI in patients with diffuse glioma; the model also enabled the distinction between tumor signals and vascular signals.

•	The leakage signal obtained from the proposed method (RLS) showed high correlation with the volume transfer constant (Ktrans) (r = 0.56, P < .001) and demonstrated more robust performance across different temporal resolutions (correlation with original values [r], 0.89 vs 0.72, P < .001; peak signal-to-noise ratio, 33.09 dB vs 28.94 dB, P < .001; structural similarity index measure, 0.92 vs 0.87, P < .001).

•	RLS outperformed Ktrans in predicting IDH mutation status in diffuse glioma (AUC = 0.87 [95% CI: 0.83–0.91] vs. 0.81 [95% CI: 0.76–0.85], P = .02).

![Fig1](Figure2.png)

## Files Description

dce.nii

## Requirements
```sh
pip install -r requirements.txt
```

## How to Run
Each Jupyter Notebook file runs sequentially to complete the full workflow.
