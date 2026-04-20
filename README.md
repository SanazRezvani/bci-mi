# 🧠 EEG Motor Imagery Classification using CSP (MATLAB)

A complete MATLAB pipeline for **EEG-based motor imagery classification** using signal processing, Common Spatial Patterns (CSP), and machine learning.

This work is based on **BCI Competition III – Dataset IVa**.

---

## 📌 Project Overview

This project implements a full Brain-Computer Interface (BCI) pipeline to classify **motor imagery EEG signals** (Right Hand vs Foot).

The objective is to transform raw EEG signals into discriminative features and evaluate multiple classifiers.

---

## ⚙️ Pipeline Overview

```text
Raw EEG
   ↓
Band-pass Filtering (μ / β bands)
   ↓
Spatial Filtering (CAR / Laplacian)
   ↓
Trial Extraction
   ↓
CSP Feature Extraction
   ↓
Feature Vector (Variance)
   ↓
Classification (SVM / KNN / LDA)


## 🧩 Key Components

### 1. Frequency Filtering

Band-pass filtering isolates motor-related rhythms:

μ band: 8–13 Hz
β band: 13–30 Hz
γ band: 13–49.9 Hz

![Frequency Spectrum](results/frequency_spectrum.png)
