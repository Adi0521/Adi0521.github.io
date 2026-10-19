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
    <p>Urbana-Champaign, IL</p>

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

I build at the point where machine learning meets biology and real hardware: protein structure refinement, large-scale spiking network simulation, EEG and ECG signal pipelines, and the inference and data infrastructure that makes them run fast.

Right now I'm a **Data Platform Engineer Intern at [Dow](https://corporate.dow.com/)**, continuing part-time through Fall 2026, and an undergraduate research assistant in the **Engelken Lab** at UIUC. 📄 [Resume](/assets/pdf/Adi_Kewalram_Resume.pdf)

---

### Experience

**Dow** (Jun 2026 – Present) _Data Platform Engineer Intern · Champaign, IL_

- Building an automated data governance pipeline in Python on Azure and Databricks, targeting 1,200+ resources daily and replacing manual redeployment work that cost dozens of engineer-hours
- Developed a recurring Databricks job that cleans and monitors data quality across platform pipelines

**Engelken Lab, UIUC** (Dec 2025 – Present) _Undergraduate Research Assistant_

- Scaled spiking network simulations of cortical dynamics from 10,000 to 100,000 neurons, targeting 1M
- Implemented a leaky integrate-and-fire network in Julia, validated against a Brian2 reference with a 15× runtime speedup
- Added parameterized axonal delay modeling with per-run random network generation, backed by a regression test suite across seeds

**Attune NeuroFeedback** (Feb 2025 – Present) _Model Development Engineer · startup spun out of Illinois Neurotech_

- Designed the EEG model pipeline for a VR neurofeedback therapy system, turning raw multi-channel signals into interpretable session metrics
- Trained a bidirectional LSTM to classify attention and working-memory engagement from Gamma-band power and Theta-Beta ratio (85% accuracy)
- Built real-time facial-mesh emotion recognition in OpenCV and deployed multiscale-entropy stress estimation inside the VR environment

**iMADE – Medical Advancements through Design & Engineering** (Nov 2024 – Aug 2026) _Project Manager & Technical Lead_

- Led a team of 8 building a heart-attack detection system end to end, from PCB design through ML validation
- Designed a custom 2-layer PCB around the TI ADS1298 analog front end for 8-channel ECG acquisition
- Built GRU and CNN classifiers for ST-elevation detection, plus a test pipeline verifying signal integrity from acquisition through inference

**Motate** (May 2025 – Aug 2025) _Software Engineering Intern · San Jose, CA_

- Built serverless architecture for an AI dubbing and lip-syncing service supporting 15+ languages, using Terraform, AWS Step Functions, Lambda, and SageMaker
- Optimized the voice-cloning model pipeline and wrote REST APIs for authorization, video upload, and translation status

**Divergence 2%** (Sep 2024 – Jun 2025) _Undergraduate Researcher · LLM agent research group_

- Cut end-to-end inference latency from ~40s to ~1.5s (26×) by converting models to ONNX and serving through TensorRT on NVIDIA Triton
- Fine-tuned DeepSeek, Qwen 3B, and Llama 3B with Direct Preference Optimization on 100+ synthetic preference datasets
- Ran distributed training across 4× H100 GPUs using NCCL

---

### What I work on

- ML for biology: protein structure prediction and refinement, molecular dynamics
- Computational neuroscience: spiking networks, EEG/ECG signal processing
- ML systems: fast inference, distributed training, data platforms
- Full-stack products that real people use

_Always happy to connect, so feel free to reach out!_
