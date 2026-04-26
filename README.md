# Yaniss Amazouz

**AI Engineer** — Telecom SudParis (Institut Polytechnique de Paris)

Building applied AI and the systems around them: LLM optimization, federated
learning, computer vision, home automation, and the boring infrastructure
that keeps it all running on a single RTX 3090.

---

### LLM serving and privacy

| Project | What | Stack |
|---|---|---|
| [**qwdense-turbo**](https://github.com/YanissAmz/qwdense-turbo) | 2.28× faster Claude Code on a local Qwen3.6-27B int4 (RTX 3090) — single installer, MTP speculative decoding, tool calling, corruption guards | vLLM, AutoRound, Anthropic protocol proxy |
| [**federated-learning-privacy**](https://github.com/YanissAmz/federated-learning-privacy) | FedAvg + iDLG gradient inversion + Central DP + Byzantine attacks + robust aggregation. Two threat models, five attacks, four aggregators, regression-tested. | PyTorch, Gradio, zCDP composition |
| [**efficient-llm-pipeline**](https://github.com/YanissAmz/efficient-llm-pipeline) | TurboQuant KV cache compression + LoRA fine-tuning on Phi-4-mini, with reproducible benchmarks and FastAPI serving | PyTorch, Transformers, PEFT |

### Computer vision

| Project | What | Stack |
|---|---|---|
| [**anomaly-detection-api**](https://github.com/YanissAmz/anomaly-detection-api) | PatchCore visual anomaly detection on MVTec AD — FastAPI service with heatmap overlay and Streamlit demo | PyTorch, WideResNet50, FastAPI, Streamlit |

### Home & desk

| Project | What | Stack |
|---|---|---|
| [**infra-home**](https://github.com/YanissAmz/infra-home) | Bring back Ambilight+Hue (TP Vision removed it in 2023), sync TV colours to PC RGB, debloat Fire TV, block ads network-wide — all from one Home Assistant dashboard | Home Assistant, JointSPACE API, OpenRGB, Pi-hole |
| [**hyte-y70-touch-dashboard**](https://github.com/YanissAmz/hyte-y70-touch-dashboard) | The only Linux dashboard for the HYTE Y70 Touch case touchscreen — 10 swipe pages, reverse-engineered LED control, dedicated Xorg :1 setup | SolidJS, FastAPI, GTK3 + WebKit2 |

### Web

| Project | What | Stack |
|---|---|---|
| [**GETA Solutions**](https://github.com/YanissAmz/getasolutions-portfolio) | E-commerce platform B2C/B2B for truck tires + parts + transport — live at [getasolutions.fr](https://getasolutions.fr) | Django 5.2, Stripe, PostgreSQL, TecDoc |

---

### Tech

**ML/AI** — PyTorch, Transformers, PEFT, bitsandbytes, vLLM, scikit-learn, OpenCV

**Backend** — Python, Django, FastAPI, PostgreSQL, Docker, Redis

**Frontend** — TypeScript, SolidJS, Vite, TailwindCSS, Gradio, Streamlit

**Systems** — Linux, CUDA, systemd, Xorg, OpenRGB, Home Assistant

---

[LinkedIn](https://www.linkedin.com/in/yaniss-amazouz-b7a461204/) · [getasolutions.fr](https://getasolutions.fr)
