# Thesis Project

This repository contains code and experiments for my thesis on **Adversarial Attacks and Defense in Image Classification model**.

## Contents
- FGSM implementation
- Adversarial training
- Defense layers
- Noise-based defense
- Epsilon training

## Details
This thesis proposes a systematic study of FGSM adversarial attacks and multiple
corresponding defense mechanisms to enhance model robustness. Specifically, it focuses on evaluating how different deep learning models both complex and lightweight
respond to adversarial attacks and what strategies can be implemented to mitigate
these effects.
The problem addressed is two fold:
1. Evaluating Vulnerability: Understanding the impact of FGSM on CNNs,
including high-capacity pretrained models like ResNet-34 and manually con-
1.4. CONTRIBUTIONS 4
structed models like myCNN, when applied to datasets such as Kaggle’s image
classification dataset and MNIST.
2. Implimenting and Testing Defenses: Implementing and analyzing various
defense techniques, including:
** Adversarial Training: ** Retraining the model using a mix of clean and
FGSM-perturbed images to build resilience.
** Defense Layer (DefendedModel): ** Introducing preprocessing steps like
Gaussian blur, JPEG compression, and median denoising to clean adversarial inputs before classification.
** Noise Injection Techniques: ** Training models on augmented data with
injected noise patterns such as Random Gaussian Noise (RGN), Stochastic Motion Blur (SMB), Stochastic Glass Blur (SGB), and Random Sized
Coarse Dropout (RSCD) to promote robustness.
** Multiple Epsilons Training: ** This involves generating adversarial examples from the training dataset and including them in the training process.
This helps the model learn more resilient decision boundaries rather than
using a single, fixed perturbation strength ϵ, adversarial samples were generated using multiple epsilon values:ϵ ∈ {0.01, 0.05, 0.1, 0.2, 0.3}.
By comparing these approaches under different epsilon levels (perturbation strengths),
the thesis aims to identify which techniques or combinations provide the most reliable
defense against FGSM, without severely compromising accuracy on clean data. The
main goal targets the development of deep learning systems which maintain security
and resilience for trusted deployment in real-world operations.

## Author  
Umesh Kumar  
IIT (ISM) DHANBAD
