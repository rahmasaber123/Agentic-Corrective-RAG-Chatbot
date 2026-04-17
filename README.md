# 🚀 Rasheqa AI —  Diet Recommendation System

Rasheqa AI is an advanced **LangGraph-powered Retrieval-Augmented Generation (RAG)** system designed to deliver **personalized, context-aware diet recommendations**.

Unlike generic chatbots, this system operates as a **domain-restricted intelligent agent**, focused exclusively on **nutrition, diet programs, and fitness**, with strong guardrails and decision-based architecture.

---
## 🧠 RAG Architecture

![RAG Architecture](https://github.com/rahmasaber123/Agentic-Corrective-RAG-Chatbot/blob/main/corrective_rag_architecture.png?raw=true)
## 🧠 Overview

This project combines:

- Structured knowledge retrieval (RAG)
- Intelligent routing (RAG vs Web)
- Domain control (scope guard)
- Conversational memory
- Recommendation logic

→ Resulting in a **controlled, production-grade AI assistant** capable of making reliable decisions—not just generating text.

---

## ✨ Core Features

### 🔹 Hybrid RAG + Web Routing
- Dynamically selects between:
  - Internal knowledge base (high precision)
  - Web search fallback (broad coverage)
- Ensures both **accuracy and completeness**

---

### 🔹 Domain Guard (Strict Scope Control)
- Handles only:
  - Diet programs
  - Nutrition
  - Fitness
- Out-of-scope queries are:
  - Safely rejected
  - Preventing hallucinations and irrelevant responses

---

### 🔹 LangGraph Decision Engine
A structured execution pipeline:

- Retrieval
- Document grading
- Routing decision
- Scope validation
- Query transformation
- Response generation

---

### 🔹 Conversational Memory
- Sliding window memory (last 10 interactions)
- Enables:
  - Context retention
  - Personalized responses
  - Multi-turn conversations

---

### 🔹 Intelligent Recommendation System
Matches user needs to the best program using:

- Tags (e.g., appetite, weight)
- Best-fit conditions
- Program advantages

Supports use cases such as:
- Appetite control
- Weight loss
- Lifestyle improvement
- Natural solutions

---

### 🔹 External Diet Mapping
Handles queries like:
- Keto diet
- Intermittent fasting

By:
- Providing a brief explanation
- Recommending a **similar internal program**
- Highlighting key advantages

---

### 🔹 Multilingual Support
- Automatic language mirroring:
  - Arabic
  - English
- Ensures natural, consistent communication

---

## 🏗️ System Architecture


User Input
↓
Retrieve (RAG)
↓
Grade Documents
↓
Decision:
├── Generate (RAG)
└── Route Query
↓
Route Decision
↓
Scope Check
├── Reject
└── Transform Query
↓
Web Search
↓
Generate


---

## ⚙️ Tech Stack

- **LangGraph** — Workflow orchestration  
- **LangChain** — Memory & chaining  
- **LLMs (Pluggable)**:
  - GPT-4 mini (development)
  - Ollama (production deployment)
- **Vector Retrieval** — Knowledge base
- **Tavily API** — Web search fallback  

---

## 🔄 Execution Flow

1. User submits a query  
2. System retrieves relevant documents  
3. Documents are graded for relevance  
4. Decision:
   - Relevant → Answer using RAG  
   - Not relevant → Route query  
5. Router selects:
   - RAG or Web  
6. Scope validation:
   - In-domain → proceed  
   - Out-of-domain → reject  
7. Web queries are refined and executed  
8. Final response is generated  

---



### 🌐 General Nutrition (Web + Reasoning)
**Input:**  
`هل الكيتو دايت مفيد؟`

**Output:**  
- Brief explanation  
- Suggests a safer internal alternative  

---

### ❌ Out-of-Scope
**Input:**  
`عايز أتعلم بايثون`

**Output:**  
- Politely rejected  
- Maintains system integrity  

---

## 🔐 Design Principles

- **No hallucination** — answers must be grounded  
- **Deterministic routing** — no random behavior  
- **Strict domain boundaries**  
- **Separation of logic and generation**  
- **Minimal reliance on prompt for control flow**

---

## 🚀 Production Readiness

This system is designed for seamless transition to production:

- FastAPI backend integration  
- Minimal frontend (HTML/CSS/JS)  
- Ollama-based local LLM deployment  
- Scalable microservice architecture  

---

## 🔮 Future Enhancements

- Scoring-based recommendation engine (beyond prompt logic)  
- Automatic BMI-based personalization  
- Reinforcement learning from user feedback  
- Multi-model routing (speed vs intelligence)  
- Analytics & monitoring dashboard  

---

## 🧠 Why This Project Matters

Most AI assistants:
> Generate answers.

Rasheqa AI:
> **Makes decisions.**

By combining:
- Retrieval
- Reasoning
- Guardrails
- Personalization

→ It delivers a **reliable, production-grade AI system** rather than a generic chatbot.

---

## 👨‍💻 Author

**Rahma Saber**  
AI Engineer

Focused on building **scalable, real-world AI systems**
