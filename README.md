<h1 align="center">Jhonatan Rodriguez Custodio</h1>

<p align="center">
  <b>AI Engineer · Azure & Generative AI</b><br/>
  I design and ship multimodal RAG systems and multi-agent architectures that run in production.
</p>

<p align="center">
  <a href="https://jhonatanrc03.pythonanywhere.com/"><img alt="Portfolio" src="https://img.shields.io/badge/Portfolio-Live%20AI%20assistant-0A66C2?style=for-the-badge&logo=googlechrome&logoColor=white"></a>
  <a href="https://www.linkedin.com/in/jrc03/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-jrc03-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"></a>
  <a href="mailto:jhonatan9494@gmail.com"><img alt="Email" src="https://img.shields.io/badge/Email-Contact-EA4335?style=for-the-badge&logo=gmail&logoColor=white"></a>
</p>

<p align="center">
  <img alt="Location" src="https://img.shields.io/badge/📍-Perú-555">
  <img alt="Experience" src="https://img.shields.io/badge/Applied%20AI-3%2B%20years-6E40C9">
  <img alt="Production" src="https://img.shields.io/badge/Systems%20in%20production-10%2B-2EA043">
  <img alt="Certs" src="https://img.shields.io/badge/Microsoft%20certifications-6-0078D4?logo=microsoft&logoColor=white">
</p>

---

### About me

Systems Engineer specialized in Artificial Intelligence. I build end-to-end AI solutions on Microsoft Azure: from document ingestion and hybrid retrieval to agent orchestration, APIs and production deployment.

- 🤖 **Multi-agent systems** on Azure AI Foundry and Microsoft Agent Framework, with Human-in-the-Loop where decisions are irreversible.
- 📚 **Multimodal RAG**: hybrid search, semantic ranking and answers with citations traceable to the source document.
- 📄 **Document AI**: structured extraction from contracts, IDs, legal powers and financial documents with Document Intelligence + LLMs.
- ☁️ **Cloud-native delivery**: App Service, Functions, Container Apps and AKS, secured with Key Vault and Entra ID and observed with Application Insights.
- 🎓 Mentor at GenAI hackathons and instructor of Azure AI Foundry workshops.

> 💬 My [portfolio](https://jhonatanrc03.pythonanywhere.com/) has an AI assistant that knows my CV. Ask it anything about my experience.

---

### What I've built in production

Corporate solutions developed at **Gestión de Sistemas** (Jan 2025 – present). Code is private; architectures and design decisions are documented in my [portfolio](https://jhonatanrc03.pythonanywhere.com/).

| Project | Type | What it does | Key stack |
|---|---|---|---|
| **Risk Agents** | Multi-agent | An orchestrator splits credit-risk evaluation across agents for history, macro/sector context (web grounding) and financial ratios (OpenAPI tools), then consolidates a rated report. | AI Foundry · Azure OpenAI · Functions · FastAPI · React |
| **Dispute Management Agents** | Multi-agent | Six sequential agents automate card disputes, from intake to resolution, with a mandatory human approval gate before chargebacks. | AI Foundry Hosted Agents · Agent Framework · Container Apps |
| **Transactional Fraud** *(in development)* | Agent | An analyst agent weighs customer-behavior evidence and issues a risk verdict justified factor by factor for human review. | AI Foundry · Container Apps · Cosmos DB · Entra ID |
| **AVI — Document Chatbot** | Multimodal RAG | Natural-language Q&A over institutional documents with hybrid search, semantic ranker and source citations. | Azure OpenAI · GPT-4 Vision · AI Search · Cosmos DB |
| **Document Knowledge** | Cloud architecture | Enterprise knowledge platform on AKS that decouples batch ingestion from a low-latency chat service. | AKS · Semantic Kernel · AI Search · Cosmos DB |
| **Helpdesk Assistant** | RAG | Support desk that answers incidents citing the exact procedure from indexed manuals. | Azure OpenAI · AI Search · Application Insights |
| **Document Processor** | Document AI | Serverless extraction of key fields from contracts, tax IDs, national IDs and promissory notes, with SFTP sync and signature validation. | Functions · Document Intelligence · Logic Apps |
| **Legal Powers Analyzer** | Document AI | Extracts attorneys-in-fact, powers, amount limits and validity from legal deeds and generates downloadable summaries. | Azure OpenAI · Document Intelligence · Key Vault |
| **Smart Recruiting** | AI search | Automated CV analysis that extracts candidate profiles and ranks them semantically. | Document Intelligence · AI Search · OpenAI |

<details>
<summary><b>Reference architecture: how my multi-agent systems are shaped</b></summary>
<br/>

```mermaid
flowchart LR
    U([User / Analyst]) --> API[FastAPI / App Service]
    API --> O{{Orchestrator agent}}
    O --> A1[Specialist agent<br/>internal data]
    O --> A2[Specialist agent<br/>web grounding]
    O --> A3[Specialist agent<br/>OpenAPI tools]
    A1 & A2 & A3 --> C[Consolidation agent]
    C --> H{Human-in-the-Loop}
    H -->|approved| R[(Report / Action)]
    A1 -.-> S[(AI Search · Cosmos DB)]
```

Every agent works on an explicit data contract. Code prepares the case file, the agent applies judgment, and irreversible actions always pass through human approval.

</details>

---

### Tech stack

**AI & agents**<br/>
<img src="https://img.shields.io/badge/Azure%20AI%20Foundry-0078D4?style=flat-square&logo=microsoftazure&logoColor=white">
<img src="https://img.shields.io/badge/Azure%20OpenAI-412991?style=flat-square&logo=openai&logoColor=white">
<img src="https://img.shields.io/badge/Microsoft%20Agent%20Framework-5C2D91?style=flat-square&logo=microsoft&logoColor=white">
<img src="https://img.shields.io/badge/Semantic%20Kernel-512BD4?style=flat-square&logo=dotnet&logoColor=white">
<img src="https://img.shields.io/badge/MCP-Model%20Context%20Protocol-000000?style=flat-square">
<img src="https://img.shields.io/badge/RAG-Hybrid%20%2B%20Semantic%20Ranker-2EA043?style=flat-square">
<img src="https://img.shields.io/badge/Prompt%20Engineering-FF6F00?style=flat-square">

**Document AI & computer vision**<br/>
<img src="https://img.shields.io/badge/Document%20Intelligence-0078D4?style=flat-square&logo=microsoftazure&logoColor=white">
<img src="https://img.shields.io/badge/Content%20Understanding-0078D4?style=flat-square&logo=microsoftazure&logoColor=white">
<img src="https://img.shields.io/badge/GPT%20Vision-412991?style=flat-square&logo=openai&logoColor=white">
<img src="https://img.shields.io/badge/YOLOv8-00FFFF?style=flat-square&logo=yolo&logoColor=black">
<img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white">
<img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white">

**Azure cloud**<br/>
<img src="https://img.shields.io/badge/AI%20Search-0078D4?style=flat-square&logo=microsoftazure&logoColor=white">
<img src="https://img.shields.io/badge/App%20Service-0078D4?style=flat-square&logo=microsoftazure&logoColor=white">
<img src="https://img.shields.io/badge/Functions-0062AD?style=flat-square&logo=azurefunctions&logoColor=white">
<img src="https://img.shields.io/badge/Container%20Apps-0078D4?style=flat-square&logo=microsoftazure&logoColor=white">
<img src="https://img.shields.io/badge/AKS-326CE5?style=flat-square&logo=kubernetes&logoColor=white">
<img src="https://img.shields.io/badge/Logic%20Apps-0078D4?style=flat-square&logo=microsoftazure&logoColor=white">
<img src="https://img.shields.io/badge/Key%20Vault-0078D4?style=flat-square&logo=microsoftazure&logoColor=white">
<img src="https://img.shields.io/badge/Application%20Insights-68217A?style=flat-square&logo=microsoftazure&logoColor=white">

**Backend & frontend**<br/>
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white">
<img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white">
<img src="https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white">
<img src="https://img.shields.io/badge/Quart-3B3B3B?style=flat-square">
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white">
<img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB">
<img src="https://img.shields.io/badge/Angular-DD0031?style=flat-square&logo=angular&logoColor=white">
<img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white">

**Data & databases**<br/>
<img src="https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white">
<img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white">
<img src="https://img.shields.io/badge/PySpark-E25A1C?style=flat-square&logo=apachespark&logoColor=white">
<img src="https://img.shields.io/badge/Databricks-FF3621?style=flat-square&logo=databricks&logoColor=white">
<img src="https://img.shields.io/badge/Power%20BI-F2C811?style=flat-square&logo=powerbi&logoColor=black">
<img src="https://img.shields.io/badge/Cosmos%20DB-0078D4?style=flat-square&logo=microsoftazure&logoColor=white">
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white">
<img src="https://img.shields.io/badge/SQL%20Server-CC2927?style=flat-square&logo=microsoftsqlserver&logoColor=white">
<img src="https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white">
<img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white">

---

### Microsoft certifications

| | Certification | Level |
|---|---|---|
| <img src="https://img.shields.io/badge/AI--102-0078D4?style=flat-square&logo=microsoft&logoColor=white"> | [Azure AI Engineer Associate](https://learn.microsoft.com/api/credentials/share/es-es/JhonatanRodriguezCustodio-7265/8AA0D450EA13F82D?sharingId=741F47D64D5A545A) | Associate |
| <img src="https://img.shields.io/badge/DP--100-0078D4?style=flat-square&logo=microsoft&logoColor=white"> | [Azure Data Scientist Associate](https://learn.microsoft.com/api/credentials/share/es-es/JhonatanRodriguezCustodio-7265/1658F7EFBA648D3E?sharingId=741F47D64D5A545A) | Associate |
| <img src="https://img.shields.io/badge/AB--731-5C2D91?style=flat-square&logo=microsoft&logoColor=white"> | [AI Transformation Leader](https://learn.microsoft.com/api/credentials/share/es-es/JhonatanRodriguezCustodio-7265/96D3C54F9F20FAE5?sharingId=741F47D64D5A545A) | Professional |
| <img src="https://img.shields.io/badge/AB--730-5C2D91?style=flat-square&logo=microsoft&logoColor=white"> | [AI Business Professional](https://learn.microsoft.com/api/credentials/share/es-es/JhonatanRodriguezCustodio-7265/BA8640C8A29E6650?sharingId=741F47D64D5A545A) | Professional |
| <img src="https://img.shields.io/badge/AI--900-50E6FF?style=flat-square&logo=microsoft&logoColor=black"> | [Azure AI Fundamentals](https://learn.microsoft.com/api/credentials/share/es-es/JhonatanRodriguezCustodio-7265/4298E8369C4AE17A?sharingId=741F47D64D5A545A) | Fundamentals |
| <img src="https://img.shields.io/badge/DP--900-50E6FF?style=flat-square&logo=microsoft&logoColor=black"> | [Azure Data Fundamentals](https://learn.microsoft.com/api/credentials/share/es-es/JhonatanRodriguezCustodio-7265/E334CB8251A8D2B8?sharingId=741F47D64D5A545A) | Fundamentals |

---

### Experience

**AI Engineer** · Gestión de Sistemas · Perú · *Jan 2025 – present*<br/>
Design and delivery of RAG, document-AI and multi-agent solutions for enterprise clients in banking, finance, legal and HR, deployed on Azure.

**Data Science & Analytics Jr** · Shintek · Spain (remote) · *Jul 2024 – Dec 2024*<br/>
Improved object-detection precision and efficiency by 20% with YOLO and transfer learning. Built KPI dashboards and prepared data for predictive models.

**Community**<br/>
Mentor at the GenAI Hackathon Interbank (Nov 2025) and the Bago Hackathon on Azure AI Foundry (Jun 2026) · Instructor of an Azure AI Foundry workshop at Habitat (Aug 2026)

---

### Featured public repositories

| Repository | Description |
|---|---|
| [CV-Jhonatan-Rodriguez-Custodio](https://github.com/JhonatanRC03/CV-Jhonatan-Rodriguez-Custodio) | My portfolio: Flask + vanilla JS with a streaming AI assistant on Azure AI Foundry, per-IP rate limiting and data-driven architecture diagrams. |
| [taller-azure-ia](https://github.com/JhonatanRC03/taller-azure-ia) | Hands-on Azure AI workshop: step-by-step labs and a chat app. |
| [fraud_detect](https://github.com/JhonatanRC03/fraud_detect) | Machine-learning model for fraud detection. |
| [Credit-Scoring-Prediction](https://github.com/JhonatanRC03/Credit-Scoring-Prediction) | Credit-default probability model for a financial institution. |
| [practica-mlops](https://github.com/JhonatanRC03/practica-mlops) · [despliegue-ml](https://github.com/JhonatanRC03/despliegue-ml) | MLOps practice and cloud deployment examples for ML models. |

---

<p align="center">
  <b>Open to AI Engineer opportunities</b>: GenAI, RAG and agentic systems on Azure.<br/>
  <a href="https://www.linkedin.com/in/jrc03/">LinkedIn</a> · <a href="mailto:jhonatan9494@gmail.com">jhonatan9494@gmail.com</a> · <a href="https://jhonatanrc03.pythonanywhere.com/">Portfolio</a>
</p>
