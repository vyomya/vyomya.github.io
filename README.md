<h1 align="center">Hi, I am Vyom Agarwal 👋</h1>
<h3 align="center">AI / ML Engineer • LLM Agents • Multimodal and Generative AI • Efficient Deep Learning</h3>

<p align="center">
  <a href="https://www.linkedin.com/in/vyom-agarwal1/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white" /></a>
  <a href="https://github.com/vyomya"><img src="https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white" /></a>
  <a href="https://scholar.google.com/citations?user=mJttqWsAAAAJ"><img src="https://img.shields.io/badge/Google%20Scholar-4285F4?style=flat&logo=googlescholar&logoColor=white" /></a>
  <a href="https://arxiv.org/abs/2606.22790"><img src="https://img.shields.io/badge/arXiv-2606.22790-B31B1B?style=flat&logo=arxiv&logoColor=white" /></a>
  <a href="https://paai-six.vercel.app/"><img src="https://img.shields.io/badge/PAAI-Live%20Demo-000000?style=flat&logo=vercel&logoColor=white" /></a>
  <a href="mailto:vyom.wal@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white" /></a>
</p>

---

### 🎓 About Me

I am a Master's student in **Applied Machine Learning at the University of Maryland, College Park** (GPA 3.83/4.0, graduating May 2027). Before this, I spent two and a half years as a **Research AI Engineer at Robert Bosch**, building a foundation model platform used across research teams, multi-agent developer tooling, and edge perception models for autonomous driving.

My research sits where efficient deep learning meets multimodal systems: compressing speech models, repairing diffusion model outputs with vision-language critics, and localizing sound outdoors with weak supervision.

- 🔭 Writing a **CVPR 2027** paper on critic-guided repair of text-to-image generations (DFAR)
- 📝 First author of **Scaling Audio Models Efficiently** ([arXiv](https://arxiv.org/abs/2606.22790), under review at ICASSP 2027)
- 🔊 Building **weakly supervised audio-visual sound localization** for outdoor environments
- 🤖 Running **PAAI**, my multi-agent personal assistant, live at [paai-six.vercel.app](https://paai-six.vercel.app/)
- 💬 Ask me about LLM agents and agent security, diffusion models and VLMs, model compression, or speech/audio ML
- 📍 College Park, MD, USA

---

### 📄 Research

| Project | Description |
|---|---|
| 🎨 [**DFAR: Critic-Guided Repair of Diffusion Outputs**](https://github.com/vyomya/DFAR) | A Qwen3-VL-8B critic inspects Stable Diffusion 1.5 generations, writes targeted edit instructions, and an autoregressive editor (VARedit) repairs the image. On the official GenEval benchmark (553 prompts x 4 samples), critic-guided repair raises macro accuracy from 42.2% to 51.0% (McNemar p ≈ 1e-45). The paper studies the instruction gap between generic, VLM-written, and oracle edit instructions, with SDXL, SD3.5, and FLUX as reference baselines. *In progress, targeting CVPR 2027.* |
| ⚙️ [**Scaling Audio Models Efficiently**](https://github.com/vyomya/SAME) · [arXiv](https://arxiv.org/abs/2606.22790) | Compute-performance tradeoffs in Whisper and wav2vec2 across model size, input length, and encoder token resolution for ASR and speech emotion recognition, with LoRA and DAMA fine-tuning. Pareto-optimal configurations deliver **4x compute savings with only an 8% accuracy drop**. *Under review at ICASSP 2027.* |
| 🔊 **Outdoor Audio-Visual Sound Event Localization** | Sound event localization and detection (SELD) for outdoor scenes, where direction-of-arrival labels are scarce and indoor-trained models degrade sharply. Uses object detection in video to derive azimuth pseudo-labels, gated by visual single-object and acoustic single-source checks and weighted by confidence, plus synthetic spatial audio for sim-to-real training on the DCASE 2025 stereo audio + video framing. *In progress.* |

---

### 🚀 Projects

| Project | Description |
|---|---|
| 🤖 [**PAAI: Personal Agentic AI Assistant**](https://github.com/vyomya/PAAI) · [Live Demo](https://paai-six.vercel.app/) | A 9-agent assistant on LangGraph: an LLM intent classifier routes each request, a planner emits a validated step plan, and specialized agents handle email summarization, prioritization, drafting, calendar, history, and preferences across Gmail, Google Calendar, and Outlook. A step evaluator checks each output against its goal and retries with targeted feedback. Memory runs on Postgres + pgvector with confidence-scored preferences that decay over time. FastAPI backend on Azure with Docker and GitHub Actions, React frontend on Vercel, Google and Microsoft sign-in, LangSmith tracing. |
| 🛡️ [**Agentic Security Guardrails**](https://github.com/vyomya/PAAI) | A six-layer defense-in-depth architecture for PAAI that contains prompt injection and untrusted tool content: provenance tagging at the tool boundary, input screening, write-gating for persistent memory, blast-radius-based human approval for irreversible actions, output screening, and a full audit trail of every tool call. Core rule: untrusted input may shape one turn of output, never persistent state or tool execution. |
| 🏗️ **Agent Studio** | An autonomous team of 6 agents (OpenClaw + Hermes Agent) with reusable skills that takes a written spec, generates and executes the code, and ships a working HTML page. Deployed on Google Cloud. |
| 📝 [**DrOCR**](https://github.com/vyomya/DrOCR) / [**LabOCR**](https://github.com/vyomya/LabOCR) | Few-shot Qwen2.5-VL-7B pipelines that transcribe handwritten medical prescriptions and scientific lab notes into structured output (abbreviations, LaTeX dosage math, reaction arrows, tables, diagram tags), with a self-critique pass for QA. WER of **12.4%** on prescriptions (vs 38.7% PaddleOCR, 44.1% Nougat, 51.2% Tesseract) and **9.05%** on lab notes. |
| 🌍 [**Wavelength**](https://github.com/mokshdagangrade/culture-fit-check) | Team project generating region-specific marketing taglines and notifications grounded in live Google Trends and Twitter trend data through RAG. I own data and evaluation: the eval harness, baselines, and error analysis. *In progress.* |
| 🍔 [**The Geography of Fast Food Pricing**](https://github.com/vyomya/restaurant-pricing) | End-to-end data science study over 1.72M menu observations from 6,717 restaurants, joined with Census, USDA, BLS, and Department of Labor data. Local income and minimum wage explain only 7.7% of price variance, while XGBoost on product identity reaches R² 0.986. |

**Exploring:** flow matching for sequential decision making (constraint-aware and value-guided policies vs diffusion policies) and LLM-guided weight editing (can an LLM agent reason over a trained model's weights to induce a targeted behavior change without fine-tuning?).

---

### 💼 Experience

**Student Researcher, University of Maryland** *(May 2026 to Aug 2026)*
Built a six-axis compute-efficiency framework for Whisper and Distil-Whisper ASR (model scale, input duration, encoder token resolution, LoRA rank, N:M sparsity, QAT), using NSGA-III to map a WER / FLOPs / peak-memory Pareto frontier. Fine-tuned Whisper large-v3 with LoRA to ~2.3% WER, implemented 2:4 sparsity with prune-and-recover fine-tuning and INT4/INT8 QAT, and ran a fault-tolerant training pipeline on RTX A6000 GPUs through SLURM.

**Research AI Engineer, Robert Bosch, Engineering R&D** *(Jan 2023 to Jul 2025)*
- **FMOps:** built a production foundation model platform (CLIP, EVA, SAM, Stable Diffusion, Mistral, Llama) for zero-shot inference, LoRA/QLoRA and DreamBooth fine-tuning, and vLLM serving on an on-prem Kubernetes GPU cluster, cutting researcher iteration time from days to hours; promoted organization-wide.
- **Agentic automation:** architected a multi-agent framework with MCP tools for PR review, documentation, and deployment workflows, adopted across 3 squads and cutting sprint overhead by 2 story points; built a codebase RAG assistant with hybrid retrieval and reranking.
- **Edge perception:** migrated a vehicle detector from MobileNet to DINO (75% → 90% accuracy, MVP approval), built real-time speed estimation on Jetson Nano with ONNX Runtime and quantization, and deployed a compressed classifier on a Raspberry Pi.
- **Generative data:** fine-tuned Stable Diffusion with DreamBooth and trained GANs to synthesize rare road scenes, expanding dataset variability by 30% and lifting perception accuracy by 4.3 percentage points.

**Earlier:** Security Intern at Deloitte USI (2022, ML-based alert classification on XSOAR, 6% fewer false positives) and Machine Learning Intern at Coneio Exim (2021, NLP classification of product descriptions into HSN trade codes at 95% accuracy).

---

### 🛠️ Tech Stack

**Languages**
![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/-C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![SQL](https://img.shields.io/badge/-SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![JavaScript](https://img.shields.io/badge/-JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![R](https://img.shields.io/badge/-R-276DC3?style=flat-square&logo=r&logoColor=white)
![Bash](https://img.shields.io/badge/-Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)

**ML / AI**
![PyTorch](https://img.shields.io/badge/-PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![HuggingFace](https://img.shields.io/badge/-🤗%20Transformers%20%7C%20PEFT-FFD21E?style=flat-square)
![TensorFlow](https://img.shields.io/badge/-TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![LangGraph](https://img.shields.io/badge/-LangGraph-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![vLLM](https://img.shields.io/badge/-vLLM-30A2FF?style=flat-square)
![ONNX](https://img.shields.io/badge/-ONNX%20Runtime-005CED?style=flat-square&logo=onnx&logoColor=white)
![OpenCV](https://img.shields.io/badge/-OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)
![scikit-learn](https://img.shields.io/badge/-scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)

**Infra & Cloud**
![FastAPI](https://img.shields.io/badge/-FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/-Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Azure](https://img.shields.io/badge/-Azure-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![AWS](https://img.shields.io/badge/-AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)
![GCP](https://img.shields.io/badge/-GCP-4285F4?style=flat-square&logo=googlecloud&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![React](https://img.shields.io/badge/-React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![SLURM](https://img.shields.io/badge/-SLURM-2C3E50?style=flat-square)

---

### 🏆 Hackathons

- **Global AI Hackathon Series, Qwen Cloud MemoryAgent Track:** extended PAAI with a Preference Agent and a History Agent for long-term agent memory
- **Deloitte USI Hackathon:** top-5 finish, leading to a security internship offer

---

<p align="center"><i>Thanks for stopping by. Always open to collaborating on ML research, agentic systems, and multimodal AI.</i></p>
