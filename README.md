# João Pedro Espanhol
**Backend Developer | Python · Django · AI/LLM Engineering**

Army officer transitioning to software engineering. I build backend systems
and LLM-powered applications, with a foundation in Python, Django, and
applied research validated in real production environments.

---

## 🛠 Technical Skills

| Domain | Technologies |
| :--- | :--- |
| **Backend** | Python, Django, SQL / PostgreSQL |
| **AI / LLM** | LangChain, LangGraph, RAG, agentic workflows, embeddings, vector stores |
| **Infrastructure** | Linux, Proxmox, Git, TCP/IP |
| **Research** | Statistical analysis, experiment design, field data collection |

---

## 🚀 Projects

### [Corrective RAG Agent](https://github.com/joao-espanhol/corrective-rag-agent)
A stateful AI agent that answers questions over financial documents
using a self-correcting retrieval loop built with LangChain and LangGraph.

- **Why LangGraph:** the agent needs cycles and conditional routing —
  if retrieval fails, it rewrites the query and retries. A plain
  LangChain chain can't express this.
- **Architecture:** `retrieve → grade relevance → generate`,
  with a corrective loop back to `retrieve` on low-relevance results.
- **Stack:** Python, LangChain, LangGraph, ChromaDB, Groq (LLaMA 3).

### [Meal & Logistics Management System](https://github.com/joao-espanhol/quartel_v2)
Full-stack Django application conceived, built, and deployed to a real
production environment inside a military unit — used daily by real users.

- Automated administrative and logistics workflows, replacing manual processes.
- **Stack:** Python, Django, PostgreSQL, Linux.

### [LoRa Telemetry Pipeline](https://github.com/joao-espanhol/LoRa_UAV)

End-to-end telemetry chain for tactical communications research: embedded
transmitter, multiple concurrent receiving stations, and a ground ingestion
server. Basis for two published field studies.

- **Ingestion:** threaded TCP server handling up to three concurrent stations.
  Buffers and frames the byte stream rather than assuming one recv per message;
  validates every record field by field; routes failures to an error log with
  the reason attached instead of dropping them.
- **Liveness:** per-station heartbeat with timeout and connection cleanup.
- **Findings:** obstruction dominates distance for ground links (SIGE/ITA 2025);
  elevating the receiver on a UAV extended the operational link to 6.3 km,
  58% beyond the ground baseline (CoBICET 2026).
- **Stack:** Python, C++, ESP32, LoRa, pandas.
---

## 📫 Connect
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/joaopedroespanhol/)
