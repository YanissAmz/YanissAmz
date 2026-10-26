# Yaniss Amazouz

**AI Engineer // LLM Inference & AI in Production** — Télécom SudParis (IP Paris) · [yamzlabs.com](https://yamzlabs.com)

I make open AI models run fast on your own hardware, then put them to work.

| ★ 210 | ~1,000 | 85,000+ | ~2× |
|:---:|:---:|:---:|:---:|
| GitHub stars for Kyojin in 3 weeks | developers installed Kyojin in 2 weeks | downloads of my models on Hugging Face | faster than llama.cpp |

## Kyojin — founder, Yamz Labs

**[Kyojin](https://github.com/Yamz-Labs/kyojin)** runs the largest open models (DeepSeek, GLM, Qwen) on one mini PC or a single graphics card, **about 2× faster than llama.cpp**, up to 3× on some models ([benchmarks](https://github.com/Yamz-Labs/kyojin/blob/main/doc/benchmarks.md)).
- 210 stars in 3 weeks, ~1,000 developers installed it in 2 weeks, 8 outside contributors.
- 20+ releases in the first month, each gated by public benchmarks and a regression check.
- Custom GPU kernels for AMD (ROCm) and NVIDIA (CUDA), built on ExLlamaV3. Our compressed models are on [hf.co/yamz-labs](https://huggingface.co/yamz-labs), quality measured against the official weights.

## In production — GETA Solutions

**[getasolutions.fr](https://getasolutions.fr)**: e-commerce platform for truck tyres, parts and services, designed, built and run alone. **Nearly €40k revenue in 3 months.**
- ~100,000 lines of code, 3,200+ automated tests, 640+ pull requests checked by CI.
- An AI agent that sells: it finds the right product, fills the cart and books a callback. Try it live with the “Besoin d'aide ?” button.
- 28 tasks fully automated: invoices, payment reminders, bank reconciliation, competitor pricing, Google Ads.
- Architecture overview: [getasolutions-portfolio](https://github.com/YanissAmz/getasolutions-portfolio).

## Upstream work

- **[llama.cpp](https://github.com/ggml-org/llama.cpp)**: NVIDIA Nemotron-3 support **merged** ([PR #25444](https://github.com/ggml-org/llama.cpp/pull/25444), reviewed by two maintainers), plus a follow-up fix ([PR #28779](https://github.com/ggml-org/llama.cpp/pull/28779)).
- **[Hugging Face](https://huggingface.co/YanissAmz)**: **85,000+ downloads** across my models. My [Tencent Hy3 GGUF](https://huggingface.co/YanissAmz/Hy3-295B-A21B-GGUF) builds became the reference local setup on [r/LocalLLaMA](https://www.reddit.com/r/LocalLLaMA/comments/1usy9ie/tencenthy3_is_the_real_deal_on_128gb/); also [Nemotron-3](https://huggingface.co/YanissAmz/Nemotron-3-Puzzle-75B-A9B-GGUF) and a [DeepSeek-V4-Flash draft model](https://huggingface.co/YanissAmz/DeepSeek-V4-Flash-DSpark-draft-GGUF).

## Home inference lab

| Repo | What |
|---|---|
| [strix-halo-llm-serving](https://github.com/YanissAmz/strix-halo-llm-serving) | Speculative decoding + kernel work on AMD Strix Halo: DeepSeek-V4-Flash, GLM-5.3-Flash, Qwen3.8 — paired duels, both legs reported |
| [escha-port](https://github.com/YanissAmz/escha-port) | Porting the ESCHAM 2-bit format (QTIP trellis) into llama.cpp — CUDA/HIP kernels, ×33 prefill, honest head-to-head vs Q4_K_XL |
| [qwdense-turbo](https://github.com/YanissAmz/qwdense-turbo) | 2.28× faster Claude Code on a local Qwen3.6-27B int4 — MTP speculative decoding, tool calling, corruption guards |
| [qwdense-llamacpp](https://github.com/YanissAmz/qwdense-llamacpp) | llama.cpp native Qwen3.6 MTP lab for long-context agentic coding |

## Most loved

- **[hyte-y70-touch-dashboard](https://github.com/YanissAmz/hyte-y70-touch-dashboard)** ⭐ most-starred — the only Linux dashboard for the HYTE Y70 Touch touchscreen: 10 swipe pages, reverse-engineered LED control.
- **[federated-learning-privacy](https://github.com/YanissAmz/federated-learning-privacy)** — FedAvg + gradient-inversion attacks + DP defenses, with the honest finding that naive Central DP collapses utility on small federations.
- **[efficient-llm-pipeline](https://github.com/YanissAmz/efficient-llm-pipeline)** — TurboQuant KV-cache compression + LoRA on Phi-4-mini, documenting three architecture-dependent findings the original paper doesn't mention.

## Stack

**Inference** — C++, llama.cpp, GGUF, quantization, speculative decoding, vLLM, SGLang, CUDA, ROCm, Vulkan · **ML** — Python, PyTorch, RAG, Hugging Face · **Software** — Django, FastAPI, PostgreSQL, Docker, GitHub Actions, Azure · **Infra** — Linux, systemd, a four-machine fleet (AMD, NVIDIA, Apple Silicon, cloud) serving models 24/7

---

[yamzlabs.com](https://yamzlabs.com) · [LinkedIn](https://www.linkedin.com/in/yaniss-amazouz) · [Hugging Face](https://huggingface.co/YanissAmz) · [getasolutions.fr](https://getasolutions.fr)
