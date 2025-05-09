---
layout: splash
title: ""  # prevents the default title from showing
permalink: /
header:
  overlay_image: /assets/images/banner.jpg
  overlay_position: center
  overlay_height: "auto"
  overlay_width: "100%"
  margin: "2rem auto"
  overlay_height: 400px
  overlay_filter: "0.0"
  actions:
    - label: "GitHub"
      url: "https://github.com/mammadmaheri7/TeleSparseRepo"
    - label: "Paper"
      url: "https://www.arxiv.org/abs/2504.19274"
    - label: "Dataset"
      url: "#"
  caption: "<br><br><br>"
---

{% include feature_row id="features" %}



A zero-knowledge-friendly sparsification technique for neural networks, designed to optimize SNARK proof generation without compromising accuracy.

{% include feature_row id="features" %}

### 🚀 TeleSparse: Practical Zero-Knowledge Proofs for Deep Neural Networks

Deep neural networks (DNNs) have transformed AI, powering breakthroughs in image recognition and language processing. But verifying these models without revealing sensitive details poses a significant privacy challenge. 🌐 TeleSparse makes zero-knowledge verification practical for today's powerful neural networks!

---

### 🕵️‍♂️ Threat Model: Ensuring Privacy and Security

TeleSparse assumes a malicious verifier and prover scenario, focusing on protecting sensitive model weights and inputs while verifying correctness. The threat model ensures that while parties follow the protocol, they may try to infer private information indirectly. TeleSparse provides robust guarantees against such privacy leakages.

<p align="center">
  <img src="assets/images/threat_model.png" alt="Threat Model" width="65%">
</p>

---

### ❓ Challenges Addressed by TeleSparse

1. **⚙️ High Computational Overhead:** Large models lead to extensive constraints, increasing computation and memory demands.
2. **📚 Extensive Lookup Tables:** Non-linear activations need massive lookup tables, further raising resource usage.

---

### 📊 System Overview

The figure below provides an overview of the TeleSparse system, showcasing its integration with the Halo2 proving system:

<p align="center">
  <img src="assets/images/overview.png" alt="System Overview" width="65%">
</p>

---

### 💡 Key Innovations of TeleSparse

#### 🌳 Sparse-aware ZK Proof Generation

TeleSparse employs sparse-aware pruning, reducing unnecessary constraints by strategically removing weights. This approach maintains high accuracy while drastically cutting prover memory use by 67% and proof generation time by 46%.

#### 🔄 Neural Network Teleportation – 📈 Activation Range Optimization

Neural network teleportation minimizes activation ranges, reducing lookup table sizes essential for zero-knowledge proofs. Teleportation optimizes activations, significantly streamlining the verification process. TeleSparse's teleportation adjusts activation ranges to be narrower, reducing the lookup tables needed. The distribution below illustrates this for ResNet20:

<p align="center">
  <img src="assets/images/teleportation.png" alt="Activation Range Distribution for ResNet20" width="55%">
</p>

---

### 🧪 Evaluation and Impressive Results

TeleSparse has been rigorously tested on popular architectures (Vision Transformers, ResNet, MobileNet) and datasets (CIFAR-10, CIFAR-100, ImageNet).

* **🚀 Faster Proof Generation:** Remarkable reductions in prover memory usage and computation time.
* **🎯 Accuracy Retention:** Only about a 1% accuracy drop—minimal compared to huge efficiency gains.

<p align="center">
  <img src="assets/images/evaluation.png" alt="Evaluation Framework" width="55%">
</p>

---

### 🛠 TeleSparse in Action

Using Halo2, known for efficient zero-knowledge proofs, TeleSparse leverages lightweight pruning and teleportation to deliver a scalable and efficient solution.

---

### 🌟 Why TeleSparse Matters

TeleSparse revolutionizes zero-knowledge proofs, enabling scalable, secure, and privacy-preserving AI. Dive deeper into TeleSparse on our [GitHub repository](https://github.com/mammadmaheri7/TeleSparseRepo) or explore our [arXiv paper](https://www.arxiv.org/abs/2504.19274)! 🌐
