# 🧠 Enterprise-RAG-Engine: Multi-Model Knowledge Platform

![Python](https://img.shields.io/badge/Python-3.9+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-Integration-1C3C3C?style=for-the-badge)
![OpenAI](https://img.shields.io/badge/OpenAI-GPT_4-412991?style=for-the-badge&logo=openai&logoColor=white)
![Gemini](https://img.shields.io/badge/Google-Gemini_Pro-4285F4?style=for-the-badge&logo=google&logoColor=white)
![ChromaDB](https://img.shields.io/badge/Vector_DB-Chroma-FF6C37?style=for-the-badge)

> *A scalable Retrieval-Augmented Generation (RAG) architecture engineered to parse, embed, and retrieve data from diverse, unstructured sources using state-of-the-art LLMs.*

---

## 🎯 Engineering Context (Targeting AI Platforms)
I architected this project to master the core components of **Enterprise AI Platforms**. Relying purely on static LLM weights leads to hallucinations and outdated responses. This engine dynamically grounds LLM generations (OpenAI, Gemini, Mistral) in external, proprietary data using highly optimized vector search semantics.

---

## ⚙️ Core Architecture & Tech Stack

**1. Data Ingestion & Chunking**
* **Supported Formats:** PDF, DOCX, CSV, TXT.
* **Processing:** Utilizes LangChain document loaders and recursive character text splitters to optimize token windows and maintain semantic context during vectorization.

**2. Embedding & Vector Store (ChromaDB)**
* Converts raw text chunks into high-dimensional vectors.
* Employs **ChromaDB** for rapid nearest-neighbor similarity search, instantly retrieving the most relevant context blocks when queried.

**3. Multi-LLM Routing Layer**
* Configured to dynamically route prompts across multiple foundation models:
  * **OpenAI (GPT-3.5 / GPT-4)** for complex reasoning.
  * **Google Generative AI (Gemini Pro)** for rapid, multi-modal task execution.
  * **Hugging Face (Mistral-7B)** for open-source deployment testing.

**4. Interactive Application UI**
* Built a streamlined user interface utilizing **Streamlit** to handle session state, manage API key authentication, and render real-time conversational history.

---

## 🚀 System Data Flow Diagram

*The visual representation below outlines the orchestration between the document loader, vector embedding space, and the conversational retrieval chain.*

<p align="center">
  <img width="800" src="https://raw.githubusercontent.com/sahilistrying/Enterprise-RAG-Engine/main/images/rag-architecture.png" alt="RAG Architecture">
</p>

---

## 🛠️ Local Execution Protocol

```bash
# 1. Initialize Virtual Environment
python -m venv ai_env
source ai_env/bin/activate  # On Windows: .\ai_env\Scripts\activate

# 2. Install Dependencies
pip install -r requirements.txt

# 3. Launch Streamlit UI
streamlit run RAG_app.py
```

---
<p align="center"><i>Engineered for robust AI Knowledge Retrieval.</i></p>
 
 
