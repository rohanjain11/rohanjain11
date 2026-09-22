# Rohan Jain

MS Data Science from CU Boulder (GPA 3.9/4.0, May 2026). I build LLM systems that hold up in production, not just in demos: agents, MCP tool servers, retrieval, and the evaluation harnesses and guardrails that make them trustworthy.

📍 San Francisco, CA &nbsp;|&nbsp; 📧 jainrohanj@gmail.com &nbsp;|&nbsp; 🌐 [LinkedIn](https://www.linkedin.com/in/rohan-jain11) &nbsp;|&nbsp; 🖥 [Portfolio](https://rohanjain11.github.io/Rohan-Jain)

---

## 🛠 Skills

<p align="left">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white"/>
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white"/>
  <img src="https://img.shields.io/badge/MCP-000000?style=for-the-badge&logo=anthropic&logoColor=white"/>
  <img src="https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white"/>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white"/>
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white"/>
  <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black"/>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white"/>
  <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white"/>
  <img src="https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white"/>
  <img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white"/>
  <img src="https://img.shields.io/badge/Databricks-FF3621?style=for-the-badge&logo=databricks&logoColor=white"/>
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white"/>
  <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white"/>
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white"/>
  <img src="https://img.shields.io/badge/MLflow-0194E2?style=for-the-badge&logo=mlflow&logoColor=white"/>
</p>

**LLM and agents:** LangGraph (ReAct, multi-agent), LangChain, Model Context Protocol, tool-calling agents, RAG (BM25, embeddings, hybrid), LiteLLM gateway, Pinecone, ChromaDB, FAISS, QLoRA fine-tuning, evaluation harnesses, prompt-injection testing, guardrails, Langfuse

**Backend and data:** FastAPI, PostgreSQL + Alembic, sqlite-vec, Temporal, Docker, Kubernetes, ArgoCD, GitLab CI, GitHub Actions, Databricks (Unity Catalog, Iceberg CDC)

**ML:** scikit-learn, XGBoost, TensorFlow, Keras, PyTorch, CNN-LSTM, custom loss functions, MLflow

---

## 🎓 Education

**MS Data Science**, University of Colorado Boulder (GPA 3.9/4.0) &nbsp;|&nbsp; Aug 2024 to May 2026
**BE Computer Engineering**, Rajiv Gandhi Institute of Technology, Mumbai &nbsp;|&nbsp; Jul 2020 to May 2024

---

## 💼 Experience

**AI Engineering Intern, Bright Machines** *(Jun 2026 to Present)*

Building the production on-prem AI platform behind Bright Machines' manufacturing software: an LLM chat agent, the MCP tool servers it calls, a knowledge pipeline, and the Kubernetes and Azure deployment around them.

- Owned tool selection for an on-prem LLM agent (LangGraph ReAct over LiteLLM): 132 MCP tool schemas exceeded the 32K-token window; built a 115-question evaluation harness that raised tool recall from 0.47 to 0.97
- Killed my own recommended tool-gate design after the same harness measured it at 0.03 infrastructure recall, shipped the conditional gate instead, and stamped the correction on the original document
- Designed and shipped a read-only-by-construction MCP server from scratch (37 files, 12 tools) serving a 32,000-workflow Temporal namespace in production
- Hardened four MCP servers: closed a Critical path-traversal vulnerability (CWE-22), enforced least-privilege RBAC, replaced a fail-open deny-list with a fail-closed allow-list, and proved via adversarial prompt injection that the agent cannot execute database writes
- Root-caused a 74-minute silent chat outage while every health probe stayed green, disproved the planned fix by inspecting the running container, and shipped Postgres persistence plus a self-healing watchdog (135 tests)
- Built a grounded document Q&A platform end to end (FastAPI, React/TypeScript, sqlite-vec, OIDC) deployed to Azure AKS via ArgoCD with 350+ tests; cut LLM citation fabrication from 31% to 0%

**Data Science and Engineering Intern, Nexus Weather and Climate** *(May 2025 to May 2026)*

- Replaced baseline SVM with tuned Random Forest; reduced temperature MAE by 47% (0.73 to 0.39) and humidity MAE by 54% (4.68 to 2.37)
- Built probabilistic CNN-LSTM with custom CRPS loss for calibrated uncertainty quantification; best CRPS of 0.1787
- Implemented an automated inference quality gate rejecting models that fail to beat pre-ML baselines; reduced failed runs by 90%, saved 20 engineer-hours per month
- Ran controlled loss-function ablation experiments (Hybrid CRPS+MSE, Huberized CRPS); hybrid trained 17% faster with consistent CRPS gains of 0.01 to 0.03

**Software Developer, Kopf Lab, CU Boulder** *(Dec 2025 to May 2026)*

- Reverse-engineered Thermo Isodat binary formats (MFC CArchive C++ serialization); built deterministic R readers with inheritance-aware decoding and fail-fast validation for 7+ instrument file types
- Standardized stable isotope data ingestion across vendor formats with consistent schemas, field naming, and unit rules
- Built regression test suites with golden outputs and corruption fixtures; deployed a multi-user ShinyProxy platform with Keycloak OIDC on AWS EC2

---

## 🚀 Projects

**[ResearchAgent](https://github.com/rohanjain11/agent-research-assistant)**, Multi-Agent Research Assistant &nbsp;|&nbsp; [live demo](https://rohanjain11.github.io/agent-research-assistant/)
Four sequential agents (Researcher, Summarizer, Critic, Reporter) on LangChain and gpt-4o-mini behind a FastAPI backend that streams per-agent progress to a React UI over Server-Sent Events. Every LLM and tool call is logged as structured JSON, and the pipeline fails deliberately when sources are insufficient. About $0.01 to $0.05 per query.
`Python` `LangChain` `FastAPI` `SSE` `ChromaDB` `React` `Tailwind`

**[RoboDocs](https://github.com/rohanjain11/robotics-manual-rag)**, Robotics Manual RAG &nbsp;|&nbsp; [live demo](https://rohanjain11.github.io/robotics-manual-rag/)
Cited Q&A over about 10 Universal Robots manuals (~3,870 chunks) indexed in Pinecone serverless. Answers carry document and page citations, section-type filters, and safety callouts, with an explicit fallback when the manuals lack an answer. Ingest under $0.50, queries under $0.01.
`Python` `FastAPI` `OpenAI Embeddings` `Pinecone` `React` `Tailwind`

**[Flan-T5 QLoRA Fine-Tune](https://github.com/rohanjain11/llm-finetune-qlora)** &nbsp;|&nbsp; [adapter on Hugging Face](https://huggingface.co/rohanjain11/flan-t5-mlds-qlora)
QLoRA (8-bit, LoRA rank 16 on attention) on flan-t5-base over a 360-example synthetic QA set generated with gpt-4o-mini. ROUGE-L went from 0.1637 to 0.2058, a 25.7% gain, in 2.2 minutes on a free T4. Diagnosed an fp16 failure (zero training loss, NaN validation) and trained the adapters in fp32.
`PyTorch` `Hugging Face` `PEFT / QLoRA` `Colab T4` `ROUGE`

**[PyTorch Model Serving on Kubernetes](https://github.com/rohanjain11/pytorch-k8s-serving)**
ResNet18 (92.78%) and a BiLSTM (88.62%) served with FastAPI on Minikube, with canary routing by model version. A Horizontal Pod Autoscaler set to 2 to 6 replicas on 50% CPU scaled 2 to 6 pods under a 30-user Locust test. Prometheus metrics and a Grafana dashboard cover request rate, p50/p95 latency and traffic split.
`PyTorch` `FastAPI` `Docker` `Kubernetes` `HPA` `Locust` `Prometheus` `Grafana`

**[ClaimPilot AI](https://github.com/rohanjain11/claimpilot-ai)**, Guardrailed Tool-Calling Agent
Deterministic Pydantic v2 checks surface claim issues, then OpenAI function calling proposes structured fixes strictly scoped to what those checks found, so the model cannot invent problems. Strict output schemas with retry and fallback guarantee a valid report even when the model fails.
`Python` `Pydantic v2` `OpenAI Function Calling` `Streamlit` `pytest`

**[AgentSquared](https://github.com/rohanjain11/AgentSquared)**, No-Code AI Agent Builder *(HackCU 12)*
Config-driven platform to build AI business agents in under 60 seconds. Two modes: RAG-powered customer support, and real-time Bluesky brand monitoring with Gemini sentiment classification and human-approved threaded replies. Every agent is a DB row plus JSON config, so a new agent type is a new prompt template rather than new code.
`Python` `FastAPI` `Google Gemini API` `RAG` `Next.js` `SQLite` `Bluesky AT Protocol`

**[MLflow Weather Benchmark](https://github.com/rohanjain11/mlflow-weather-benchmark)**
Five regression models per target trained on live Open-Meteo data, with every run logged to MLflow. An automated quality gate rejects any model failing to beat a mean-prediction baseline; the best models improved MAE by 84.8% on temperature and 79.8% on humidity. CI runs a live-data smoke test on every push.
`Python` `scikit-learn` `XGBoost` `MLflow` `GitHub Actions`

**[SafeRide](https://github.com/Simrann020/Saferide)**, Risk-Aware Geospatial Routing API
Crash-aware route ranking for driving, cycling, and walking. OSRM alternatives scored via PostGIS spatial joins against crash and 311 hazard datasets. Deployed serverlessly on AWS Lambda and API Gateway with RDS.
`Python` `FastAPI` `PostgreSQL` `PostGIS` `GeoPandas` `AWS Lambda` `Docker`

**[AI PDF Chatbot](https://github.com/rohanjain11/AI-PDF-ChatBot)**, RAG Document Q&A
Full-stack RAG pipeline: OCR ingestion, LangChain chunking, FAISS similarity search, GPT-4 answers. Embedding caching, configurable retrieval parameters, usage logging. Deployed on Vercel.
`Python` `FastAPI` `LangChain` `FAISS` `OpenAI GPT-4` `React.js`

**[Denver Airport Analytics Dashboard](https://github.com/rohanjain11/Denver-Airport-Dashboard)**, Hackathon 3rd Place
Integrated ServiceNow and Azure DevOps data, then built dual Power BI dashboards with drill-downs for SLA, queue times, and bottlenecks. Reduced manual reporting by 40%.
`Python` `Power BI` `Tableau` `Power Query` `pandas`

---

## 📄 Publication

**Yoga Posture Detection and Correction**, peer-reviewed research paper. TensorFlow/Keras pose classification achieving 96.5% accuracy with real-time corrective feedback.
[View Publication](https://journals.stmjournals.com/joosdt/article=2024/view=161704/)

---

<p align="center">
  📫 Open to full-time AI Engineer, ML Engineer and Software Engineer roles.<br/>
  <a href="mailto:jainrohanj@gmail.com">jainrohanj@gmail.com</a>
</p>
