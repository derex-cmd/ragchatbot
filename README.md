# 🤖 AI-Powered PDF Question Answering Assistant (RAG-Based)

This project implements a **Retrieval-Augmented Generation (RAG)** pipeline to interactively ask questions about PDF documents using a lightweight LLM and a vector store for semantic search. It supports both **text queries** and **image-based queries** with OCR.

---

## 🧠 Features

- 📄 Parses PDFs and extracts both **text** and **images**
- 🧠 Generates **sentence embeddings** using `all-MiniLM-L6-v2`
- 🗃️ Stores embeddings in **ChromaDB**
- 🔍 Performs **semantic retrieval**
- 🗣️ Uses **DistilGPT-2** for lightweight text generation
- 🖼️ Supports **image upload** with OCR via `pytesseract`
- 🎯 Fully **RAG-based**: combines retrieved context with queries
- 🌐 Interactive **Gradio interface**

---

## 📁 Folder Structure

📦project-root/
├── pdf_preprocessing.ipynb      # Extracts text/images, creates embeddings, stores in Chroma
├── rag_interface.ipynb          # LLM + retrieval interface using Gradio
├── chroma_db/                   # Local vector database (auto-generated)
├── requirements.txt             # Dependencies


## 🛠️ Setup

# 1. Clone the repository
git clone https://github.com/your-repo/pdf-rag-assistant.git
cd pdf-rag-assistant

# 2. Install dependencies
pip install -r requirements.txt

# Or install manually
pip install sentence-transformers chromadb pdfplumber pytesseract gradio transformers

### 🧪 Run the Pipeline
## 1. Preprocess the PDFs

# Open and run the following notebook:
📄 pdf_preprocessing.ipynb
# It will extract data, create embeddings, and store them in ChromaDB

## 📊 Evaluation

- ✅ Cosine similarity for retrieval effectiveness
- ✅ Query response time
- ✅ Manual relevance scoring

## ⚙️ Tech Stack

| Component      | Tool               |
|----------------|--------------------|
| Embeddings     | all-MiniLM-L6-v2   |
| Vector Store   | ChromaDB           |
| OCR            | pytesseract        |
| Interface      | Gradio             |
| LLM            | DistilGPT-2        |
| PDF Parsing    | pdfplumber / PyMuPDF |


## 👥 Contributors

- **Omer Nasir** – [omernasir29@gmail.com](mailto:omernasir29@gmail.com)  
- **Abdul Ahad** – [aadi.25003@gmail.com](mailto:aadi.25003@gmail.com)







