# 🧠 Cognitive Research Agent with Persistent Memory

## 📌 Project Description 
This project implements a **Cognitive AI Research Agent** that goes beyond a traditional chatbot by incorporating **persistent memory** and **decision-aware reasoning**. The agent is designed to assist users in long-term research workflows by remembering their preferences, past questions, and historical decisions, and then using that memory to influence future responses.

Unlike stateless chatbots, this agent maintains both **short-term conversational context** and **long-term semantic memory** stored in a vector database. The system is built using modern LangChain (LCEL), a local LLM served via Ollama, and a vector database for scalable memory retrieval.

---

## 🎯 Problem Statement

Most LLM-based chatbots are **stateless**:

* They forget user preferences
* They do not remember past decisions
* Each interaction is treated as isolated

This limits their usefulness in research, learning, and decision-making tasks that naturally span multiple sessions.

---

## 💡 Solution Overview

This project introduces a **Cognitive Research Agent** that:

* Stores long-term user memory using embeddings
* Retrieves relevant memory semantically
* Injects memory dynamically into the LLM prompt
* Adapts its reasoning based on past user decisions

---

## 🧠 What Does “Cognitive” Mean Here?

The agent does not just answer questions.
It **reasons with memory**:

* If the user prefers deep technical explanations → future answers become more technical
* If the user rejected beginner resources → future recommendations avoid them
* If the user focuses on a specific research domain → answers stay aligned with it

This mimics a basic form of human-like learning and adaptation.

---

## 🏗️ System Architecture

User Input
↓
Memory Retrieval (Vector DB)
↓
Prompt Construction (with memory context)
↓
LLM Reasoning (Ollama – Llama 3)
↓
Final Response

---

## 🧰 Tech Stack

* **Language:** Python
* **LLM:** Llama 3 (via Ollama)
* **Framework:** LangChain (LCEL)
* **Vector DB:** ChromaDB
* **Embeddings:** Sentence Transformers
* **Environment:** Google Colab

---

## 🚀 Future Improvements

* Automatic decision extraction using LLM classification
* LangGraph state machine for multi-step reasoning
* CrewAI multi-agent research collaboration
* Memory evaluation and retrieval accuracy metrics

---

### Cognitive Research Agent with Persistent Memory

A decision-aware AI research assistant that maintains long-term memory using vector embeddings and adapts its reasoning based on user preferences and historical decisions.

**Key Features:**

* Persistent semantic memory (vector DB)
* Decision-aware reasoning
* Local LLM inference with Ollama
* Modern LangChain (LCEL) architecture

**Use Cases:**

* Long-term research assistance
* Personalized learning agents
* Decision-support systems
