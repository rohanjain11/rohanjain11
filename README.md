# Rohan Jain

MS Data Science candidate at CU Boulder (GPA 3.9/4.0), graduating May 2026. I build production ML pipelines, LLM agents, and data systems with a focus on reliability, reproducibility, and measurable outcomes.

📍 Vista, CA &nbsp;|&nbsp; 📧 jainrohanj@gmail.com &nbsp;|&nbsp; 🌐 [LinkedIn](https://www.linkedin.com/in/rohan-jain11) &nbsp;|&nbsp; 🖥 [Portfolio](https://rohanjain11.github.io/Rohan-Jain)

---



## 🛠 Skills

<p align="left">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/R-276DC3?style=for-the-badge&logo=r&logoColor=white"/>
  <img src="https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white"/>
  <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white"/>
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white"/>
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white"/>
  <img src="https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white"/>
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white"/>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white"/>
  <img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white"/>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white"/>
  <img src="https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black"/>
  <img src="https://img.shields.io/badge/Tableau-E97627?style=for-the-badge&logo=tableau&logoColor=white"/>
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white"/>
</p>

---

## 🎓 Education

**MS Data Science** — University of Colorado Boulder (GPA 3.9/4.0) &nbsp;|&nbsp; Expected May 2026  
**BE Computer Engineering** — Rajiv Gandhi Institute of Technology, Mumbai &nbsp;|&nbsp; May 2024

---

## 💼 Experience

**Data Science & Engineering Intern — Nexus Weather and Climate** *(May 2025 - Present)*
- Replaced baseline SVM with tuned Random Forest; reduced temperature MAE by 47% (0.73 to 0.39) and humidity MAE by 54% (4.68 to 2.37)
- Built probabilistic CNN-LSTM with custom CRPS loss for calibrated uncertainty quantification; best CRPS of 0.1787
- Implemented automated inference quality gate rejecting models that fail to beat pre-ML baselines; reduced failed runs by 90%, saved 20 engineer-hours per month
- Ran controlled loss-function ablation experiments (Hybrid CRPS+MSE, Huberized CRPS); hybrid trained 17% faster with consistent CRPS gains of 0.01 to 0.03

**Graduate Research Assistant — Kopf Lab, CU Boulder** *(Dec 2025 - Present)*
- Reverse-engineered Thermo Isodat binary formats (MFC CArchive C++ serialization); built deterministic R readers with inheritance-aware decoding and fail-fast validation for 7+ instrument file types
- Standardized stable isotope data ingestion across vendor formats with consistent schemas, field naming, and unit rules
- Built regression test suites with golden outputs and corruption fixtures; deployed multi-user ShinyProxy platform with Keycloak OIDC on AWS EC2

---

## 🚀 Projects

**[ClaimPilot AI](https://github.com/rohanjain11/claimpilot-ai)** — Guardrailed LLM Agent for Healthcare Claims Validation  
Hybrid agent: deterministic Pydantic layer validates ICD-10/CPT/NPI codes; OpenAI function calling proposes structured fixes strictly scoped to detected issues. LLM cannot hallucinate beyond tool outputs. Full pytest suite, per-run artifact storage, batch eval script.  
`Python` `Pydantic v2` `OpenAI Function Calling` `Streamlit` `pytest`

**[AgentSquared](https://github.com/rohanjain11/AgentSquared)** — No-Code AI Agent Builder *(HackCU 12)*  
Config-driven platform to build AI business agents in under 60 seconds. Two modes: RAG-powered customer support and real-time Bluesky brand monitoring with Gemini sentiment classification and threaded replies. Every agent is a DB row + JSON config - no per-agent code.  
`Python` `FastAPI` `Google Gemini API` `RAG` `Next.js` `SQLite` `Bluesky AT Protocol`

**[SafeRide](https://github.com/Simrann020/Saferide)** — Risk-Aware Geospatial Routing API  
Crash-aware route ranking for driving, cycling, and walking. OSRM alternatives scored via PostGIS spatial joins against crash and 311 hazard datasets. Deployed serverlessly on AWS Lambda + API Gateway with AWS RDS.  
`Python` `FastAPI` `PostgreSQL` `PostGIS` `GeoPandas` `AWS Lambda` `Docker`

**[AI PDF Chatbot](https://github.com/rohanjain11/AI-PDF-ChatBot)** — RAG Document Q&A  
Full-stack RAG pipeline: OCR ingestion, LangChain chunking, FAISS similarity search, GPT-4 answers. Embedding caching, configurable retrieval parameters, usage logging. Deployed on Vercel.  
`Python` `FastAPI` `LangChain` `FAISS` `OpenAI GPT-4` `React.js`

**[Denver Airport Analytics Dashboard](https://github.com/rohanjain11/Denver-Airport-Dashboard)** — Hackathon 3rd Place  
Integrated ServiceNow and Azure DevOps data; built dual Power BI dashboards with drill-downs for SLA, queue times, and bottlenecks. Reduced manual reporting by 40%.  
`Python` `Power BI` `Tableau` `Power Query` `pandas`

---

## 📄 Publication

**Yoga Posture Detection and Correction** — Peer-reviewed research paper; TensorFlow/Keras pose classification achieving 96.5% accuracy with real-time corrective feedback.  
[View Publication](https://journals.stmjournals.com/joosdt/article=2024/view=161704/)

---



<p align="center">
  📫 Open to full-time roles in Data Science, ML Engineering, Data Engineering, and AI Engineering starting May 2026.<br/>
  <a href="mailto:jainrohanj@gmail.com">jainrohanj@gmail.com</a>
</p>
