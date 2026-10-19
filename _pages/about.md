---
layout: about
title: about
permalink: /
subtitle: Computer Science + Bioengineering @ <a href='https://illinois.edu/'>University of Illinois Urbana-Champaign</a>

profile:
  align: right
  image: prof_pic.jpg
  image_circular: false # crops the image to make it circular
  more_info: >
    <p>B.S. Computer Science & Bioengineering</p>
    <p>Grainger College of Engineering, UIUC</p>
    <p>Champaign, IL</p>

selected_papers: false # no publications page for now
social: true # includes social icons at the bottom of the page

announcements:
  enabled: true # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false
---

Hi there! I'm **Adi Kewalram**, a junior at the University of Illinois Urbana-Champaign studying **Computer Science and Bioengineering** in the Grainger College of Engineering.

I build at the point where machine learning meets biology, neuroscience, and systems: agentic protein structure prediction, large-scale spiking network simulation, EEG and ECG signal pipelines, and the inference and data infrastructure that makes them run fast.

Right now I'm a **Data Platform Engineer Intern at [Dow](https://corporate.dow.com/)**, building data governance pipelines, LangGraph agents, and MCP tooling, and an undergraduate research assistant in the **Engelken Lab** at UIUC. 📄 [Resume](/assets/pdf/Adi_Kewalram_Resume.pdf)

---

### Experience

**Dow Inc.** (Jun 2026 – Present) _Data Platform Engineer Intern · Champaign, IL_

- Deployed an end-to-end automated data governance pipeline in Python on Azure and Databricks, processing 1,200+ Databricks resources daily and replacing manual work that cost dozens of engineer-hours
- Developing LangGraph agents that verify code quality and accuracy before creating resources and filing pull requests
- Built rate limiting and request validation for the team's chemoinformatics MCP catalog, converting internal REST APIs into MCP servers for chemical manufacturing workflows

**Engelken Lab, UIUC** (Dec 2025 – Present) _Undergraduate Research Assistant_

- Scaled spiking neural network simulations from 10,000 to 100,000 neurons, modeling cortical dynamics with heterogeneous neuronal spike strengths
- Implemented a leaky integrate-and-fire network in Julia, validated against a Brian2 reference with a 15× runtime speedup
- Added parameterized axonal delay modeling with per-seed random network generation, backed by a regression suite across seeds

**Attune NeuroFeedback** (Feb 2025 – Present) _Model Development Engineer_

- Designed a model pipeline for a VR-neurofeedback therapy system that makes EEG data easy to interpret
- Built a bidirectional LSTM measuring attention and focused memory usage at 85% accuracy from Gamma frequencies and the Theta-Beta ratio
- Deployed a Multiscale Entropy algorithm for real-time stress prediction inside the VR therapy game, ahead of upcoming clinical trials

**iMADE – Medical Advancements through Design & Engineering** (Sep 2024 – Present) _Project Manager & Technical Lead_

- Managing a team of 8 building a heart-attack detection system from PCB design through ML validation
- Designed a custom 2-layer PCB in Eagle CAD around the TI ADS1298 for ECG acquisition and processing
- Trained GRU, LSTM, and CNN models classifying ST-elevation across 10,000+ ECG traces at 90% sensitivity and 80% specificity

**Motate** (May 2025 – Aug 2025) _Software Engineering Intern · San Jose, CA_

- Built serverless architecture for an AI dubbing and lip-syncing service supporting 15+ languages, using Terraform, AWS Step Functions, Lambda, and SageMaker
- Optimized the voice-cloning model pipeline and wrote REST APIs for authorization, video upload, and translation status

**Divergence 2%** (Sep 2024 – Jun 2025) _Undergraduate Researcher_

- Cut end-to-end inference latency from ~40s to ~1.5s (26×) by converting models to ONNX and serving through TensorRT on NVIDIA Triton
- Fine-tuned Qwen 2.5-72B and Llama 3.1-70B with LoRA-based DPO on 100+ synthetic conversational datasets
- Configured multi-GPU training across 4× H100s with NCCL/NVLink and wrote a custom CUDA kernel for fused attention

---

### What I work on

- ML for biology: agentic protein structure prediction, molecular dynamics
- Computational neuroscience: spiking networks, EEG/ECG signal processing
- ML systems: fast inference, distributed training, CPU-only models and clusters
- Full-stack products that real people use

_Always happy to connect, so feel free to reach out!_