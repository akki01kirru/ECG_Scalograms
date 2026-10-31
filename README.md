# ECG Scalogram Dataset for Multiclass Cardiac Classification

## 1. Overview

This repository contains an ECG scalogram image dataset developed for multiclass cardiac condition classification using Deep Learning and Hybrid Quantum Machine Learning techniques.

The dataset consists of Continuous Wavelet Transform (CWT) scalogram images derived from electrocardiogram (ECG) signals obtained from PhysioNet.

Four cardiac classes are considered:

- **CHF** – Congestive Heart Failure
- **NSR** – Normal Sinus Rhythm
- **AF** – Atrial Fibrillation
- **ARR** – Arrhythmia

The dataset is intended for research and experimentation involving ECG image classification, time-frequency analysis, deep neural networks, and quantum machine learning.

## 2. Dataset Description

| Parameter | Description |
|---|---|
| Data source | PhysioNet |
| Signal type | ECG |
| Number of classes | 4 |
| Original recordings | 30 per class |
| Sampling frequency | 128 Hz |
| Samples per recording | 65,536 |
| Total original recordings | 120 |
| Scalogram generation | Continuous Wavelet Transform (CWT) |
| Image representation | Time-frequency scalograms |
| Images per class | 300 |
| Total images | 1,200 |

## 3. Class Distribution

| Class | Description | Number of Images |
|---|---|---:|
| CHF | Congestive Heart Failure | 300 |
| NSR | Normal Sinus Rhythm | 300 |
| AF | Atrial Fibrillation | 300 |
| ARR | Arrhythmia | 300 |
| **Total** | | **1,200** |

## 4. Signal Preprocessing

The original ECG signals were obtained from PhysioNet and processed before scalogram generation.

The preprocessing operations include:

1. ECG signal extraction from the original database.
2. Sampling frequency adjustment according to the dataset specifications.
3. Resampling to 128 Hz.
4. Truncation of signals to 65,536 samples.
5. Gain normalization.
6. Continuous Wavelet Transform for time-frequency representation.
7. Generation and storage of scalogram images.

The resulting scalograms represent the time-frequency characteristics of ECG signals and are used as image inputs for classification models.

## 5. Dataset Organization

The dataset is organized into four class-specific folders.

```text
ECG-Scalogram-Dataset/
│
├── CHF/
│   ├── CHF_001.png
│   ├── CHF_002.png
│   └── ...
│
├── NSR/
│   ├── NSR_001.png
│   ├── NSR_002.png
│   └── ...
│
├── AF/
│   ├── AF_001.png
│   ├── AF_002.png
│   └── ...
│
├── ARR/
│   ├── ARR_001.png
│   ├── ARR_002.png
│   └── ...
│
└── README.md
```

Each folder contains 300 scalogram images belonging to the corresponding cardiac class.

## 6. Methodology

The proposed research workflow is:

```text
PhysioNet ECG Database
         |
         v
ECG Signal Acquisition
         |
         v
Signal Preprocessing
         |
         v
Resampling to 128 Hz
         |
         v
Signal Truncation and Normalization
         |
         v
Continuous Wavelet Transform
         |
         v
ECG Scalogram Generation
         |
         v
Four-Class Image Dataset
         |
         v
Deep Learning and
Hybrid Quantum Classification
         |
         v
Performance Evaluation
```

## 7. Intended Applications

This dataset can be used for the following research applications:

- ECG-based cardiac condition classification.
- Time-frequency analysis of biomedical signals.
- AlexNet-based ECG image classification.
- Convolutional Neural Network (CNN) architectures.
- Hybrid Quantum-Classical Machine Learning.
- Variational Quantum Circuit (VQC)-based classification.
- Comparative evaluation of classical and quantum machine learning algorithms.

## 8. Proposed Classification Models

The dataset is intended for comparative experimentation using:

**Classical Deep Learning**
- AlexNet
- Convolutional Neural Networks (CNN)

**Hybrid Quantum Machine Learning**
- AlexNet with Variational Quantum Circuits (AlexNet–VQC)
- Quantum-enhanced ECG image classification.

The performance of these approaches can be evaluated using accuracy, precision, recall, F1-score, ROC-AUC and confusion matrices.

## 9. Reproducibility and Evaluation

For reliable experimental evaluation:

- Maintain consistent class labels across experiments.
- Use training, validation and independent testing datasets.
- Avoid data leakage by keeping images derived from the same original ECG recording within the same data partition.
- Apply identical evaluation conditions when comparing classical and hybrid quantum models.
- Report all preprocessing and model configuration parameters.

## 10. Data Source and Acknowledgement

The original ECG recordings were obtained from PhysioNet.

**PhysioNet:** https://physionet.org/

Users of this derived dataset should consult the original PhysioNet database documentation, associated publications and applicable data-use licenses.

Please acknowledge the original database contributors and cite the relevant PhysioNet database publications when using this dataset.

## 11. Disclaimer

This dataset is intended exclusively for academic research, educational purposes and algorithm development.

The generated scalogram images and classification models are not intended to replace professional medical diagnosis or clinical decision-making.

## 12. Keywords

ECG, PhysioNet, CWT, Scalogram, Congestive Heart Failure, Normal Sinus Rhythm, Atrial Fibrillation, Arrhythmia, AlexNet, Deep Learning, Quantum Machine Learning, Variational Quantum Circuit, Biomedical Signal Processing.

---

**Repository:** ECG Scalogram Dataset for Classical and Hybrid Quantum Machine Learning Research.
