# 🍕 Pizza Project (RAG with LangChain)

An AI-powered tool that allows users to ask natural language questions about restaurant reviews and receive intelligent, context-aware answers.

This project uses a **Retrieval-Augmented Generation (RAG)** pipeline built with LangChain to combine semantic search with a local language model.

---

## 🚀 Features

* 🔍 Ask questions about restaurant reviews in plain English
* 🧠 Semantic search over review data using vector embeddings
* ⚡ Real-time answers powered by a local LLM
* 📊 Processes structured CSV review data
* 🔒 Runs locally using Ollama (no external APIs required)

---

## 🛠 Tech Stack

* **Python**
* **LangChain**
* **Ollama (LLM + Embeddings)**
* **ChromaDB (Vector Database)**
* **Pandas**

---

## ⚙️ How It Works

1. Loads restaurant review data from a CSV file
2. Converts each review into a document
3. Generates embeddings using a local model
4. Stores them in ChromaDB for semantic retrieval
5. User asks a question
6. Relevant reviews are retrieved
7. LLM generates a grounded response based on those reviews

---

## 💡 Example Questions

* “What do customers think about the pizza quality?”
* “Are there complaints about service?”
* “What are the most common positive reviews?”
* “Do people recommend this restaurant?”

---

## ▶️ Running the Project

### 1. Install dependencies

```bash
python -m pip install langchain langchain-ollama langchain-chroma pandas
```

---

### 2. Install and run Ollama

Download from: [https://ollama.com](https://ollama.com)

Then pull required models:

```bash
ollama pull llama3.2
ollama pull mxbai-embed-large
```

---

### 3. Run the application

```bash
python main.py
```

---

## 📂 Project Structure

```
.
├── main.py              # CLI interface + LLM pipeline
├── vector.py            # Embeddings + vector database setup
├── realistic_restaurant_reviews.csv
├── requirements.txt
```

---

## 📌 Notes

* Uses **semantic retrieval**, not exact keyword matching
* Answers are generated only from retrieved reviews
* Designed as a lightweight local AI system for experimentation

---

## 📈 Future Improvements

* Add a web interface (React / Flask)
* Improve ranking and filtering of results
* Support multiple restaurants / datasets
* Add sentiment analysis and summarization

---

## 🧠 What This Project Demonstrates

* Retrieval-Augmented Generation (RAG)
* Vector databases and embeddings
* Prompt engineering with LangChain
* Local LLM integration (privacy-focused AI systems)

---
