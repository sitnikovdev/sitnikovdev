# Hi 👋 I'm Oleg

iOS developer (Swift, UIKit, SwiftUI) currently transitioning into **AI Engineering**.

I keep public notes here as I work through building LLM applications — from a first RAG pipeline to agents that decide on their own when and what to do. I used to design state and side effects in TCA — now I'm learning to design the behavior and decisions of LLM systems. A lot of the mindset carries over: predictability, testability, and clear boundaries of responsibility matter in both worlds.

These aren't a retelling of any course — they're my own notes on what clicked, what broke, and what I'd do differently.

---

## 🧭 What these notes cover

### 1. LLMs and knowledge retrieval
How large language models work and how retrieval-augmented generation looks in practice: from a basic keyword/vector search to a full "question → relevant context → answer" pipeline. First experiments with the OpenAI SDK and processing my own data.

- [ ] Basic keyword search built from scratch
- [ ] Vector search and embeddings
- [ ] First working RAG pipeline on real data

### 2. Agents and tools
Moving from a fixed pipeline to a system that decides for itself whether to call a tool and which one. Function calling, agent SDKs (PydanticAI and similar), integrating external tools via MCP.

- [ ] A simple agent with function calling
- [ ] Connecting tools via MCP
- [ ] Mini-project: an agent solving a real task

### 3. Checking response quality
How to tell whether an agent actually got better, not just "looks different." Offline evaluation, LLM-as-a-judge, comparing approaches on objective metrics.

- [ ] A test-case set for my own project
- [ ] LLM-as-a-judge in practice
- [ ] Comparing two pipeline versions by metrics

### 4. Observability and safety in production
What happens to a system after launch: logging, tracing, metrics, and guarding against undesired model behavior.

- [ ] Basic monitoring of requests/responses
- [ ] Guardrails against unwanted responses
- [ ] A dashboard with key metrics

---

## 🛠️ Stack I'm picking up

`Python` · `OpenAI SDK` · `Vector search` · `MCP` · `Evaluation frameworks` · `Observability (Grafana / OpenTelemetry)`

## 📌 Why this repo exists

I keep it to:
1. Reinforce the material by explaining it in my own words
2. Have a public track record of moving toward an AI-Engineer role
3. Build a portfolio of projects I can show in interviews

---

*Updated as I work through the material.*
