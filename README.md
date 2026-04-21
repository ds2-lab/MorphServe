# MorphServe

**MorphServe** is a dynamic, workload-aware serving framework for Large Language Models (LLMs). It enables **elastic adaptation of both transformer layer weight precision and KV cache capacity at runtime**, allowing systems to maintain high throughput and stable latency under varying workloads.

---

## 🚧 Code Release Status

We are currently preparing the codebase for public release. The repository is being cleaned, documented, and organized for reproducibility, with additional examples and usage guidelines under preparation.

👉 **The full code will be released soon. Stay tuned!**

---

## 🔍 Overview

Modern LLM serving systems face significant challenges under dynamic and bursty workloads, where fixed resource allocation strategies often lead to suboptimal performance or degraded quality.

MorphServe addresses this by introducing a **joint adaptation mechanism** that coordinates:

- **Layer Weight Precision** (via selective quantization)
- **KV Cache Capacity** (via dynamic memory management)

This allows the system to respond effectively to runtime resource pressure without requiring model retraining or offline reconfiguration.

---

## ✨ Features

- Dynamic adaptation to workload fluctuations
- No retraining required
- Compatible with existing LLM serving optimizations (e.g., FlashAttention, PagedAttention, dynamic batching)
- Designed for real-world deployment scenarios

---

## 📄 Paper

More details can be found in our paper:

> *MorphServe: Efficient and Workload-Aware LLM Serving via Runtime Quantized Layer Swapping and KV Cache Resizing*

📌 https://mlsys.org/virtual/2026/oral/3816

---

## 📌 Citation

If you find our work useful, please consider citing:

```bibtex
@article{su2025morphserve,
  title={MorphServe: Efficient and Workload-Aware LLM Serving via Runtime Quantized Layer Swapping and KV Cache Resizing},
  author={Su, Zhaoyuan and Zhang, Zeyu and Lan, Tingfeng and Wang, Zirui and Shen, Haiying and Yang, Juncheng and Cheng, Yue},
  journal={arXiv preprint arXiv:2506.02006},
  year={2025}
}
