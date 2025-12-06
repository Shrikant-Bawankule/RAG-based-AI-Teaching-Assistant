# 🎓 RAG-based AI Teaching Assistant  
A GenAI-powered learning assistant that transcribes, indexes, and retrieves lecture content using Whisper ASR + Embeddings + LLMs.

---

## 🚀 Project Overview
This project transforms long lecture videos into an interactive AI assistant capable of:
- Transcribing content into structured text (with timestamps)
- Searching concepts via semantic retrieval (not keyword-based)
- Providing accurate, contextual responses powered by LLMs
- Allowing learners to jump directly to exact lecture moments

Designed to improve student learning by enabling fast discovery of relevant information.

---

## 🧠 Key Features
✔ Automatic speech-to-text using **Whisper**  
✔ Context-aware answer generation using **RAG Pipeline**  
✔ Semantic search using **Embeddings + Vector Similarity**  
✔ Timestamp navigation for transparent learning  
✔ Clean UI for query interaction  
✔ Scalable for any educational content  

---

## 🏗️ System Architecture

```mermaid
flowchart TD
A[Video Input] --> B[Whisper Transcription]
B --> C[Chunk + Metadata Assignment]
C --> D[Embedding Generation]
D --> E[Vector Store Search]
E --> F[LLM Contextual Response Generation]
F --> UI[User Interface]
🛠️ Tech Stack
Category	Tools
ASR	OpenAI Whisper
LLM + RAG	LangChain / Llama-based / GPT-based
Vector Search	FAISS or ChromaDB
Interface	Streamlit
Dev Tools	Python, Pandas, NumPy, Joblib
Cloud Execution	Google Colab

📊 Workflow Steps
1️⃣ Extract Audio from lecture videos
2️⃣ Whisper Model → generate text + timestamps
3️⃣ Chunk + Metadata Storage
4️⃣ Embeddings Generation for semantic matching
5️⃣ Top-k Retriever to fetch relevant lecture segments
6️⃣ LLM Generates Final Response with citations

📈 Example Use Cases
🎯 Ask: "What is Precision and Recall?"
🤖 AI responds with summary + timestamp to jump right into video
📌 Improves revision speed and content accessibility


📂 Folder Structure
bash
Copy code
├── data/                     # raw & processed transcripts
├── embeddings/               # vector DB storage
├── notebooks/                # experimentation notebooks
├── app/streamlit_app.py      # final deployed interface
├── utils/                    # helper modules
└── README.md
💡 Future Improvements
🔹 Multi-video indexing
🔹 User profile-based personalization
🔹 MCQs and quiz generation
🔹 GPU-based inference for faster search
🔹 Dashboard for lecture progress analytics

🙌 Contributors
👤 Shrikant Bawankule
