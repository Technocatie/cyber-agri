# Resilient AI for UAV-Based Crop Disease Monitoring

This repository investigates the vulnerability of deep learning architectures to adversarial attacks in agricultural settings and proposes a "Mixed Adversarial Hardening" strategy to ensure the reliability of autonomous unmanned aerial vehicles (UAVs).

## Research Abstract
As autonomous unmanned aerial vehicles (UAVs) become integral to global food security through real-time crop disease monitoring, the vulnerability of their underlying deep learning architectures to adversarial manipulation poses a significant systemic risk. This study investigates the susceptibility of a ResNet-18 architecture trained on the PlantVillage dataset to digital sabotage via the Fast Gradient Sign Method (FGSM). 

While our baseline model achieved a state-of-the-art clean accuracy of **98.25%**, it demonstrated a catastrophic performance degradation to **30.47%** under adversarial perturbation. Our proposed hardening approach successfully achieved an adversarial robustness of **78.71%** while simultaneously improving clean accuracy to **99.80%**.

## Key Performance Metrics

| Model State | Clean Accuracy | Adversarial Robustness (FGSM) |
| :--- | :---: | :---: |
| **Baseline ResNet-18** | 98.25% | 30.47% |
| **With Median Filtering** | - | 39.58% |
| **Hardened ResNet-18 (Ours)** | **99.80%** | **78.71%** |

---

## Adversarial Attacks in Agriculture

Digital sabotage using the **Fast Gradient Sign Method (FGSM)** introduces subtle perturbations to leaf images. 

![Adversarial Perturbation Example](image1.png)
*Figure 1: Original healthy Blueberry leaf vs. Adversarial Noise vs. Attacked image.*

---

## Baseline Model Evaluation

The following confusion matrix illustrates the performance of the Baseline ResNet-18 model across the 38 distinct plant-leaf disease classes within the PlantVillage dataset.

![Confusion Matrix](image2.png)
*Figure 2: Confusion Matrix: Baseline ResNet18*

---

## Methodology
* **Vulnerability Assessment:** Evaluated ResNet-18 against FGSM attacks.
* **Defense Mechanisms:** Tested Median Filtering (passive) vs. Mixed Adversarial Hardening (intrinsic).
* **Dataset:** [PlantVillage Dataset (Kaggle)](https://www.kaggle.com/datasets/abdallahalidev/plantvillage-dataset)

---

## Citation (APA Format)
If you use this research or code in your work, please cite it as follows:

> **Mamgain, M., & Sinha, A. (2026).** *Resilient AI for UAV-Based Crop Disease Monitoring: Mixed Adversarial Hardening*. GitHub Repository. [Insert Your Repository Link Here]

## Contributors
* **Maitreyi Mamgain**
* **Anishka Sinha**
