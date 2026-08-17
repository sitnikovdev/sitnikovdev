---
Created: 2026-08-15
Updated: 2026-08-17
---

# From Code to Meaning: A Developer's Guide to LLMs

## Introduction

- [What changed: development before and after LLMs](books/Intro-1.md)
- [A contested but important question: does this mean programming as a skill is dying?](books/intro-2.md)
- [What it means to be a developer now](books/intro-3.md)
- [Why this book exists and who it's for](books/intro-4.md)

## Part I. How the Machine Sees and Understands Text

**Chapter 1. The Developer in the Age of AI**

- 1.1 The developer-as-executor vs. the developer-as-solution-architect
- 1.2 What AI can do instead of you — and what it can't
- 1.3 The new skill set: what actually matters now

**Chapter 2. Knowledge Without Knowledge**

- 2.1 How a human "knows" things
- 2.2 What if knowledge is patterns in language, not facts?
- 2.3 The magic of predicting the next word
- 2.4 Why this even works: scale of data as fuel
- 2.5 What we learned

**Chapter 3. How the Machine Sees Text: Tokens and Vocabulary**

- 3.1 The problem: letters aren't what a neural network works with
- 3.2 The naive idea, and why it doesn't work
- 3.3 How text is actually cut up: from letters to words through merging
- 3.4 A token is a number, but the number means nothing by itself
- 3.5 Hands-on: a naive BPE tokenizer in Swift
- 3.6 What we learned

**Chapter 4. Vectors and Embeddings: Meaning as Geometry**

- 4.1 A token isn't meaning yet — it's just a label
- 4.2 What if we stored every word as a point in space?
- 4.3 A space of meaning, by example: flower, tree, garden
- 4.4 Chaos at the start: what vectors mean before training
- 4.5 Training as rearranging the furniture
- 4.6 How to measure the "closeness" of two meanings
- 4.7 The same token, a different vector
- 4.8 What this gives the model in practice
- 4.9 What we learned

**Chapter 5. How Transformers Work**

- [5.1 The problem: sequential memory and its limits (RNNs/LSTMs)](books/5.1.md)
- [5.2 The turning point: dropping sequence ("Attention Is All You Need," 2017)](books/5.2.md)
- [5.3 Why this became physically possible: parallel computation instead of step-by-step](books/5.3.md)
- [5.4 Three projections of one token: Q, K, V](books/5.4.md)
- 5.5 How a token compares itself to everyone: from similarity to weights _(softmax — not yet covered)_
- [5.6 A token's new representation: a weighted sum of V](books/5.6.md)
- [5.7 One head isn't enough: multi-head attention](books/5.7.md)
- [5.8 What we learned](books/5.8.md)

## Part II. Search and Knowledge

**Chapter 6. When the Words Don't Match, but the Meaning Does**

- 6.1 The problem: how to search among thousands of documents
- 6.2 The idea: pull keywords out of the query
- 6.3 The inverted index: how it works under the hood
- 6.4 Finding isn't enough — you need ranking
- 6.5 The wall: where lexicon ends and meaning begins
- 6.6 What we learned

**Chapter 7. Searching by Meaning**

- 7.1 Back to embeddings — now applied to search
- 7.2 Documents become points in the space of meaning too
- 7.3 The query is a vector too
- 7.4 Finding the nearest neighbors
- 7.5 Hybrid: keyword + semantic search together
- 7.6 What we learned

**Chapter 8. From a Retrieved Chunk of Text to a Model's Answer**

- 8.1 What "RAG" actually means, step by step
- 8.2 How documents get split into chunks, and why that's its own problem
- 8.3 Assembling context for the model
- 8.4 A first experiment on my own data
- 8.5 What we learned

## Part III. Agents and Tools _(in progress)_

Chapter 9. What Is an AI Agent

- 9.1 The problem: a chatbot answers, but doesn't act
- 9.2 What changes when the model can decide what to do next on its own
- 9.3 The ReAct loop: reason → act → observe the result
- 9.4 The fork: satisfied with the result — answer the user; not satisfied — the loop repeats
- 9.5 What fundamentally sets an agent apart from a scripted bot
- 9.6 What we learned

Chapter 10. A Simple Agent with Function Calling (in progress)

Chapter 11. Connecting Tools via MCP (in progress)

Chapter 12. Mini-Project: An Agent Solving a Real Task (in progress)

## Part IV. Checking Quality _(in progress)_

- A test-case set for my own project
- LLM-as-a-judge in practice
- Comparing two pipeline versions by metrics

## Part V. Production _(in progress)_

- Basic monitoring of requests/responses
- Guardrails against unwanted responses
- A dashboard with key metrics

---

_The introduction and Chapters 1–8 are broken down into sections based on my own understanding of the material. Parts III–V are still at the high-level plan stage — they'll be fleshed out as I work through those topics._ _Actual prose written so far: 1.2, 4.1, 4.2. Everything else is structure only, awaiting text. Chapter 5 is still missing an explanation of softmax (5.5) — needs to be closed before writing the chapter's prose._

