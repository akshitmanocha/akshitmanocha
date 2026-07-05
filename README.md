<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=8,12,20&height=200&section=header&text=Akshit%20Manocha&fontSize=58&fontColor=fff&animation=fadeIn&fontAlignY=35&desc=Applied%20Scientist%20Intern%20%40%20Amazon%20%7C%20LLM%20Post-training%20%C2%B7%20Agentic%20Systems%20%C2%B7%20Representation%20Learning&descAlignY=57&descSize=16" />

<a href="https://readme-typing-svg.demolab.com">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&duration=3200&pause=700&color=9D4EDD&center=true&vCenter=true&width=760&lines=Applied+Scientist+Intern+%40+Amazon;LLM+Reasoning+%26+Post-training+%7C+SFT+%2B+Distillation;Agentic+Systems+%26+LLMOps+%2F+MLOps;Representation+Learning+%26+Information+Retrieval;Kaggle+Competitions+Expert+%E2%80%94+Global+Rank+19+%40+CAFA-6" alt="Typing SVG" />
</a>

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/akshit-manocha-503150285/)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:akshit_m@ch.iitr.ac.in)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/akshitmanocha)
[![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)](https://www.kaggle.com/akshitmanocha)

</div>

<br/>

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=8,12,20&height=3&width=100%"/>

## Research Focus

<img align="right" width="360" src="https://user-images.githubusercontent.com/74038190/229223263-cf2e4b07-2615-4f87-9c38-e37600f8381a.gif" />

Final-year B.Tech student at **IIT Roorkee** and **Applied Scientist Intern at Amazon**, working on machine learning systems that are measured, reproducible, and production-shaped. My work spans **LLM post-training and reasoning**, **agentic systems and LLMOps**, and **representation learning** for both language and scientific data.

I care about the full loop — from a research idea to a rigorous evaluation harness to a containerized, deployable service — and I default to *measuring* claims rather than asserting them.

**Interests**
- LLM reasoning &nbsp;·&nbsp; post-training (SFT, PEFT, distillation)
- Agentic memory &nbsp;·&nbsp; multi-agent orchestration &nbsp;·&nbsp; LLMOps / evaluation
- Representation & contrastive learning
- Information retrieval &nbsp;·&nbsp; ML for scientific discovery

<br clear="right"/>

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=8,12,20&height=3&width=100%"/>

## Experience

### Applied Scientist Intern — Amazon
`May 2026 – Aug 2026 · Bangalore` &nbsp;|&nbsp; *Representation learning · geospatial ML · uncertainty*

- Trained a **contrastive location embedding** (CLIP-style InfoNCE with a frozen geo-encoder warm-start and time-conditioned fusion) that distills operational behavior into a coordinates-plus-time "fingerprint," so delivery-time predictions generalize to **cold-start zones with no history**.
- Engineered a reusable feature pipeline over **49M+ orders** — traffic-friction speed, order density, and dwell time from delivery GPS — aggregated per zone × hour × day-of-week at multiple spatial scales.
- Built a rigorous **spatial cold-start protocol** (whole-zone / whole-city holdout, leakage-controlled ablations) to isolate generalization from memorization on a conformal delivery-window model at **90% coverage**.

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=8,12,20&height=3&width=100%"/>

## Selected Projects

### LLM Post-training & Reasoning

**NVIDIA Nemotron Reasoning Challenge** — *teaching a 30B model to reason*
Fine-tuned a **30B-parameter Nemotron** model to solve logic puzzles via supervised fine-tuning with **Unsloth**. Built an LLM pipeline that classifies every puzzle type and extracts its hidden rule, then used a larger teacher (**GPT-OSS-120B**, served with **vLLM**) to generate step-by-step reasoning and **distilled** it into the smaller model.
`SFT · PEFT/LoRA · distillation · Unsloth · vLLM`

### Agentic Systems & LLMOps

**MemEval — does agentic-memory complexity earn its cost?**
A controlled, reproducible study comparing **six LLM-agent memory strategies** (no-memory, full-context, BM25, FAISS, **Mem0**, **A-MEM**) on the **LongMemEval** benchmark under one pinned reader, scorer, and budget — measuring **accuracy *and* cost** (ingest time, query tokens, latency, store size). Crash-resilient per-system subprocess driver, bootstrap CIs, and paired-difference significance testing.
`agentic memory · evaluation · Ollama · bootstrap stats · reproducibility`

**Smart Provider Credentialing Analytics Platform** — [repo](https://github.com/akshitmanocha/Smart-Provider-Credentialing-Analytics-Platform)
A **multi-agent** system (hand-rolled supervisor: understand → plan → dispatch → synthesize) that reconciles a healthcare provider roster against authoritative sources and answers plain-English questions. The governing rule — **the LLM never computes a number** — with a deterministic numeric-**faithfulness guard**, a 3-mode backend (hosted Groq → local Ollama → deterministic fallback), and a **4-suite LLMOps evaluation scorecard** gated for CI.
`multi-agent · LLMOps · faithfulness · DuckDB · Flask · Docker`

### Representation Learning & Information Retrieval

**CAFA-6 Protein Function Prediction** — *Kaggle Global Rank 19 (Competitions Expert)*
Placed **19th of thousands** worldwide (team). Built a **multi-tower** model fusing pretrained protein language models (**ESM-2, ProtT5**) with taxonomy for 3,000-way hierarchical multi-label GO-term prediction, plus a **BLAST nearest-neighbor** transfer model — ontology-aware label propagation (True Path Rule) and IA-weighted F-max threshold selection throughout.
`ESM-2 · ProtT5 · multi-label · hierarchical classification · transfer learning`

**Beetle — hybrid semantic search engine** — [repo](https://github.com/akshitmanocha/Beetle-Search-Engine)
End-to-end retrieval system over AI/ML content: crawling, extraction, weakly-supervised quality classification, and **lexical (BM25) + dense (FAISS) + learned-sparse (SPLADE) + ColBERT** indexes fused with weighted Reciprocal Rank Fusion and a cross-encoder reranker. Improved **NDCG@10 to 0.77 from a 0.65 keyword baseline** on BEIR; shipped as a containerized **FastAPI** service with health probes, property tests, and a **DVC** pipeline.
`hybrid retrieval · SPLADE · ColBERT · RRF · FastAPI · DVC · BEIR eval`

### ML for Scientific Discovery

**Epidemic-PINN — recovering hidden transmission rates from case data**
Recovers an epidemic's time-varying transmission rate β(t) and reproduction number R(t) from reported cases alone, by backpropagating **through a differentiable SEIR simulator** (torch RK4). On Germany's first wave it tracks an independent OWID estimate to **RMSE 0.14** and beats a classical growth-rate baseline by **~10×**, with identifiability treated honestly throughout.
`physics-informed ML · differentiable simulation · inverse problems · PyTorch`

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=8,12,20&height=3&width=100%"/>

## Technical Skills

<div align="center">

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C%2FC%2B%2B-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

**ML / Deep Learning**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)

**LLM / Gen AI / Agentic**

![vLLM](https://img.shields.io/badge/vLLM-1868F2?style=for-the-badge&logo=lightning&logoColor=white)
![Unsloth](https://img.shields.io/badge/Unsloth-00C853?style=for-the-badge&logo=llama&logoColor=white)
![LoRA / PEFT](https://img.shields.io/badge/LoRA%20%2F%20PEFT-6A1B9A?style=for-the-badge&logo=pytorch&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=ollama&logoColor=white)
![FAISS](https://img.shields.io/badge/FAISS-0467DF?style=for-the-badge&logo=meta&logoColor=white)

**MLOps / LLMOps / Infra**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![DVC](https://img.shields.io/badge/DVC-945DD6?style=for-the-badge&logo=dvc&logoColor=white)
![MLflow](https://img.shields.io/badge/MLflow-0194E2?style=for-the-badge&logo=mlflow&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)

</div>

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=8,12,20&height=3&width=100%"/>

## Achievements

| Year | Achievement |
|---|---|
| 2026 | **Global Rank 19**, Kaggle CAFA-6 Protein Function Prediction |
| 2026 | **Competitions Expert**, Kaggle |
| 2025 | **AIR 26**, Amazon ML Challenge |
| 2024 | **Global Rank 46 / 1,120**, FIDE & Google Efficient Chess AI Challenge (Silver) |
| 2023 | **AIR 4441**, JEE Advanced |

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=8,12,20&height=3&width=100%"/>

## Education

**B.Tech, Chemical Engineering** — Indian Institute of Technology (IIT) Roorkee
Expected July 2027 · CGPA **8.39 / 10**

**Selected self-study:** CS229 (Machine Learning, Stanford) · CS224N (NLP with Deep Learning, Stanford) · MIT 6.S191 (Deep Learning)

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=8,12,20&height=3&width=100%"/>

## Research Map

```mermaid
graph LR
    A[Machine Learning Systems] --> B[LLM Post-training]
    A --> C[Agentic Systems and LLMOps]
    A --> D[Representation Learning]
    A --> E[Information Retrieval]
    A --> F[ML for Science]
    B --> B1[SFT and PEFT]
    B --> B2[Reasoning Distillation]
    C --> C1[Agentic Memory]
    C --> C2[Multi-agent Orchestration]
    C --> C3[Evaluation Harnesses]
    D --> D1[Contrastive Embeddings]
    D --> D2[Protein Language Models]
    E --> E1[Hybrid Retrieval and RRF]
    F --> F1[Physics-informed ML]
    style A fill:#9D4EDD,color:#fff
    style B fill:#7209B7,color:#fff
    style C fill:#7209B7,color:#fff
    style D fill:#7209B7,color:#fff
    style E fill:#7209B7,color:#fff
    style F fill:#7209B7,color:#fff
```

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=8,12,20&height=3&width=100%"/>

## GitHub Activity

<div align="center">

<img height="170em" src="https://github-readme-stats.vercel.app/api?username=akshitmanocha&show_icons=true&theme=radical&hide_border=true&bg_color=0D1117&title_color=9D4EDD&icon_color=9D4EDD&text_color=FFFFFF" />
<img height="170em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=akshitmanocha&layout=compact&theme=radical&hide_border=true&bg_color=0D1117&title_color=9D4EDD&text_color=FFFFFF" />

<img src="https://github-readme-streak-stats.herokuapp.com/?user=akshitmanocha&theme=radical&hide_border=true&background=0D1117&ring=9D4EDD&fire=9D4EDD&currStreakLabel=9D4EDD" />

<img width="95%" src="https://github-readme-activity-graph.vercel.app/graph?username=akshitmanocha&theme=react-dark&hide_border=true&bg_color=0D1117&color=9D4EDD&line=9D4EDD&point=FFFFFF" />

</div>

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=8,12,20&height=3&width=100%"/>

## Contact

<div align="center">

Open to research, MLOps / LLMOps, agentic, and Gen AI roles and collaborations.

[![LinkedIn](https://img.shields.io/badge/Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/akshit-manocha-503150285/)
[![Email](https://img.shields.io/badge/Reach_Out-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:akshit_m@ch.iitr.ac.in)

![Profile Views](https://komarev.com/ghpvc/?username=akshitmanocha&color=9D4EDD&style=for-the-badge&label=Profile+Views)

</div>

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=8,12,20&height=120&section=footer" />
