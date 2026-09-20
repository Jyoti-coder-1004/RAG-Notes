# 🧠 RAG LAB

### *From Zero → Retrieval → Intelligence → Production*

> **Learn RAG. Build RAG. Break RAG. Improve RAG. Deploy RAG.**

<div align="center">

### 🚀 Retrieval-Augmented Generation — A Visual & Practical Journey

**Beginner-friendly • Deep Technical Knowledge • Hands-on Projects • Production**

<br>

`Python` · `LLM` · `Embeddings` · `Vector DB` · `Retrieval` · `Reranking` · `Agents`

</div>

---

## 🌌 Welcome to RAG Lab

Imagine an LLM as a brilliant person sitting in a room.

It can reason, explain, summarize and write.

But there is a problem...

> **What if the information it needs is outside the room?**

That's where **RAG** comes in.

RAG gives the LLM a way to **look outside the room, find useful information, bring it back, and use it to answer.**

```text
                  🧠 LLM
                   │
            "I need information..."
                   │
                   ▼
             🔎 RETRIEVER
                   │
             Search Knowledge
                   │
                   ▼
             📚 KNOWLEDGE
                   │
              Relevant Data
                   │
                   ▼
             🧠 LLM + CONTEXT
                   │
                   ▼
              ✨ ANSWER
```

---

# 🗺️ Your RAG Journey

Instead of reading everything at once, follow the journey.

```text
        🌱
     FOUNDATION
         │
         ▼
     📚 RAG BASICS
         │
         ▼
     🧩 BUILD RAG
         │
         ▼
     🔎 BETTER RETRIEVAL
         │
         ▼
     ⚡ ADVANCED RAG
         │
         ▼
     🤖 AGENTIC RAG
         │
         ▼
     🏭 PRODUCTION
         │
         ▼
     🚀 DEPLOYMENT
```

### Progress Map

* [ ] 🌱 Understand LLM fundamentals
* [ ] 📚 Understand RAG architecture
* [ ] 🧩 Build your first RAG
* [ ] 🔎 Master retrieval
* [ ] 🧠 Understand embeddings
* [ ] 🗄️ Work with vector databases
* [ ] ⚡ Build Hybrid RAG
* [ ] 🎯 Add reranking
* [ ] 🧪 Evaluate your RAG
* [ ] 🤖 Build Agentic RAG
* [ ] 🖼️ Explore Multimodal RAG
* [ ] 🏭 Productionize
* [ ] 🚀 Deploy

---

# ✨ What Exactly Is RAG?

## RAG = Retrieval-Augmented Generation

Break the name into three parts:

| Word          | Meaning                            |
| ------------- | ---------------------------------- |
| 🔎 Retrieval  | Find relevant information          |
| ➕ Augmented   | Add that information to the prompt |
| 🧠 Generation | LLM generates the answer           |

So:

```text
RAG
│
├── Retrieval
│      ↓
│   Find knowledge
│
├── Augmentation
│      ↓
│   Add knowledge to context
│
└── Generation
       ↓
    Generate answer
```

### 🧠 One-line definition

> **RAG is a system that retrieves relevant external knowledge and gives it to an LLM before generating an answer.**

---

# 🎯 Why Does RAG Exist?

Imagine asking an LLM:

> "What is my company's 2026 leave policy?"

The model may know nothing about your company's internal policy.

Instead:

```text
                 USER
                  │
                  ▼
       "What is our leave policy?"
                  │
                  ▼
             🔎 SEARCH
                  │
                  ▼
        📄 Company Handbook
                  │
                  ▼
          Relevant Paragraph
                  │
                  ▼
             🧠 LLM
                  │
                  ▼
        "Employees receive..."
```

Now the answer is grounded in your organization's knowledge.

---

# 🆚 Without RAG vs With RAG

### ❌ Traditional LLM

```text
User
 ↓
LLM
 ↓
Answer
```

The model primarily relies on what it already knows and what is supplied in the prompt.

### ✅ RAG

```text
User
 ↓
Retriever
 ↓
Knowledge Base
 ↓
Relevant Context
 ↓
LLM
 ↓
Answer
```

### 💡 Remember

> **LLM = reasoning + language**
>
> **RAG = access to external knowledge + reasoning + language**

---

# 🏗️ The RAG Machine

A RAG system has two major journeys.

## Journey 1 — Build the Knowledge Base

```text
📄 Documents
     │
     ▼
📖 Parse
     │
     ▼
✂️ Chunk
     │
     ▼
🧠 Embed
     │
     ▼
🗄️ Store
     │
     ▼
🔎 Searchable Knowledge
```

## Journey 2 — Answer a Question

```text
👤 User Question
       │
       ▼
    🔎 Retrieve
       │
       ▼
 📚 Relevant Chunks
       │
       ▼
   🎯 Rerank
       │
       ▼
 📝 Build Context
       │
       ▼
      🧠 LLM
       │
       ▼
    ✨ Answer
```

---

# 🔬 RAG Under the Microscope

```text
                    ┌───────────────────┐
                    │     DOCUMENTS     │
                    └─────────┬─────────┘
                              │
                              ▼
                    ┌───────────────────┐
                    │      PARSER       │
                    └─────────┬─────────┘
                              │
                              ▼
                    ┌───────────────────┐
                    │     CHUNKER       │
                    └─────────┬─────────┘
                              │
                              ▼
                    ┌───────────────────┐
                    │    EMBEDDING      │
                    │      MODEL        │
                    └─────────┬─────────┘
                              │
                              ▼
                    ┌───────────────────┐
                    │   VECTOR STORE    │
                    └─────────┬─────────┘
                              │
                              │
              ┌───────────────┘
              │
              ▼
        👤 USER QUERY
              │
              ▼
        Query Embedding
              │
              ▼
       🔎 RETRIEVAL
              │
              ▼
         Top-K Chunks
              │
              ▼
          🎯 RERANK
              │
              ▼
          📝 CONTEXT
              │
              ▼
            🧠 LLM
              │
              ▼
          ✨ ANSWER
```

---

# 🧩 RAG Building Blocks

Think of RAG as LEGO.

```text
🧱 Data
🧱 Parsing
🧱 Chunking
🧱 Embeddings
🧱 Vector Database
🧱 Retrieval
🧱 Reranking
🧱 Prompting
🧱 LLM
🧱 Evaluation
🧱 Monitoring
```

Put the blocks together correctly → **RAG system**

---

# 📚 01 — DATA

Your RAG system needs knowledge.

It could come from:

```text
📄 PDF
📝 TXT
📘 DOCX
🌐 Website
💻 GitHub
🗃️ Database
📊 CSV
🔌 API
🖼️ Images
📑 Tables
```

### Mini Challenge 🧩

> Collect 5 documents from one domain.

Examples:

* AI documentation
* college notes
* company policies
* programming documentation
* research papers

---

# ✂️ 02 — CHUNKING

A 100-page document is usually not retrieved as one giant block.

We divide it.

```text
                 DOCUMENT
                    │
        ┌───────────┼───────────┐
        ▼           ▼           ▼
      Chunk 1     Chunk 2     Chunk 3
        │           │           │
        ▼           ▼           ▼
      Vector      Vector      Vector
```

### The Chunking Question

> How big should a chunk be?

There is no universal answer.

Too small:

```text
❌ Less context
❌ Meaning can disappear
```

Too large:

```text
❌ Less precise retrieval
❌ More unnecessary tokens
```

Good RAG engineering means **testing**, not blindly choosing a number.

---

# 🧠 03 — EMBEDDINGS

Embeddings transform meaning into vectors.

```text
"Python is easy to learn"
             │
             ▼
      🧠 Embedding Model
             │
             ▼
[0.12, -0.41, 0.82, ...]
```

Now similar meanings can be compared mathematically.

```text
Query Vector
      │
      │ similarity
      ▼
Document Vectors
```

---

# 🗄️ 04 — VECTOR DATABASE

A vector database stores:

```text
Vector
+
Text
+
Metadata
```

Example:

```json
{
  "id": "chunk_42",
  "text": "Employees receive 20 days...",
  "metadata": {
    "source": "handbook.pdf",
    "page": 15,
    "department": "HR"
  }
}
```

Popular technologies include:

* Qdrant
* Pinecone
* Weaviate
* Milvus
* Chroma
* FAISS
* pgvector

---

# 🔎 05 — RETRIEVAL

This is the heart of RAG.

Question:

> "How many paid leaves are available?"

The retriever searches the knowledge base.

```text
Query
 │
 ├── Chunk 12 → 0.91 ⭐
 ├── Chunk 42 → 0.87
 ├── Chunk 05 → 0.81
 ├── Chunk 71 → 0.42
 └── Chunk 09 → 0.21
```

Then we keep the most useful results.

---

# 🎯 TOP-K

`K` = number of results retrieved.

Example:

```text
Top-K = 5
```

means:

```text
Query
 ↓
Search
 ↓
Best 5 chunks
```

But:

> **Higher K does not automatically mean better RAG.**

You need enough context without flooding the LLM with irrelevant information.

---

# ⚡ RAG EVOLUTION

This repository doesn't stop at basic RAG.

```text
                 BASIC RAG
                    │
                    ▼
              METADATA RAG
                    │
                    ▼
              HYBRID SEARCH
                    │
                    ▼
                RERANKING
                    │
                    ▼
             QUERY REWRITING
                    │
                    ▼
              MULTI-QUERY
                    │
                    ▼
             CONTEXTUAL RAG
                    │
                    ▼
              AGENTIC RAG
                    │
                    ▼
             MULTIMODAL RAG
                    │
                    ▼
             PRODUCTION RAG
```

---

# 🔀 HYBRID SEARCH

Why choose only one type of search?

Combine:

```text
        USER QUERY
             │
       ┌─────┴─────┐
       ▼           ▼
   🔵 Dense      🟡 Sparse
   Search        Search
       │           │
       └─────┬─────┘
             ▼
       Result Fusion
             │
             ▼
       Better Candidates
```

Dense search understands **meaning**.

Sparse/lexical search is useful for **exact terms**.

Together:

> Semantic understanding + keyword precision

---

# 🎯 RERANKING

Initial retrieval:

```text
100 documents
       ↓
Retriever
       ↓
20 candidates
```

Reranker:

```text
20 candidates
       ↓
Reranker
       ↓
5 highly relevant documents
```

Think:

> **Retriever = fast filter**
>
> **Reranker = careful judge of relevance**

---

# 🧪 RAG EVALUATION

Never say:

> "My RAG works because I tested it once."

Instead ask:

```text
Did we retrieve the correct information?
        ↓
Was the context relevant?
        ↓
Did the answer use that context?
        ↓
Was the answer faithful?
        ↓
Was the answer useful?
```

---

# 📊 RAG SCORECARD

Create an evaluation dataset:

```text
Question
Expected Evidence
Expected Answer
Retrieved Evidence
Generated Answer
```

Then measure:

```text
🔎 Retrieval Quality
🎯 Context Relevance
🧠 Faithfulness
💬 Answer Relevance
⚡ Latency
💰 Cost
```

---

# 🧪 RAG LAB

This repository should contain experiments.

## Experiment #01

### Does chunk size affect retrieval?

Test:

```text
250 tokens
500 tokens
750 tokens
1000 tokens
```

Compare retrieval quality.

---

## Experiment #02

### Dense vs Hybrid Retrieval

```text
Dense Search
      VS
Hybrid Search
```

Record:

```text
Accuracy
Recall
Latency
Cost
```

---

## Experiment #03

### Reranking

```text
Retriever
   VS
Retriever + Reranker
```

Document your results.

This transforms the repository from **notes** into an actual **engineering laboratory**.

---

# 🤖 AGENTIC RAG

Traditional RAG:

```text
Question
 ↓
Retrieve
 ↓
Answer
```

Agentic RAG:

```text
                  QUESTION
                     │
                     ▼
                  🤖 AGENT
                     │
          ┌──────────┼──────────┐
          ▼          ▼          ▼
       📚 RAG      🗃️ SQL     🌐 API
          │          │          │
          └──────────┼──────────┘
                     ▼
                 Synthesize
                     │
                     ▼
                  Answer
```

The system can decide:

> "Which tool should I use?"

---

# 🖼️ MULTIMODAL RAG

Knowledge isn't always text.

Modern RAG can work with:

```text
📄 Text
🖼️ Images
📊 Tables
📈 Charts
🎥 Video
🎵 Audio
```

Example:

> "What trend is shown in the sales chart?"

The retrieval pipeline can locate the relevant chart before a multimodal model analyzes it.

---

# 🕸️ GRAPH RAG

Some questions depend on relationships.

```text
Microsoft
    │
    ├── owns → GitHub
    │
    └── develops → Products
                       │
                       └── used by → Developers
```

Graph-based approaches can represent these relationships explicitly.

---

# 🏭 PRODUCTION RAG

A production system needs more than:

```text
PDF → LLM
```

It needs:

```text
🔐 Authentication
🛡️ Authorization
📊 Monitoring
🧪 Evaluation
⚡ Caching
💰 Cost Control
📝 Logging
🔄 CI/CD
🐳 Docker
☁️ Deployment
```

---

# 🚀 DEPLOYMENT JOURNEY

```text
💻 Local
   │
   ▼
🧪 Prototype
   │
   ▼
🌐 API
   │
   ▼
🐳 Docker
   │
   ▼
☁️ Cloud
   │
   ▼
📊 Monitor
   │
   ▼
🏭 Production
```

---

# 🧭 PROJECT ROADMAP

## 🟢 LEVEL 1 — Beginner

### Project: PDF Chatbot

```text
PDF
 ↓
Chunk
 ↓
Embedding
 ↓
Vector DB
 ↓
Retrieve
 ↓
LLM
```

---

## 🟡 LEVEL 2 — Intermediate

### Project: Multi-Document Knowledge Assistant

Add:

* multiple PDFs
* metadata
* citations
* document filtering
* chat history

---

## 🟠 LEVEL 3 — Advanced

### Project: Hybrid RAG

Add:

* BM25
* dense retrieval
* hybrid search
* reranking
* query rewriting
* evaluation

---

## 🔴 LEVEL 4 — Expert

### Project: Agentic RAG

Add:

* RAG
* SQL
* APIs
* web search
* tool calling
* agent routing

---

## 🟣 LEVEL 5 — Production

### Project: RAG SaaS

```text
Frontend
   +
FastAPI
   +
Authentication
   +
Vector DB
   +
LLM
   +
Evaluation
   +
Monitoring
   +
Docker
   +
Cloud
```

---

# 📁 Repository Structure

```text
rag-lab/
│
├── 📖 README.md
│
├── 🌱 01-rag-basics/
│
├── 📄 02-document-processing/
│
├── ✂️ 03-chunking/
│
├── 🧠 04-embeddings/
│
├── 🗄️ 05-vector-database/
│
├── 🔎 06-basic-rag/
│
├── 🔀 07-hybrid-rag/
│
├── 🎯 08-reranking/
│
├── 🧪 09-evaluation/
│
├── 🤖 10-agentic-rag/
│
├── 🖼️ 11-multimodal-rag/
│
├── 🏭 12-production-rag/
│
├── 🚀 deployment/
│
├── 🧪 experiments/
│
├── 📊 benchmarks/
│
├── 🧾 requirements.txt
│
├── 🔐 .env.example
│
└── 📜 LICENSE
```

---

# 🎮 RAG LEARNING SYSTEM

Turn learning into levels.

### 🟢 Level 1

**RAG Explorer**

Learn the architecture.

### 🔵 Level 2

**Retriever**

Understand embeddings and vector search.

### 🟣 Level 3

**RAG Engineer**

Build complete pipelines.

### 🟠 Level 4

**RAG Architect**

Design hybrid and advanced systems.

### 🔴 Level 5

**RAG Builder**

Deploy production applications.

---

# 💡 "THINK LIKE A RAG ENGINEER"

Whenever your RAG gives a bad answer, don't immediately blame the LLM.

Ask:

```text
❓ Did we parse the document correctly?

        ↓

❓ Did we chunk it correctly?

        ↓

❓ Are the embeddings good?

        ↓

❓ Did retrieval find the right chunks?

        ↓

❓ Did reranking help?

        ↓

❓ Did we send enough context?

        ↓

❓ Is the prompt clear?

        ↓

❓ Did the LLM generate faithfully?
```

This mindset is one of the most important skills in RAG engineering.

---

# 🧠 THE GOLDEN RULES OF RAG

### 01

> **Garbage in → garbage out.**

Bad documents produce bad retrieval.

### 02

> **More context ≠ better context.**

Relevant context matters more than volume.

### 03

> **Retrieval quality matters.**

A great LLM cannot answer from evidence it never received.

### 04

> **Always evaluate.**

Don't rely only on demos.

### 05

> **Security belongs in retrieval.**

Don't retrieve information a user isn't authorized to see.

### 06

> **Start simple.**

Don't build Agentic RAG before understanding basic RAG.

---

# 🧠 FINAL MENTAL MODEL

If you remember only one diagram from this repository, remember this:

```text
                         RAG
                          │
             ┌────────────┴────────────┐
             │                         │
        KNOWLEDGE                   QUESTION
             │                         │
             ▼                         ▼
        Documents                 User Query
             │                         │
             ▼                         ▼
          Chunking                  Embedding
             │                         │
             ▼                         ▼
         Embeddings              🔎 Retrieval
             │                         │
             ▼                         ▼
       Vector Database             Top-K
             │                         │
             └────────────┬────────────┘
                          ▼
                     🎯 Reranking
                          │
                          ▼
                     📚 Context
                          │
                          ▼
                       🧠 LLM
                          │
                          ▼
                      ✨ ANSWER
                          │
                          ▼
                   🧪 EVALUATION
```

---

# 🌟 FINAL MESSAGE

RAG is not one library.

It is not one database.

It is not one prompt.

It is an **engineering architecture**.

```text
Data
 +
Retrieval
 +
Context
 +
Generation
 +
Evaluation
 =
RAG System
```

And the journey is:

```text
🌱 Learn
   ↓
🧩 Build
   ↓
🔎 Retrieve
   ↓
⚡ Optimize
   ↓
🧪 Evaluate
   ↓
🤖 Automate
   ↓
🏭 Productionize
   ↓
🚀 Deploy
```

> **Don't just learn RAG. Build a RAG system, experiment with it, measure it, break it, improve it, and deploy it.**

---

<div align="center">

## 🚀 Welcome to RAG Lab

### Learn → Build → Experiment → Evaluate → Deploy

**Made for developers who want to understand RAG — not just copy a RAG tutorial.**

⭐ Star the repository if it helps you learn.

</div>
