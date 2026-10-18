<h1 align="center">Hi, I'm Manav Goel 👋</h1>
<h3 align="center">Backend & AI Engineer shipping production APIs and LLM-powered products</h3>

<p align="center">
Final-year CS student at USICT, GGSIPU. I build backend services and the AI systems that run on them: FastAPI APIs, PostgreSQL data layers, ingestion pipelines, RAG and agents, shipped to production and backed by tests and evals.
</p>

<p align="center">
<a href="https://drive.google.com/file/d/1-7Rk1a-r3y61RnpXdaQnOXNXu2QYjeJG/view?usp=sharing"><strong>📄 Resume</strong></a> ·
<a href="https://linkedin.com/in/manavgoel1104"><strong>LinkedIn</strong></a> ·
<a href="mailto:me.manavgoel@gmail.com"><strong>Email</strong></a>
</p>

---

### 💼 Experience

**AI Engineer Intern @ IntelGrader** · *Jun 2026 – Aug 2026*

Built a RAG-based assessment pipeline (Python, Gemini, LangChain, ChromaDB) over 50+ educational documents, using hybrid semantic search, BM25 reranking and LLM-based query routing to reach **95%+ chapter-classification accuracy**. Automated answer generation and grading for **1200+ exam questions** at up to **92% benchmark accuracy**, cutting manual content-review effort.

Also engineered a multi-agent pipeline that turns Class 8–12 STEM content into interactive educational webpages across **12 visual families** (LLM orchestration, Node.js, JavaScript, HTML/CSS/SVG, browser automation), with automated validation and self-repair across 25+ generated experiences to cut recurring generation and rendering failures.

**AI/ML Intern @ Hyrte** · *Dec 2025 – Feb 2026*

Redesigned LLM prompt orchestration across an interview pipeline with LangChain, improving conversational coherence and reducing repetitive system responses. Engineered a dual-layer evaluation system (heuristic + evidence-based) with adaptive difficulty progression and priority-based topic ordering. Optimized prompt structure and rolling context windows, **cutting LLM token usage by 42%** and improving response latency in a FastAPI backend.

---

### 🔭 Featured Projects

**[Groundwork](https://github.com/Manav0411/Groundwork)** · *Cited engineering Q&A agent*
`Python` `FastAPI` `LangGraph` `PostgreSQL` `pgvector` `Next.js` `Docker`

A LangGraph agent that answers questions about engineering work across GitHub, Jira and Slack, with a citation for every claim. Exact questions ("last commit by X") route to typed SQL in **under 25 ms with no model call**; everything else goes to hybrid full-text + pgvector retrieval fused with reciprocal rank fusion (**recall@8 0.807, MRR 0.941**).

Answer integrity is enforced by a model-based sufficiency grader (**0.950 accuracy**) driving a bounded CRAG corrective loop, per-marker citation validation, and an entailment check that downgrades and discloses any claim its cited passage doesn't actually state (**recall 0.909**). Deployed to production (Next.js on Vercel; FastAPI + Postgres on EC2 behind Caddy/TLS), cutting the RAG turn from **67.9 s to 1.8 s**, with releases gated on **340+ tests** plus eval suites, including a generalization suite that scored **8/8 on an unseen project**.

**[InsightGraph](https://github.com/Manav0411/InsightGraph-AI)** · *Autonomous AI intelligence pipeline*
`Python` `FastAPI` `LangGraph` `LangSmith` `pgvector`

A 6-agent LangGraph pipeline with a two-stage hallucination firewall: a semantic validator that filters irrelevant signals pre-ingestion, and a final evaluator enforcing word-count and diversity constraints, with dynamic conditional retry routing to recover from failed generations. Memory-augmented RAG via pgvector (384-dim embeddings) lets agents query historical briefings for longitudinal trend context, and tiered LLM routing (8B for parallel relevance filtering, 70B for deep analysis) keeps compute costs down. LangSmith traces all 6 agents for step-level debugging.

*Two things I'm oddly proud of:* production on Render was silently failing on a DNS-blocking issue until I migrated embedding inference to HuggingFace's `InferenceClient` SDK, and the daily delivery runs on a GitHub Actions cron job I engineered specifically to keep a free-tier backend awake through the entire pipeline run.

#### More projects

**[TeachersAid](https://github.com/Manav0411/TeachersAid)** · *AI answer-sheet extraction & grading* · `TypeScript` `Next.js` `Gemini` `Groq` `Vitest` · [Live](https://teachers-aid.vercel.app)
A teacher uploads a question paper and a student's handwritten answer sheet. In about a minute the app extracts every question, transcribes the answers, maps each answer to its question, highlights the exact ink on the sheet, grades it and writes a summary. Mapping runs deterministic label matching first and calls the LLM only for leftovers; anything below 0.55 confidence is flagged for review instead of guessed. Tested on 4 fixtures including real handwriting: **29/29 questions extracted, 28/28 confident mappings correct, 0 silent wrong mappings**. Stateless API routes on Vercel, Gemini for vision, Groq for grading, with capped concurrency and retry with backoff.

**[AskBase](https://github.com/Manav0411/AskBase)** · *AI-powered internal knowledge base* · `FastAPI` `LangChain` `FAISS` `React` `PostgreSQL`
RAG knowledge base where organizations upload policy documents and get context-grounded answers. JWT auth, role-based access control, FAISS + Cohere embeddings with MMR retrieval, Groq (LLaMA 3.3 70B) inference; deployed on Render + Vercel with rate limiting.

**[Technical-Blog-Generator](https://github.com/Manav0411/Technical-Blog-Generator)** · *LLM blog generation system* · `Python` `LangChain`
Turns a topic into a full technical blog post, optionally pulling live web research so content isn't stale, and generating and inserting images into the final article.

---

### 🎖️ Leadership

**Vice-Lead, ACM ICPC Club** · *USICT, GGSIPU · 2024 – 2026*
Organized coding contests and DSA workshops; mentored **150+ junior students** in algorithms and problem-solving, boosting participation in national coding competitions.

---

### 🏆 Achievements

- **700+ DSA problems** solved across LeetCode, GeeksforGeeks and CodeStudio
- **Level 3 Conqueror** certificate, Coding Ninjas Slayground 2.0

---

### 🎯 What I'm looking for

Open to **AI Engineer / GenAI / LLM engineering roles and new-grad positions** focused on agentic systems, retrieval, evaluation and scalable AI infrastructure.

### 💬 Ask me about

RAG architecture & hybrid retrieval, agentic pipelines (LangGraph), eval-harness design (recall@k, MRR, citation & entailment checks), LLM cost optimization, FastAPI backends, or DSA.

---

### 📊 GitHub Stats

<p align="center">
<img height="165" src="https://streak-stats.demolab.com/?user=Manav0411&theme=tokyonight&hide_border=true" />
</p>

<p align="center">
<img height="180" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Manav0411&layout=donut&theme=tokyonight&hide_border=true&langs_count=6" />
</p>

---

### 🧩 LeetCode Stats

<p align="center">
<img src="https://leetcard.jacoblin.cool/me_manaav?theme=dark&font=Karla&ext=heatmap" />
</p>

---

### ⚡ Tech Stack

**Languages**
<p align="center">
<img src="https://img.shields.io/badge/Python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54" />
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" />
<img src="https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E" />
<img src="https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white" />
<img src="https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white" />
</p>

**AI, LLMs & Evaluation**
<p align="center">
<img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white" />
<img src="https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white" />
<img src="https://img.shields.io/badge/LangSmith-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white" />
<img src="https://img.shields.io/badge/DeepEval-6C63FF?style=for-the-badge" />
<img src="https://img.shields.io/badge/Gemini-8E75B2?style=for-the-badge&logo=googlegemini&logoColor=white" />
<img src="https://img.shields.io/badge/Groq-F55036?style=for-the-badge" />
<img src="https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=ollama&logoColor=white" />
<img src="https://img.shields.io/badge/HuggingFace-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black" />
</p>

**Backend & Data**
<p align="center">
<img src="https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi" />
<img src="https://img.shields.io/badge/SQLAlchemy-D71F00?style=for-the-badge&logo=sqlalchemy&logoColor=white" />
<img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" />
<img src="https://img.shields.io/badge/pgvector-336791?style=for-the-badge" />
<img src="https://img.shields.io/badge/ChromaDB-FF6B6B?style=for-the-badge" />
<img src="https://img.shields.io/badge/FAISS-2C2D72?style=for-the-badge" />
<img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white" />
<img src="https://img.shields.io/badge/React-20232a?style=for-the-badge&logo=react&logoColor=61DAFB" />
</p>

**Infra & Testing**
<p align="center">
<img src="https://img.shields.io/badge/Docker-0db7ed?style=for-the-badge&logo=docker&logoColor=white" />
<img src="https://img.shields.io/badge/AWS_EC2-FF9900?style=for-the-badge&logo=amazonec2&logoColor=white" />
<img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white" />
<img src="https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white" />
<img src="https://img.shields.io/badge/Caddy-1F88C0?style=for-the-badge&logo=caddy&logoColor=white" />
<img src="https://img.shields.io/badge/pytest-0A9EDC?style=for-the-badge&logo=pytest&logoColor=white" />
<img src="https://img.shields.io/badge/Git-F05033?style=for-the-badge&logo=git&logoColor=white" />
</p>

---

### 🌐 Connect with Me

<p align="center">
<a href="https://linkedin.com/in/manavgoel1104"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
<a href="mailto:me.manavgoel@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" /></a>
<a href="https://github.com/Manav0411"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" /></a>
<a href="https://leetcode.com/u/me_manaav"><img src="https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" /></a>
<a href="https://codolio.com/profile/Manav0411"><img src="https://img.shields.io/badge/Codolio-6C63FF?style=for-the-badge" /></a>
</p>
