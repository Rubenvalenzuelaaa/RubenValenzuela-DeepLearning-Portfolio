# 🤖 Final Course Project — AI Agent Creation  
**Course:** ITAI 2376 – Deep Learning Artificial Intelligence  
**Student:** Ruben Valenzuela  
**Team:** AI Alchemists  

This repository contains my **Final Course Project**, where I designed and implemented a fully functioning **AI Research Assistant Agent** capable of retrieving information, performing web search, scraping sources, generating embeddings, storing vectors, performing semantic search, summarizing content, and interacting using a ReAct-style reasoning loop.

The system also includes safety layers, memory, and a lightweight reinforcement feedback mechanism.

---

## 📌 Project Summary

The Final Project required building an AI Agent with:

### ✔️ **Retrieval-Augmented Generation (RAG)**  
- Custom embedding model (`all-MiniLM-L6-v2`)  
- Vector storage using **ChromaDB**  
- Semantic similarity search  
- Context retrieval for answering complex questions  

### ✔️ **Tools & Actions Layer**  
The agent uses three custom tools:

1. **Web Search Tool (DuckDuckGo API)**  
2. **Web Scraper Tool** (extracts & cleans text from URLs)  
3. **Vector Database Query Tool** for semantic retrieval  

### ✔️ **ReAct Agent Loop**  
Implements:  
**Thought → Action → Observation → Final Response**

With transparent logs that allow the user to follow the reasoning chain.

### ✔️ **Summarization Engine**  
- Multi-step summarization  
- Topic extraction  
- Key insights aggregation  

### ✔️ **Safety Filter**  
Prevents the system from producing:  
- Illegal advice  
- Harmful content  
- Private data extraction  
- Disallowed academic output  

### ✔️ **Reinforcement Feedback Mechanism**  
The user scores the agent (1–5).  
The system updates internal weighting and improves future summaries.

---


---

---

## 🧠 Key Technologies Used

- Python  
- Transformers / SentenceTransformers  
- ChromaDB  
- DuckDuckGo Search  
- BeautifulSoup4  
- ReAct Reasoning  
- Summarization Models  
- Reinforcement Learning (lightweight loop)  

---

## 📄 Documentation

All formal project submissions are included:

- **Finalproject_2376.pdf** — formatted project PDF  
- **FINALPROJECT_ITAI2376.docx** — editable version  
- **Finalproject_2376.ipynb** — full code & logs  

---

## 💬 Author  
**Ruben Valenzuela**  
_AI Alchemists Team_  
ITAI 2376 – Fall Semester


