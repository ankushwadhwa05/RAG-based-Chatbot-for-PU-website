#  Panjab University Admissions AI Chatbot (RAG)

### Overview
This project presents a **Retrieval-Augmented Generation (RAG)** chatbot designed to streamline the admission process for Panjab University (PU). By bridging the gap between static documents and dynamic student queries, this AI assistant helps prospective students and faculty access accurate information from over **50+ official PDF handbooks** and web notices instantly.

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=Streamlit&logoColor=white)
![LLaMA](https://img.shields.io/badge/Model-LLaMA_3.2-0467DF?style=for-the-badge&logo=meta&logoColor=white)
![Nomic](https://img.shields.io/badge/Embeddings-Nomic-green?style=for-the-badge)

---

### Interface Preview
([<img width="900" height="400" alt="Screenshot 2026-02-10 193432" src="https://github.com/user-attachments/assets/2b3e94de-0a6d-47f8-b12c-088db68e1105" />](https://github.com/ankushwadhwa05/Func/blob/main/Screenshot%202026-02-10%20193432.png?raw=true)
)

> *The Streamlit interface providing real-time, context-aware answers to admission queries.*

---

###  How It Works (The Architecture)
The system moves beyond simple keyword search by using **semantic search** to understand the *meaning* behind a student's question.

1.  **Data Ingestion:**
    * Scraped data from the official PU admissions portal.
    * Extracted text from **50+ official PDF handbooks**, notices, and regulations.
2.  **Preprocessing & Embedding:**
    * **Chunking:** Split long documents into manageable text chunks to optimize retrieval.
    * **Embeddings:** utilized **Nomic Embeddings** to convert text into high-dimensional vectors.
3.  **Retrieval System:**
    * When a user asks a question, the system performs a semantic similarity search to find the most relevant "chunks" of text from the knowledge base.
4.  **Generation (LLM):**
    * The retrieved context is passed to **LLaMA 3.2:3B** (running locally).
    * The LLM generates a natural language response grounded strictly in the university's official data.

---

### Tech Stack
* **Language:** Python
* **Frontend:** Streamlit (for the chat interface)
* **LLM:** LLaMA 3.2:3B (Local Inference)
* **Embeddings:** Nomic AI
* **Vector Operations:** Semantic Similarity Search
* **Data Sources:** PDF Processing & Web Scraping

---

### Key Features
* **Context-Aware:** Remembers conversation history for multi-turn queries.
* **Privacy-Focused:** Runs on a local LLM (LLaMA 3.2), ensuring data privacy and reducing API costs.
* **Source Grounding:** Answers are based on actual extracted documents, reducing hallucinations common in generic AI models.
* **Scalability:** The pipeline allows for easy addition of new academic years' handbooks without retraining the model.

---

### Impact
* **Accessibility:** significantly reduces the time students spend searching through complex admission handbooks.
* **Efficiency:** Reduces the administrative workload on university staff by automating repetitive queries.

---

### Connect with Me
<a href="https://www.linkedin.com/in/ankush-wadhwa-038315293/">
  <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
</a>
