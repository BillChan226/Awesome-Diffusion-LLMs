# Awesome Diffusion Large Language Models (DLMs) 🎈

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

> A curated list of research papers, code, models, datasets, and methods for **diffusion-based** large language models (2024 – now).

*Pull requests welcome – see [Contributing](#contributing).*

---

## Contents
- [Text-only Diffusion LLMs](#text-only-diffusion-llms)
- [Multimodal Diffusion LLMs](#multimodal-diffusion-llms)
- [Diffusion-LLM Training & Hybrid Methods](#diffusion-llm-training--hybrid-methods)
- [Safety of Diffusion LLMs](#safety-of-diffusion-llms)
- [Contributing](#contributing)
- [Citation](#citation)

---

## Text-only Diffusion LLMs

| Date | Project | Org | Intro | HF Model | HF Dataset | Takeaway Messages |
|------|---------|-----|-------|----------|------------|-------------------|
| 2025-02-14 | **LLaDA 8B** | Renmin U. & Ant | [Paper](https://arxiv.org/abs/2502.09992) | [Code](https://github.com/ML-GSAI/LLaDA) | [LLaDA-8B-Base](https://huggingface.co/GSAI-ML/LLaDA-8B-Base) | —— | <details><summary>Click</summary>First open-source 8 B diffusion LLM; rivals LLaMA-3 8B, fixes reversal-curse. :contentReference[oaicite:0]{index=0}</details> |
| 2025-04-30 | **Dream 7B** | HKU NLP & Huawei | [Blog](https://hkunlp.github.io/blog/2025/dream/) | [GitHub](https://github.com/HKUNLP/Dream) | [Dream-v0-Base-7B](https://huggingface.co/Dream-org/Dream-v0-Base-7B) | —— | <details><summary>Click</summary>Weight-reuse + context-adaptive noise yields 7 B model matching AR peers, strong planning. :contentReference[oaicite:1]{index=1}</details> |
| 2025-02-27 | **Mercury** | Inception Labs | [Site](https://www.inceptionlabs.ai/introducing-mercury) | —— | —— | <details><summary>Click</summary>Commercial dLLM family; >1 000 tok/s on H100 (≈10× AR speed) with GPT-4-mini-level quality. :contentReference[oaicite:2]{index=2}</details> |
| 2025-05-?? | **Gemini Diffusion** | Google DeepMind | [Overview](https://deepmind.com/research/highlighted-research) | —— | —— | <details><summary>Click</summary>Prototype text diffusion model shown to match Google’s fastest LLM quality while cutting latency. :contentReference[oaicite:3]{index=3}</details> |
| 2024-10-25 | **SEDD** | Stanford & CMU | [Paper](https://arxiv.org/abs/2310.16834) | [GitHub](https://github.com/louaaron/Score-Entropy-Discrete-Diffusion) | —— | <details><summary>Click</summary>Score-Entropy loss closes perplexity gap; SEDD beats GPT-2 on perplexity with 4×-32× fewer evals. :contentReference[oaicite:4]{index=4}</details> |
| 2023-10-31 | **SSD-LM** | CMU & UToronto | [Paper](https://arxiv.org/abs/2210.17432) | [GitHub](https://github.com/xhan77/ssd-lm) | —— | <details><summary>Click</summary>Semi-autoregressive blocks + simplex diffusion → GPT-2-level quality; modular controllable generation. :contentReference[oaicite:5]{index=5}</details> |
| 2023-05-16 | **AR-Diffusion** | Microsoft & THU | [Paper](https://arxiv.org/abs/2305.09515) | [Code](https://github.com/microsoft/ProphetNet/tree/master/AR-diffusion) | —— | <details><summary>Click</summary>Position-aware denoising mixes AR ordering with diffusion; up to 100–600× faster vs. GENIE at parity. :contentReference[oaicite:6]{index=6}</details> |

---

## Multimodal Diffusion LLMs

| Date | Project | Org | Intro | HF Model | HF Dataset | Takeaway Messages |
|------|---------|-----|-------|----------|------------|-------------------|
| 2025-05-21 | **MMaDA 8B** | THU & PKU | [Paper](https://arxiv.org/abs/2505.15809) | [GitHub](https://github.com/Gen-Verse/MMaDA) | —— | <details><summary>Click</summary>First unified multimodal diffusion LLM; UniGRPO RL boosts text + vision + T2I; beats SD-XL & LLaMA-3-7B. :contentReference[oaicite:7]{index=7}</details> |

*(add future multimodal entries here)*

---

## Diffusion-LLM Training & Hybrid Methods

| Date | Project | Org | Intro | HF Model | HF Dataset | Takeaway Messages |
|------|---------|-----|-------|----------|------------|-------------------|
| 2024-08-10 | **Diffusion-Guided LM** | Cornell | [Paper](https://arxiv.org/abs/2408.04220) | [Code](https://github.com/justinlovelace/Diffusion-Guided-LM) | —— | <details><summary>Click</summary>Uses diffusion to propose latent guidance that steers an AR LM; improves controllability (toxicity ↓) with minimal overhead. :contentReference[oaicite:8]{index=8}</details> |

---

## Safety of Diffusion LLMs

| Date | Project | Org | Intro | HF Model | HF Dataset | Takeaway Messages |
|------|---------|-----|-------|----------|------------|-------------------|
| 2025-01-05 | **DiffusionAttacker** | BUPT & Tsinghua | [Paper](https://arxiv.org/abs/2412.17522) | —— | —— | <details><summary>Click</summary>First jailbreak attack that *uses* a seq-to-seq diffusion model to rewrite prompts; ↑ ASR vs. AR baselines. :contentReference[oaicite:9]{index=9}</details> |
| 2025-01-18 | **DART** | ETH Zürich | [Paper](https://arxiv.org/abs/2501.08246) | —— | —— | <details><summary>Click</summary>*Text-Diffusion Red-Teaming*: diffusion perturbations with proximity constraints uncover harmful behaviours better than AR methods. :contentReference[oaicite:10]{index=10}</details> |

---

## Contributing

Please open an issue or PR to add new diffusion-LLM papers, codebases, models, benchmarks, or safety analyses.

---

## Citation

If you find this list useful, please cite it:

```bibtex
@misc{awesome2025diffusionllm,
  title  = {Awesome Diffusion Large Language Models},
  author = {Community},
  year   = {2025},
  url    = {https://github.com/BillChan226/Awesome-Diffusion-LLMs}
}
