## Azaz Mir

**MS Computer Science (AI) — University of Texas at Arlington.** I work on making vision-language models actually run on edge hardware, and on finding out where they break.

🌐 [azazmir1.github.io](https://azazmir1.github.io) · 💼 [LinkedIn](https://linkedin.com/in/azazmir) · ✉️ axm6255@mavs.uta.edu

---

### Research

**Characterizing Multi-Turn Vision-Language Model Inference on Resource-Constrained Edge Hardware**
*Under review — ACM SIGMETRICS '27*

A systematic profiling study of five compact VLMs across four platforms (RTX A6000, Jetson AGX Orin, Jetson Orin Nano, Raspberry Pi 5) under multi-turn, multi-image workloads. Key findings:

- Per-turn inference cost is governed by **cumulative context length**, not turn count
- **Parameter count does not predict latency** — LFM2-VL-450M runs 1.8–2.4× faster than the smaller SmolVLM-256M
- Latency rises 4.3–4.7× from A6000 to Orin Nano, and up to **56× on CPU-only Raspberry Pi 5**
- An empirical memory model predicts OOM boundaries at **0.8% MAPE in-device**, 2.2–7.3% cross-device

**Multi-Stage Static Analysis of Software Supply Chain Attacks**
Graph-contextual anomaly ranking plus a GNN API-call sequence matcher for detecting zero-day malicious PyPI packages — where signature-based scanners have zero recall. **99.96% precision, 94.4% recall, 0.99998 AUROC** at a 0.023% false-positive rate.

---

### What I build

| | |
|---|---|
| **Edge AI** | Jetson AGX Orin / Orin Nano, Raspberry Pi 5, TensorRT, ONNX, INT4/AWQ quantization |
| **Multimodal** | SmolVLM, FastVLM, InternVL, LLaVA-OV, LFM2-VL, Florence-2, ViT encoders |
| **ML / GenAI** | PyTorch, TensorFlow, Hugging Face, RAG, FAISS, LangChain, Llama-2/3 |
| **Graph ML & Security** | PyTorch Geometric, igraph, Leiden/Louvain, Isolation Forest, AST analysis |
| **Agentic AI** | CrewAI, AutoGen, multi-agent orchestration, tool use |
| **Data & Cloud** | Spark, Databricks, Delta Lake, Azure (Data Factory, ADLS, Synapse), AWS |

---

### Selected repositories

- **[new_vlm_profiling](https://github.com/azazmir1/new_vlm_profiling)** — multi-turn VLM inference profiling across Jetson and Raspberry Pi 5 (SIGMETRICS '27 submission)
- **[vlm-jetson-benchmark](https://github.com/azazmir1/vlm-jetson-benchmark)** — 16 compression methods × 19 models on an 8GB Jetson Orin Nano
- **[vlm-edge-profiling-results](https://github.com/azazmir1/vlm-edge-profiling-results)** — FP16/FP32 profiling results with per-component timing breakdowns
- **[florence_vlm](https://github.com/azazmir1/florence_vlm)** — component-level latency and memory profiler for Florence-2
- **[LawChatbot_llama3](https://github.com/azazmir1/LawChatbot_llama3)** — legal information retrieval with Llama-3 and RAG

---

<sub>Previously: Data Scientist at Royal Cyber Inc. (2023–2025), building production LLM and RAG systems for enterprise clients.</sub>
