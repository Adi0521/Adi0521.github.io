cv:
  name: Aditya (Adi) Kewalram
  label: Computer Science & Bioengineering @ UIUC
  email: adi.kewalram@gmail.com
  location: Champaign, IL
  image: ""
  summary: Junior at the University of Illinois Urbana-Champaign working across ML for biology, computational neuroscience, and ML systems.

  social_networks:
    - network: GitHub
      username: Adi0521
    - network: LinkedIn
      username: adi-kewalram

  sections:
    Education:
      - institution: University of Illinois Urbana-Champaign
        location: Urbana-Champaign, IL
        url: https://illinois.edu/
        area: Computer Science & Bioengineering, Grainger College of Engineering
        studyType: B.S.
        start_date: 2024-08
        end_date: 2028-05
        score: "GPA: 3.9/4.0"
        highlights:
          - "Honors: Dean's List"
          - "Relevant coursework: Deep Learning, Computer Vision, AI Systems and Engineering, Biologically Plausible AI, Systems Programming, Computer Architecture, Algorithms & Models of Computation, Data Structures, Linear Algebra, Differential Equations, Bioinformatics, Soft Robotics"
          - "Organizations: iMADE (Medical Advancements through Design & Engineering), Neurotech, EV Concept Design"

    Experience:
      - company: Dow Inc.
        position: Data Platform Engineer Intern
        location: Champaign, IL
        start_date: 2026-06
        end_date: present
        highlights:
          - Deployed an end-to-end automated data governance pipeline in Python on Azure and Databricks within an Agile team, processing 1,200+ Databricks resources daily and replacing manual work previously costing dozens of engineer-hours
          - Developing LangGraph agents that verify code quality and accuracy before creating resources and filing pull requests
          - Wrote SQL queries to track resources, handling concurrent additions and deletions from a shared table across 1,000+ queries per run
          - Built rate limiting and request validation for the team's chemoinformatics MCP catalog, converting internal REST APIs into MCP servers for chemical manufacturing workflows
          - Researched MCP gateways and implementations for Dow, informing the decision on the future direction of MCP server utilities and gateway setup

      - company: Engelken Lab, University of Illinois Urbana-Champaign
        position: Undergraduate Research Assistant
        location: Champaign, IL
        start_date: 2025-12
        end_date: present
        highlights:
          - Scaled spiking neural network simulations from 10,000 to 100,000 neurons, modeling cortical dynamics as a high-dimensional dynamical system with heterogeneous neuronal spike strengths
          - Implemented a leaky integrate-and-fire (LIF) network in Julia, validated against a Brian2 reference with a 15× runtime speedup
          - Added parameterized axonal delay modeling with per-seed random network generation; wrote a regression suite validating correctness across seeds

      - company: Attune NeuroFeedback (formerly Brainstorm)
        position: Model Development Engineer
        location: Champaign, IL
        start_date: 2025-02
        end_date: present
        highlights:
          - Designed a model pipeline for a VR-neurofeedback therapy system that makes EEG data easy to interpret
          - Built a facial-mesh pipeline for real-time emotion recognition using OpenCV; correlated facial movements to EEG patterns with a Random Forest classifier and Gaussian Mixture Models
          - Built a bidirectional LSTM classifier measuring user attention and focused memory usage at 85% accuracy by analyzing Gamma frequencies and the Theta-Beta ratio
          - Deployed a Multiscale Entropy (MSE) algorithm, measuring EEG signal complexity across time scales, for real-time stress prediction within the VR therapy game ahead of upcoming clinical trials

      - company: iMADE – Medical Advancements through Design and Engineering
        position: Project Manager & Technical Lead
        location: Champaign, IL
        start_date: 2024-09
        end_date: present
        highlights:
          - Managing a cross-functional team of 8 building a heart-attack detection system from PCB design through ML validation
          - Designed a custom 2-layer PCB in Eagle CAD integrating the TI ADS1298 for ECG signal acquisition and processing
          - Built an end-to-end verification pipeline validating signal fidelity from PCB acquisition through the classification stage
          - Trained GRU, LSTM, and CNN models, classifying ST-elevation in over 10,000 ECG traces at 90% sensitivity and 80% specificity

      - company: Motate
        position: Software Engineering Intern
        location: San Jose, CA
        start_date: 2025-05
        end_date: 2025-08
        highlights:
          - Implemented serverless architecture in Agile sprints for an AI-assisted dubbing and lip-syncing service supporting 15+ languages using Terraform, AWS Step Functions, Lambda, and SageMaker
          - Optimized the voice-cloning model pipeline and integrated it with the translation stage via Terraform-managed SageMaker deployments
          - Developed REST APIs backing user authorization, video upload, and translation-status Lambda functions
          - Integrated the Mailjet API into a JWT authorization Lambda function for new-user registration and confirmation

      - company: Divergence 2% LLC
        position: Undergraduate Researcher
        location: Champaign, IL
        start_date: 2024-09
        end_date: 2025-06
        highlights:
          - Built a backend inference server on NVIDIA Triton Inference Server with FastAPI and WebSockets for real-time streaming responses from conversational AI characters
          - Cut end-to-end inference latency from ~40 s to ~1.5 s (26×) by converting models to ONNX and serving through TensorRT; applied quantization and request batching to optimize serving
          - Configured multi-GPU training across 4 NVIDIA H100s with NCCL/NVLink over TCP/IP; wrote a custom CUDA kernel for fused attention
          - Fine-tuned Qwen 2.5-72B and Llama 3.1-70B with LoRA-based DPO on 100+ synthetic conversational datasets, producing more human-like responses
          - Designed an event-simulation pipeline orchestrating realistic, self-driven multi-agent LLM conversations
          - Evaluated fine-tuned models with GPT-4o-as-judge scoring; used RAG to supply character-specific context during LLM testing
          - Began with exploratory research in optical computing before moving to LLM inference and alignment work

      - company: Science Gurus
        position: Bioinformatics Intern
        location: Fremont, CA
        start_date: 2023-06
        end_date: 2023-08
        highlights:
          - Trained a model to recognize NMOSD genetic markers, separating seronegative and seropositive patients at 95% confidence
          - Identified that 9% of patients treated with Tocilizumab experience intense relapse using bioinformatics tools and clinical-trial data
          - Sorted data in R and modeled progress in NMOSD inhibition across drugs; presented findings to the founder of Aarvik Therapeutics

    Projects:
      - name: ProPredict – Agentic Protein Structure Prediction
        summary: Python, FastAPI, Celery, Redis, Postgres, Docker, Modal, LangGraph
        highlights:
          - Built a LangGraph agent that orchestrates structure prediction, physics simulation, and mutation scoring, then accepts, refines, or escalates each run, falling back to a deterministic loop on failure
          - Designed agent policies (fast, accurate, constraint-driven) that decide from ensemble uncertainty, pLDDT, and constraint checks; accept above pLDDT 80, refine at 60–80, escalate below 60
          - Raised structure-prediction accuracy (TM-score) from 0.50 to 0.87 across 88 benchmark targets by adding retrieval-based conditioning
          - Integrated ESMFold, Boltz, Chai, and GROMACS in a multi-container setup supporting ligand docking, position-specific mutations (e.g., A12V), and iterative structure refinement
          - Built a scoring pipeline with pLDDT, TM-score, and clash detection, using sha256 feature hashing to key a Redis cache across sequences and contexts
          - Deployed in two modes, docker-compose locally (FastAPI + Celery/Redis + Postgres) and Modal GPU for inference, with GitHub Actions CI and SSRF-guarded webhooks

      - name: KalshiBot – Event-Driven Trading Bot (HackIllinois 2026)
        summary: Python, C++, SQL, Flask, React, Modal, FinBERT, Groq
        highlights:
          - Built a multi-stage autonomous pipeline from 25+ RSS feeds through SentenceTransformers ticker matching, FinBERT sentiment scoring on Modal GPU (A10G), and Llama 3.3 70B signal routing via Groq for ambiguous events
          - Implemented a C++ execution layer with RSA-PSS signed limit orders at 5–7 ms construction and signing time, enforcing stop-loss, max buy-in, and sell targets on live capital
          - Executed 200+ trades at a 70%+ win rate and $50+ net profit; a background sell heartbeat monitors positions and closes on sentiment reversal
          - Filtered signals with configurable thresholds (min FinBERT score 0.70, min ticker confidence 0.40) and URL-hash deduplication
          - Stored trade and user data in SQL; built a Flask + SSE backend on Railway and a React + Vite + Three.js frontend on Vercel

      - name: Distributed CPU Inference Cluster
        summary: Ubuntu, Docker, MPI, Slurm, TCP Sockets, PyTorch, NFS, Grafana, SimGrid
        highlights:
          - Designing a daisy-chained network of CPU nodes for running models locally, communicating over TCP sockets and MPI with Slurm job scheduling and a shared NFS file system
          - Running workloads in Docker containers on Ubuntu with compiled kernels and a PyTorch runtime; monitoring the cluster through Grafana dashboards
          - Simulating the cluster in SimGrid across 8 nodes to validate the design

      - name: CPU World Model Distillation
        summary: Python, PyTorch, ONNX Runtime, DIAMOND, Atari Breakout
        highlights:
          - Distilling DIAMOND's pretrained Breakout diffusion world model into a student that runs entirely on CPU, so an RL agent can train on CPU-generated rollouts while the GPU handles distillation and policy updates
          - Designed a cheapest-first optimization ladder benchmarked as separate variants, including batched inference, torch.compile/ONNX Runtime export, static INT8 quantization, network distillation, and consistency-style sampling-step distillation
          - Specified a batched vector-environment adapter feeding DIAMOND's actor-critic learner, with a CPU throughput target derived from the transition budget a GPU reference agent needs to beat random
          - Wrote the PRD and evaluation plan, with multi-horizon dynamics validation using pixel-level event detectors and 5-seed bot comparisons in real Breakout with bootstrap confidence intervals against the GPU reference

      - name: Linux Systems Programming (CS 341)
        summary: C, POSIX, pthreads, Sockets, epoll
        highlights:
          - Built a Unix shell with fork/exec process management, background jobs, signal handling, I/O redirection, command history, and a /proc-based ps
          - Implemented a custom heap allocator (malloc/calloc/realloc/free) and a memory-leak checker
          - Wrote a TCP chat server and an epoll-based, non-blocking file server with a custom client-server protocol
          - Built multithreaded tools with pthreads, a dependency-graph parallel make and a parallel password cracker; implemented barriers, semaphores, and deadlock detection
          - Implemented CPU scheduling policies (FCFS, SJF, round robin, priority), virtual memory (MMU/TLB), a MINIX-style file system, and MapReduce

      - name: Manhunt – Live Location Game
        summary: Next.js, React, Supabase, Leaflet/OpenStreetMap, OAuth
        highlights:
          - Built a real-time location-based game with live GPS tracking, an interactive map with admin-configurable boundaries, and a competitive points/challenges system serving 250+ users with 80 peak concurrent
          - Integrated Supabase for user accounts, challenge management, and OAuth; built a Kahoot-style room system where admins create rooms, set challenges, and invite players via a shareable code
          - Implemented Leaflet/OpenStreetMap with live bus route and schedule polling, real-time player location updates, and interactive overlays; deployed on Vercel
          - Iterated on the map-boundary feature and user interface based on player feedback

      - name: BillSplitter
        summary: C++17, Crow, PostgreSQL, Vue 3, Vite, Tailwind, Tesseract OCR
        highlights:
          - Built a C++ REST backend with object-oriented design separating bills, line items, people, and split groups into distinct classes, persisted in PostgreSQL
          - Added OCR receipt scanning that drafts line items from common bill formats and screenshots, with automatic tip/tax calculation and manual override
          - Tracks a running balance per person within a split and cleans up data automatically when a group is deleted; in active use among friend groups

      - name: Reci – Social Recipe Platform
        summary: Next.js, TypeScript, Tailwind, FastAPI, SQLAlchemy, Supabase Postgres
        highlights:
          - Built the backend of a social platform for chefs with a 6-person team, a FastAPI + SQLAlchemy API on Postgres with separate profile, recipe, review, follow, and friendship tables for quick updates
          - Built frontend features with teammates in Next.js and TypeScript (recipe feed, recipe detail and add-recipe modals, rankings, and profiles) with JWT-based auth; deployed on Vercel

      - name: Course Scheduler
        summary: C++, Python, Node.js, HTML/CSS, Figma
        highlights:
          - Built a micro-scheduling algorithm and APIs that generate, suggest, and return all possible hourly breakdowns of weekly class schedules; integrated with a teammate's semester-level macro-scheduler
          - Integrated a small LLM-based RAG model to suggest offered courses based on users' interests and available time slots
          - Collaborated in a 4-person Agile/Scrum team, owning the scheduling backend and RAG integration while teammates built the HTML/CSS frontend from a Figma design

      - name: Self-Driving MiniCar
        summary: Python, C++, OpenCV, MATLAB Simulink
        highlights:
          - Preprocessed LiDAR and camera frames and used a CNN for obstacle detection, route correction, and sensor fusion for robust autonomous navigation
          - Improved times around a 400-meter route by ~4.5 seconds through model compression and algorithmic optimization for embedded constraints
          - Solo end-to-end build, from CAD-designed chassis and soldered components to coded algorithms deployed on embedded hardware; validated in MATLAB Simulink before launch

    Awards:
      - title: Dean's List
        awarder: Grainger College of Engineering, UIUC

    Skills:
      - name: Languages
        icon: fa-solid fa-code
        keywords: "Python, C++, C, Java, Julia, R, JavaScript, TypeScript, SQL, Bash, MATLAB"

      - name: ML & AI
        icon: fa-solid fa-brain
        keywords: "PyTorch, TensorFlow, OpenCV, Pandas, SentenceTransformers, LangGraph, MCP, LoRA/DPO, Reinforcement Learning, RAG, LLM-as-Judge Evaluation"

      - name: Inference & HPC
        icon: fa-solid fa-microchip
        keywords: "NVIDIA Triton Inference Server, TensorRT, ONNX, CUDA, NCCL, Quantization, Batching, Distributed Training, MPI, Slurm"

      - name: Backend & Web
        icon: fa-solid fa-server
        keywords: "FastAPI, Flask, Celery, Redis, PostgreSQL, SQLAlchemy, Supabase, Node.js, React, Next.js, Vue, Vite, Tailwind, Spring Boot, Crow, REST APIs, WebSockets, OAuth/JWT"

      - name: Cloud & Infrastructure
        icon: fa-solid fa-cloud
        keywords: "AWS (Lambda, Step Functions, SageMaker), Microsoft Azure, Databricks, Terraform, Docker, Modal, Railway, Vercel, Linux, Git, GitHub Actions, CI/CD, NFS, Grafana, SimGrid"

      - name: Systems & Networking
        icon: fa-solid fa-network-wired
        keywords: "POSIX, pthreads, GDB, Valgrind, Sockets, epoll, TCP/IP, DNS, DHCP, NTP, SMTP, SNMP"

      - name: Tools & Domain
        icon: fa-solid fa-flask
        keywords: "Agile/Scrum, Jira, Figma, Jupyter, Pytest, MATLAB Simulink, Eagle CAD, Brian2, Boltz, Chai, ESMFold, AlphaFold, GROMACS, Rosetta, PDB"