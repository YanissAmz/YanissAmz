# Yaniss Amazouz

**AI Engineer // LLM Inference & Systems** — Télécom SudParis (IP Paris)

I bring big models to small machines: 320B-parameter models on a 128 GB mini PC, where it usually takes a GPU server worth over €100k.

## Kyojin — founder, Yamz Labs

**[Kyojin](https://github.com/Yamz-Labs/kyojin)** is an open-source inference engine (built on ExLlamaV3) that runs GLM-5.3-Flash (320B), Qwen3.8-Flash-Next and MiMo-V2.6-Flash on one AMD Ryzen AI Max+ 395 with 128 GB, up to 500K tokens of context.
- Faster than competing engines on the same machine, up to 3× llama.cpp ([benchmarks](https://github.com/Yamz-Labs/kyojin/blob/main/doc/benchmarks.md)).
- Quality measured against the official FP8 weights (KL, top-1); models on [hf.co/yamz-labs](https://huggingface.co/yamz-labs).
- 170+ stars in two weeks, 5 outside contributors.

## Upstream work

- **[llama.cpp](https://github.com/ggml-org/llama.cpp)** — brought up **NVIDIA Nemotron-3-Puzzle-75B-A9B** (per-layer MoE): C++ graph builder, per-layer hparams, HF→GGUF converter. **Merged** — [PR #25444](https://github.com/ggml-org/llama.cpp/pull/25444) (56 files, two maintainer reviews). Follow-up robustness fix — [PR #28779](https://github.com/ggml-org/llama.cpp/pull/28779).
- **[Hugging Face](https://huggingface.co/YanissAmz)** — the reference GGUF builds, **70k+ all-time downloads**: [Hy3-295B-A21B-GGUF](https://huggingface.co/YanissAmz/Hy3-295B-A21B-GGUF) (51k), [Nemotron-3-Puzzle-75B-A9B-GGUF](https://huggingface.co/YanissAmz/Nemotron-3-Puzzle-75B-A9B-GGUF), [DeepSeek-V4-Flash-DSpark-draft-GGUF](https://huggingface.co/YanissAmz/DeepSeek-V4-Flash-DSpark-draft-GGUF). Picked as the reference local setup on [r/LocalLLaMA](https://www.reddit.com/r/LocalLLaMA/comments/1usy9ie/tencenthy3_is_the_real_deal_on_128gb/) for publishing perplexity numbers.

## Home inference lab

| Repo | What |
|---|---|
| [strix-halo-llm-serving](https://github.com/YanissAmz/strix-halo-llm-serving) | Speculative decoding + kernel work on AMD Strix Halo: DeepSeek-V4-Flash, GLM-5.3-Flash, Qwen3.8 — paired duels, both legs reported |
| [escha-port](https://github.com/YanissAmz/escha-port) | Porting the ESCHAM 2-bit format (QTIP trellis) into llama.cpp — CUDA/HIP kernels, ×33 prefill, honest head-to-head vs Q4_K_XL |
| [qwdense-turbo](https://github.com/YanissAmz/qwdense-turbo) | 2.28× faster Claude Code on a local Qwen3.6-27B int4 — MTP speculative decoding, tool calling, corruption guards |
| [qwdense-llamacpp](https://github.com/YanissAmz/qwdense-llamacpp) | llama.cpp native Qwen3.6 MTP lab for long-context agentic coding |

## Production

- **[GETA Solutions](https://github.com/YanissAmz/getasolutions-portfolio)** — B2C/B2B e-commerce platform (truck tires, parts, transport), designed, built and operated solo: Django 5.2, Stripe (cards, SEPA, Alma), PostgreSQL, TecDoc — live at [getasolutions.fr](https://getasolutions.fr), €18k revenue in August 2026.

## Most loved

- **[hyte-y70-touch-dashboard](https://github.com/YanissAmz/hyte-y70-touch-dashboard)** ⭐ most-starred — the only Linux dashboard for the HYTE Y70 Touch touchscreen: 10 swipe pages, reverse-engineered LED control.
- **[federated-learning-privacy](https://github.com/YanissAmz/federated-learning-privacy)** — FedAvg + gradient-inversion attacks + DP defenses, with the honest finding that naive Central DP collapses utility on small federations.
- **[efficient-llm-pipeline](https://github.com/YanissAmz/efficient-llm-pipeline)** — TurboQuant KV-cache compression + LoRA on Phi-4-mini, documenting three architecture-dependent findings the original paper doesn't mention.

## Stack

**Inference** — C++, llama.cpp, GGUF, quantization, speculative decoding, vLLM, SGLang, CUDA, ROCm, Vulkan · **ML** — Python, PyTorch, RAG, Hugging Face · **Software** — Django, FastAPI, PostgreSQL, Docker, GitHub Actions, Azure · **Infra** — Linux, systemd, a four-machine fleet (AMD, NVIDIA, Apple Silicon, cloud) serving models 24/7

---

[LinkedIn](https://www.linkedin.com/in/yaniss-amazouz) · [Hugging Face](https://huggingface.co/YanissAmz) · [getasolutions.fr](https://getasolutions.fr)
