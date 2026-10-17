# comfy-ai-studio
High-performance generative AI workflows and infrastructure optimization pipeline based on ComfyUI.
# ComfyUI-based High-Performance Generative AI Workflow Studio

Welcome to the official repository of **ComfyAI Studio**. This project is dedicated to designing, optimizing, and deploying advanced node-based Generative AI image and video production workflows leveraging ComfyUI. 

Our core focus is minimizing VRAM usage while maximizing generation speed and throughput for large-scale Diffusion models (SDXL, Flux, and next-generation architecture).

---

## 🚀 Project Overview

As generative models grow in parameter size, local consumer hardware often hits a performance bottleneck. This repository serves as a centralized codebase and pipeline manager for scaling ComfyUI into enterprise-level cloud infrastructure, specifically optimized for high-end cloud GPU nodes.

### Key Research Areas
* **Infrastructure Orchestration:** Automating the deployment of custom ComfyUI Docker containers on remote Linux GPU cloud servers.
* **Workflow Optimization:** Enhancing execution schedules for multi-subject generation, control networks (ControlNet), and high-resolution latent upscaling.
* **Custom Node Engineering:** Developing lightweight, specialized custom nodes to accelerate workflow automation and API-based generation pipelines.

---

## 🛠️ System Architecture & Infrastructure Requirements

To run our production-ready workflows seamlessly without memory overflows or excessive latency, the environment requires robust data throughput and top-tier computational power.

### 1. Compute & GPU Specifications
* **Minimum Requirement:** NVIDIA RTX 4090 (24GB VRAM) or NVIDIA L4 (24GB VRAM) for standard workflow benchmarking.
* **Target Infrastructure:** NVIDIA A100 (80GB VRAM) or NVIDIA H100 (80GB VRAM) clusters to support heavy multi-batch Flux.1 generation and complex LoRA training jobs.

### 2. Software Environment
* **OS:** Ubuntu 22.04 LTS / 24.04 LTS (Optimized for headless cloud environments)
* **CUDA Version:** CUDA 12.1 or higher
* **Core Libraries:** Python 3.10+, PyTorch 2.3+ (with XFormers or FlashAttention integration)

---

## 📂 Repository Structure

```text
├── .github/                 # CI/CD workflows for automated deployment
├── workflows/               # JSON and API format ComfyUI workflow schematics
│   ├── standard_sdxl/       # Optimized SDXL Base + Refiner pipelines
│   └── advanced_flux/       # Flux.1 dev/schnell enterprise configurations
├── custom_nodes/            # In-house custom nodes for API acceleration
├── scripts/                 # Shell scripts for cloud GPU driver setup & dependency installation
└── README.md                # Project documentation and infrastructure roadmap
```

---

## 🗺️ Development Roadmap

- [x] Initial workflow architectural design and node mapping.
- [ ] Establish automated environment setup scripts for standard Linux GPU instances.
- [ ] Implement VRAM allocation profiling for multi-layer ControlNet pipelines.
- [ ] Build a lightweight REST API wrapper for headless ComfyUI workflow execution.

---

## 👥 Core Contributors & Contact

* **Lead Researcher / Engineer:** [Shihwan Yoon / MyAi studio]
* **Project Inquiry:** For collaboration, infrastructure testing partnerships, or enterprise deployment queries, please open an issue in this repository.

---
*Disclaimer: This repository contains proprietary research and active codebases meant for scalable cloud cloud benchmarking. All workflows are tested extensively under strict compliance with open-source licenses.*
