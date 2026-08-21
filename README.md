<h1 align="center">Hi, I'm Manav Goel 👋</h1>
<h3 align="center">AI/ML Engineer building agentic AI systems & LLM infrastructure</h3>

<p align="center">
B.Tech CS student at USICT, GGSIPU (graduating May 2027) designing multi-agent RAG pipelines, optimizing LLM costs in production and shipping full-stack AI applications end-to-end.
</p>

<p align="center">
<a href="https://drive.google.com/file/d/1-7Rk1a-r3y61RnpXdaQnOXNXu2QYjeJG/view?usp=sharing"><strong>📄 Resume</strong></a> ·
<a href="https://linkedin.com/in/manavgoel1104"><strong>LinkedIn</strong></a> ·
<a href="mailto:me.manavgoel@gmail.com"><strong>Email</strong></a>
</p>

---

### 💼 Experience

**AI Engineer Intern @ IntelGrader** — *Jun 2026 – Aug 2026 (Remote)*

Built a multi-agent pipeline that turns Class 8–12 STEM content into interactive educational webpages across 12 visual families, using LLM orchestration, Node.js and browser automation. Wrote automated validation and self-repair workflows for 25+ generated learning experiences, checking semantic accuracy, quantitative reasoning, geometry, responsive layout and animation behavior — to cut recurring generation failures.

Also shipped a RAG-based assessment pipeline (Python, Gemini, LangChain, ChromaDB) over 50+ educational documents, using hybrid semantic search with BM25 reranking and LLM-based query routing to hit **95%+ chapter-classification accuracy**, then automated answer generation and grading for **1200+ exam questions** at up to 92% benchmark accuracy.

**AI/ML Intern @ Hyrte** — *Dec 2025 – Feb 2026 (New Delhi)*

Redesigned LLM prompt orchestration across an interview pipeline with LangChain, improving conversational coherence and killing repetitive system responses. Engineered a dual-layer evaluation system (heuristic + evidence-based) with adaptive difficulty progression and priority-based topic ordering. Optimized prompt structure and rolling context windows, **cutting LLM token usage by 42%** while improving response latency in a FastAPI backend.

---

### 🔭 Projects

**[InsightGraph](https://github.com/Manav0411/InsightGraph-AI)** — *Autonomous AI intelligence pipeline*
`Python` `FastAPI` `LangGraph` `LangSmith` `pgvector`

A 6-agent LangGraph pipeline with a two-stage hallucination firewall: a semantic validator that filters irrelevant signals pre-ingestion, and a final evaluator enforcing word-count and diversity constraints, with dynamic conditional retry routing to recover from failed generations. Memory-augmented RAG via pgvector (384-dim embeddings) lets agents query historical briefings for longitudinal trend context, and tiered LLM routing (8B for parallel relevance filtering, 70B for deep analysis) keeps compute costs down. LangSmith traces all 6 agents for step-level debugging.

*Two things I'm oddly proud of:* production on Render was silently failing on a DNS-blocking issue until I migrated embedding inference to HuggingFace's `InferenceClient` SDK — and the daily delivery runs on a GitHub Actions cron job I engineered specifically to keep a free-tier backend awake through the entire pipeline run.

**[AskBase](https://github.com/Manav0411/AskBase)** — *AI-powered internal knowledge base*
`Python` `FastAPI` `LangChain` `FAISS` `React` `PostgreSQL`

A production-ready RAG knowledge base where organizations upload policy documents and get context-grounded answers from natural language queries. REST APIs built with FastAPI, JWT auth and role-based access control; semantic search over FAISS + Cohere embeddings with MMR retrieval to reduce hallucinations. Groq (LLaMA 3.3 70B) for fast inference, full stack deployed on Render + Vercel with rate limiting.

**[Technical-Blog-Generator](https://github.com/Manav0411/Technical-Blog-Generator)** — *LLM blog generation system*
`Python` `LangChain`

Takes a topic and produces a full technical blog post — optionally pulling live web research so the content isn't stale against the model's cutoff, and generating and inserting images into the final article.

---

### 🎖️ Leadership

**Vice-Lead, ACM ICPC Club** — *USICT, GGSIPU · 2024 – Present*
Organize coding contests and DSA workshops; mentored **150+ junior students** in algorithms and problem-solving, driving campus participation in national coding competitions.

---

### 🎯 What I'm looking for

Open to **GenAI / LLM engineering roles and new-grad positions** focused on agentic systems, retrieval optimization and scalable AI infrastructure.

### 💬 Ask me about

RAG architecture, agentic pipelines (LangGraph), LLM evaluation & cost optimization, FastAPI backends, or DSA — **600+ problems solved** across LeetCode, GeeksforGeeks and CodeStudio.

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

<p align="center">
<img src="https://img.shields.io/badge/Python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54" />
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" />
<img src="https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E" />
<img src="https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white" />
</p>

<p align="center">
<img src="https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white" />
<img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white" />
<img src="https://img.shields.io/badge/LangSmith-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white" />
<img src="https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi" />
<img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white" />
<img src="https://img.shields.io/badge/React-20232a?style=for-the-badge&logo=react&logoColor=61DAFB" />
</p>

<p align="center">
<img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" />
<img src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white" />
<img src="https://img.shields.io/badge/FAISS-2C2D72?style=for-the-badge" />
<img src="https://img.shields.io/badge/ChromaDB-FF6B6B?style=for-the-badge" />
<img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=PyTorch&logoColor=white" />
<img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=TensorFlow&logoColor=white" />
</p>

<p align="center">
<img src="https://img.shields.io/badge/Docker-0db7ed?style=for-the-badge&logo=docker&logoColor=white" />
<img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white" />
<img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white" />
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
