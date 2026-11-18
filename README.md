## Hi, I'm Andrey 👋

**AI Engineer** with a background in backend Python development. I build conversational AI
assistants for healthcare: LLM agents, RAG, and the evaluation that shows they can be trusted.

📍 Belgrade, Serbia · open to work  
📫 [Email](mailto:andrey.volkovitskiy@gmail.com) · [Telegram](https://t.me/andrey_volkovitskiy) · [LinkedIn](https://www.linkedin.com/in/andrey-volkovitskiy)  
📄 [CV (Resume)](./--CV--.pdf)

---

### 🛠 Stack

- **LLMs & agents:** Claude API · OpenAI API · LangGraph · tool calling · structured outputs · prompt caching · MCP
- **RAG:** Qdrant · hybrid search (dense + BM25) · Voyage embeddings and rerank
- **AI evaluation & observability:** golden-set eval harness · Langfuse tracing
- **Backend:** Python · FastAPI · AsyncIO · Pydantic · PostgreSQL · SQLAlchemy (async) · gRPC · Django
- **Delivery:** Docker · Kubernetes (k3s) · GitHub Actions · Pytest · mypy
- **AI-assisted development:** Claude Code · spec-driven development (spec-kit) · custom skills and hooks

---

### 🩺 Portfolio project

**VisitDoc - an AI clinic receptionist**

**[Live demo ↗](https://visitdoc.app)** (no sign-up) · **[Repository ↗](https://github.com/Andrey-Volkovitskiy/visit-doc#readme)** · Sep–Oct 2026

A chat assistant that books, reschedules and cancels clinic appointments and answers policy/FAQ
questions with citations. When it can't answer reliably, it hands the conversation to staff
instead of guessing.

<p>
<a href="https://visitdoc.app"><img src="img/visitdoc-preview.png" alt="VisitDoc live demo: the patient chat and the staff console" width="48.5%"></a>
&nbsp;
<a href="https://github.com/Andrey-Volkovitskiy/visit-doc#readme"><img src="img/repo-preview.png" alt="The visit-doc repository README" width="45%"></a>
</p>

- **Agent:** a LangGraph flow on Claude that splits mixed-intent messages across parallel specialist nodes and merges their answers
- **RAG:** hybrid retrieval on Qdrant (Voyage embeddings + BM25, Voyage rerank) with citations, plus an abstain-and-escalate path
- **Evaluation:** a 146-case golden set, comparing every change against a committed baseline and the measured run-to-run noise. Langfuse traces each step
- **Architecture:** FastAPI services talking over gRPC, a booking service whose PostgreSQL constraints rule out double-booking, a React chat UI and staff console, an MCP connector for staff
- **Deployment:** Docker, then Kubernetes (k3s) on a VPS

One-pagers: [AI engineering](https://andrey-volkovitskiy.github.io/visit-doc/portfolio-ai-engineering.html) ·
[Development lifecycle](https://andrey-volkovitskiy.github.io/visit-doc/portfolio-adlc.html) ·
[Architecture](https://andrey-volkovitskiy.github.io/visit-doc/portfolio-architecture.html)

