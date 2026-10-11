

<div align="center">

<!-- === SLOT 01 of 19 | hero.svg | 1600x520 | Top banner -->
<a href="https://azol-ai.vercel.app">
  <img src="./hero.svg" alt="Md Adil Muzaffar, AI/ML engineer. Creator of AZOL AI V1.0, a live multi-agent AI operating system." width="100%">
</a>

<br>

[![Live App](https://img.shields.io/badge/AZOL_AI-Live_App-635BFF?style=for-the-badge&logo=vercel&logoColor=white)](https://azol-ai.vercel.app)
[![Portfolio](https://img.shields.io/badge/Portfolio-Visit-20D9A0?style=for-the-badge&logo=googlechrome&logoColor=white)](https://md-adil-muzaffar-portfolia.lovable.app)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/md-adil-muzaffar)
[![Email](https://img.shields.io/badge/Email-Say_hello-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:adilmuzaffar96@gmail.com)

<br>

<!-- === SLOT 02 of 19 | stats.svg | 1200x170 | Key numbers strip -->
<img src="./stats.svg" alt="Key numbers: 8 LangGraph nodes, 98.42% deepfake detection accuracy, 0.9989 ROC-AUC, 280+ page design document, 4+ live AI applications, 10+ certifications" width="100%">

<!-- === SLOT 03 of 19 | divider.svg | 1200x22 | Thin divider line -->
<img src="./divider.svg" alt="" width="100%">

</div>

I am **Md Adil Muzaffar**, an AI/ML engineer focused on agentic AI and GenAI. I build AI systems end to end: agent design, retrieval, backend APIs, frontend, authentication, deployment and documentation. My flagship project, **AZOL AI V1.0**, is a multi-agent platform that I designed, built and deployed solo. I also have a published deepfake-detection framework (my M.Tech thesis) and several deployed LLM applications.

> *"We are moving from training isolated models to deploying autonomous AI systems."*

| | |
|---|---|
| 🎓 **Education** | M.Tech in Computer Science (Data Science), Jamia Hamdard University, New Delhi. CGPA 9.0+/10 |
| 🚀 **Shipped** | AZOL AI V1.0, a live 8-node LangGraph multi-agent platform |
| 📄 **Published** | Interpretable Deepfake Detection Framework: 98.42% accuracy, 0.9989 ROC-AUC |
| 🔭 **Next** | AZOL AI V2.0: autonomous data intelligence (database connectors, NL-to-SQL, live dashboards) |
| 🎯 **Looking for** | AI Engineer · GenAI / LLM Engineer · AI Agent Engineer · Applied ML Engineer |
| 📍 **Based in** | Patna, India. Open to relocation. Immediate joiner |

<br>

<!-- === SLOT 04 of 19 | h-featured.svg | 1200x108 | Heading: Featured product -->
<img src="./h-featured.svg" alt="Featured product: AZOL AI V1.0, live in production" width="100%">

**An autonomous multi-agent AI operating system.** Give it a goal in plain language. It plans, researches, analyzes, executes and verifies the work, then streams back a result you can inspect.

<div align="center">

<!-- === SLOT 05 of 19 | azol-landing-preview.png | 1146x640 | AZOL landing page screenshot (PNG) -->
<a href="https://azol-ai.vercel.app">
  <img src="./azol-landing-preview.png" alt="AZOL AI landing page: Your AI workforce. Working as one." width="92%">
</a>

<br><br>

<!-- === SLOT 06 of 19 | pipeline.svg | 1200x150 | Plan > Research > Analyze > Execute > Verify -->
<img src="./pipeline.svg" alt="Plan, Research, Analyze, Execute, Verify: the AZOL AI execution pipeline" width="100%">

<br>

[**Launch the live app**](https://azol-ai.vercel.app) · [**Source code**](https://github.com/mdadilmuzaffar24/AZOL-AI) · [**Portfolio case study**](https://md-adil-muzaffar-portfolia.lovable.app)

<!-- Add your YouTube walkthrough here, for example:
[**Watch the 1080p walkthrough**](https://www.youtube.com/watch?v=YOUR_VIDEO_ID) · -->

</div>

> The API may be asleep when idle, so the **first load can take up to a minute** while it wakes up. After that it is fast.

### Why it is different from a chatbot

| | A typical AI chatbot | AZOL AI |
|---|---|---|
| **Scope** | One prompt, one answer | One goal, multi-step execution across specialist agents |
| **Trust** | You fact-check the answer | A QA Reviewer node audits claims against sources before delivery |
| **Risk** | Runs whatever it is asked | Human-in-the-loop approval gate (`interrupt()`) for high-risk steps |
| **Memory** | Forgets between sessions | Persistent project memory (FAISS + PostgreSQL checkpoints) |
| **Isolation** | Flat chat history | Multi-tenant workspaces scoped by user |

### How a goal flows through the system

```mermaid
flowchart TD
    A([Operator goal]) --> B[Auth and RBAC gate]
    B --> C[Supervisor router<br/>LangGraph]
    C --> D[Planner<br/>task decomposition]
    C --> E[Researcher<br/>live web + FAISS RAG]
    C --> F[Data Analyst<br/>Python sandbox]
    C --> G[Coding Agent<br/>scripts and artifacts]
    D --> H[QA Reviewer<br/>grounding and citation audit]
    E --> H
    F --> H
    G --> H
    H --> I{{Human approval gate}}
    I -->|approved| J[(Persistent memory<br/>FAISS + PostgreSQL)]
    J --> K([Verified, streamed output and artifacts])

    classDef core stroke:#635BFF,stroke-width:2px
    classDef gate stroke:#20D9A0,stroke-width:2px
    class C,H core
    class B,I gate
```

### What is inside V1.0

| Capability | Details |
|---|---|
| 🧠 **Multi-agent orchestration** | LangGraph supervisor routes work across Planner, Researcher, Data Analyst, Coding and QA Reviewer nodes |
| 📚 **RAG knowledge base** | 5-stage ingestion for PDF, DOCX, PPTX, CSV and TXT. FAISS with `BAAI/bge-small-en-v1.5` embeddings and project-scoped retrieval |
| ⚡ **Live workspace** | React 18 workspace with SSE token streaming, a live React Flow agent graph, and 7 tabs per project (overview, chat, documents, tasks, agents, memory, outputs) |
| 🛡️ **Security** | Google OAuth 2.0, email OTP, HttpOnly JWT cookies, PostgreSQL token-revocation blacklist, rate limiting |
| 📈 **Telemetry** | Execution metrics, token usage and latency views with CSV export |
| ☁️ **Deployment** | Frontend on Vercel, FastAPI on Render, PostgreSQL on Neon. Docker Compose for local infrastructure |
| 📝 **Documentation** | README, 1080p walkthrough video and a 280+ page software design document |

<details>
<summary><b>🔭 Roadmap: V2.0 and beyond (planned)</b></summary>

<br>

**V2.0: From AI workforce to autonomous data intelligence**

- **Database connectors:** read-only access to PostgreSQL, MySQL, MongoDB, Snowflake and CSV/Excel
- **NL-to-SQL and cleaning:** schema introspection, query generation, variance analysis and anomaly detection
- **Live BI dashboards:** interactive dashboards generated from plain-language questions

**Beyond:** an autonomous business OS where agents, data and knowledge work together across a team.

*Everything in this roadmap is planned. V1.0 is what is live today.*

</details>

<br>

<!-- === SLOT 07 of 19 | h-research.svg | 1200x108 | Heading: Published research -->
<img src="./h-research.svg" alt="Published research: peer-reviewed, with a live app" width="100%">

<!-- === SLOT 08 of 19 | card-research.svg | 1200x330 | Deepfake research card -->
<img src="./card-research.svg" alt="Interpretable Deepfake Detection Framework: MTCNN, Xception, Grad-CAM and SHAP. 98.42% accuracy, 0.9989 ROC-AUC, 10,000+ training images, tested on FaceForensics++" width="100%">

<div align="center">

[**Read the paper (DOI)**](https://doi.org/10.5281/zenodo.20470289) · [**Try the live app**](https://universal-deepfake-forensics.streamlit.app) · [**Source code**](https://github.com/mdadilmuzaffar24/Interpretable-Deepfake-Detection)

</div>

<br>

<!-- === SLOT 09 of 19 | h-projects.svg | 1200x108 | Heading: More projects -->
<img src="./h-projects.svg" alt="More projects, built end to end" width="100%">

<div align="center">

<a href="https://github.com/mdadilmuzaffar24/AI-Ledger-Agent"><img src="./card-ledger.svg" alt="AI Financial and Ledger Agent: about 80% less manual invoice entry. LangChain, Llama 3.1 on Groq, Pydantic, Streamlit" width="49%"></a><!-- SLOT 10 of 19 | card-ledger.svg | 584x268 | Project card 1 (AI Ledger Agent) -->
<a href="https://github.com/mdadilmuzaffar24/AI-Document-Chatbot"><img src="./card-rag.svg" alt="AI Document Chatbot with RAG: PDF, Word and text. LangChain, FAISS, MiniLM, Streamlit" width="49%"></a><!-- SLOT 11 of 19 | card-rag.svg | 584x268 | Project card 2 (Document Chatbot) -->

<a href="https://github.com/mdadilmuzaffar24/Autism_Predicition_ML_project"><img src="./card-asd.svg" alt="Autism Spectrum Disorder Screening: 0.96 cross-validated ROC-AUC. XGBoost, scikit-learn, SMOTETomek, SHAP" width="49%"></a><!-- SLOT 12 of 19 | card-asd.svg | 584x268 | Project card 3 (Autism screening) -->
<a href="https://github.com/mdadilmuzaffar24/Fake_News_Prediction"><img src="./card-news.svg" alt="Fake News Detection: 98.4% accuracy with Linear SVM. TF-IDF, scikit-learn" width="49%"></a><!-- SLOT 13 of 19 | card-news.svg | 584x268 | Project card 4 (Fake News) -->

</div>

<br>

<!-- === SLOT 14 of 19 | h-stack.svg | 1200x108 | Heading: Tech stack -->
<img src="./h-stack.svg" alt="Tech stack: agents, ML, backend, frontend, cloud" width="100%">

<!-- === SLOT 15 of 19 | stack.svg | 1200 wide | Tech stack panel -->
<img src="./stack.svg" alt="Tech stack: LangGraph, LangChain, RAG, MCP, Groq, Ollama, FAISS, Python, PyTorch, TensorFlow, Keras, scikit-learn, XGBoost, OpenCV, FastAPI, PostgreSQL, Redis, Docker, React, Vite, Tailwind, Vercel, Render, Neon, Azure AI, Git" width="100%">

<br>

<!-- === SLOT 16 of 19 | h-experience.svg | 1200x108 | Heading: Experience -->
<img src="./h-experience.svg" alt="Experience, 2023 to present" width="100%">

**Founder & Independent AI Systems Engineer, AZOL AI** · *2026 to present, self-directed*<br>
Designed, built, deployed and documented a production multi-agent platform end to end: LangGraph orchestration, RAG, security, a React workspace, cloud deployment and a 280+ page design document.

**Artificial Intelligence Intern**, Edunet Foundation (Microsoft, AICTE) · *Apr 2025 to May 2025*<br>
Built the XGBoost autism-screening model (0.96 CV ROC-AUC) and deployed an image classifier on Azure Custom Vision.

**Data Science Intern**, Internshala Trainings (Remote) · *Jun 2023 to Oct 2023*<br>
Built a weather-forecast model in Python, analysed IPL ball-by-ball data with SQL for an auction-strategy simulation, and built a Tableau sales dashboard.

<br>

<!-- === SLOT 17 of 19 | h-credentials.svg | 1200x108 | Heading: Credentials -->
<img src="./h-credentials.svg" alt="Education and credentials: M.Tech and 10+ certifications" width="100%">

**M.Tech, Computer Science Engineering (Data Science)**, Jamia Hamdard University, New Delhi · *2024 to 2026* · CGPA 9.0+/10<br>
**B.Tech, Electrical & Electronics Engineering**, MACET, Patna · *2018 to 2022* · CGPA 7.6/10

<details>
<summary><b>🎓 Certifications (10+)</b></summary>

<br>

| Certification | Issuer | Date |
|---|---|---|
| [Agentic AI with LangChain and LangGraph](https://www.coursera.org/verify/FADJ5PHL5L9E) | IBM | Sep 2026 |
| Introduction to Model Context Protocol · MCP: Advanced Topics | Anthropic | Aug 2026 |
| MLOps and Data Pipeline Orchestration for AI Systems | LinkedIn Learning | Jul 2026 |
| Deep Learning Specialization | DeepLearning.AI (Andrew Ng) | Apr 2026 |
| Machine Learning Specialization | Stanford University | Aug 2025 |
| IBM Data Science Professional Certificate | IBM / Coursera | Jun 2025 |
| AI/ML for Crop Acreage Mapping | ISRO IIRS | Apr 2025 |
| Generative AI for Data Science | Microsoft | Mar 2025 |
| Python for Data Analysis and Visualization | Coursera | Mar to Apr 2025 |
| Microsoft Azure AI Essentials Professional Certificate | LinkedIn Learning | |

</details>

<br>

<!-- === SLOT 18 of 19 | h-community.svg | 1200x108 | Heading: Community -->
<img src="./h-community.svg" alt="Community: AI Updates on LinkedIn and Instagram" width="100%">

I run the **AI Updates** series on LinkedIn and Instagram, explaining agentic AI and frontier-model research with verified data points to an audience of 1,500+ followers.

<br>

<div align="center">

### Let's build something

I am looking for AI Engineer, GenAI Engineer and AI Agent Engineer roles, and I can join immediately.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/md-adil-muzaffar)
[![Portfolio](https://img.shields.io/badge/Portfolio-Visit-20D9A0?style=for-the-badge&logo=googlechrome&logoColor=white)](https://md-adil-muzaffar-portfolia.lovable.app)
[![Email](https://img.shields.io/badge/adilmuzaffar96%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:adilmuzaffar96@gmail.com)

<br>

<!-- === SLOT 19 of 19 | footer.svg | 1600x300 | Closing banner -->
<img src="./footer.svg" alt="I don't just train models. I engineer and ship AI systems to production. Md Adil Muzaffar, AZOL AI." width="100%">

<sub>If AZOL AI or any of these projects is useful to you, a ⭐ on the repo is appreciated.</sub>

</div>
