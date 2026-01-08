# Dual-RMV
Federated Ranking Learning (FRL) is a state-of-the-art FL framework that stands out for its communication efficiency and robustness to poisoning attacks. Unlike traditional FL paradigm, FRL evaluates the discrete rankings rather than gradient updates, significantly reducing the communication overhead and bounding the space of malicious manipulation. Additionally, it alters the parameter aggregation to the majority voting, ensuring the fairness since that each client contributes a single vote. However, recent findings indicate that the robustness of FRL can be substantially undermined due to inherent structural vulnerabilities. Consequently, we first examine the fundamental causes behind the effectiveness of such attacks and verify that public knowledge of the majority-voting mechanism enables adversaries to accurately infer benign privacy. Based on this observation, our main idea consists of two parts: 1) On the client side, to mislead adversaries into identify benign updates with bias, we propose an adaptive RDP-Calibrated perturbation that reducing the effectiveness of attacks while accentuating the characteristics of malicious updates, and 2) on the server side, we propose a robust-improved majority voting that using spectral analysis to filter out malicious votes and thus maximize the robustness of majority voting. Through extensive experiments on benchmark datasets, we demonstrate that our approach achieves an overall 3.58% attack impact and is ∽16× more robust than existing AGRs.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)

## Installation

```bash
# Clone the repository
git clone [https://github.com/alanyw/Dual-RMV.git]
```
```bash
# Change the directory into the project
cd Dual-RMV
```
```bash
# Install dependencies
pip install -r requirements.txt
```
## Usage

To use this project, follow these steps:

### For MNIST dataset

```bash
cd testing/sh
```
```bash
sh mnist.sh
```
### For CIFAR10 dataset

```bash
cd sh
```
```bash
sh cifar10.sh
```



