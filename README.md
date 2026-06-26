# 📄 RAG Chatbot for PDF Question Answering

A Retrieval-Augmented Generation (RAG) chatbot that enables users to upload one or more PDF documents and ask natural language questions based on their content. The application retrieves the most relevant information from the uploaded documents using semantic search and generates context-aware responses through a Groq-powered Large Language Model (LLM).

The project is deployed on **Hugging Face Spaces** with an interactive **Gradio** interface, making it easily accessible through a web browser.

---

## 🚀 Features

* Upload multiple PDF documents
* Automatic text extraction from uploaded PDFs
* Intelligent document chunking with overlapping segments
* Semantic search using Sentence-Transformer embeddings
* Retrieval-Augmented Generation (RAG)
* Context-aware responses powered by Groq LLM
* Source attribution with PDF name and page number
* Interactive Gradio web interface
* Cloud deployment on Hugging Face Spaces

---

## 🏗️ System Architecture

```text
User
   │
   ▼
Upload PDF(s)
   │
   ▼
Text Extraction
   │
   ▼
Document Chunking
   │
   ▼
Sentence-Transformer Embeddings
   │
   ▼
Vector Similarity Retrieval
   │
   ▼
Relevant Context
   │
   ▼
Groq Large Language Model
   │
   ▼
Generated Answer + Source Reference
```

---

## ⚙️ Technology Stack

| Category             | Technology            |
| -------------------- | --------------------- |
| Programming Language | Python                |
| Frontend             | Gradio                |
| LLM                  | Groq API              |
| Embeddings           | Sentence Transformers |
| NLP Framework        | RAG Pipeline          |
| Deployment           | Hugging Face Spaces   |

---

## 📂 Project Structure

```text
rag_chatbot/
│
├── app.py                 # Main application
├── requirements.txt       # Python dependencies
├── README.md              # Project documentation
├── sample_documents/      # Sample PDFs
└── assets/                # Images and screenshots
```

---

## 🔄 Workflow

1. Upload one or more PDF documents.
2. Extract text from every page.
3. Split the text into semantic chunks.
4. Generate vector embeddings using Sentence Transformers.
5. Retrieve the most relevant chunks using semantic similarity.
6. Send the retrieved context and user query to the Groq LLM.
7. Display the generated response along with source references.

---

## 📌 Key Functionalities

### Document Processing

* Multiple PDF upload support
* Automatic text extraction
* Semantic chunking
* Context preservation using overlapping chunks

### Semantic Retrieval

* Sentence-Transformer embeddings
* Similarity-based document retrieval
* Relevant context selection

### Response Generation

* Context-aware answers
* Natural language interaction
* Source transparency
* Page-level references

---

## 🌟 Enhancements

Compared to a basic PDF chatbot, this project includes:

* Semantic embeddings instead of keyword matching
* Overlapping text chunking for better context retention
* Source citations including document name and page number
* Responsive web interface
* Public cloud deployment

---

## 💻 Installation

Clone the repository

```bash
git clone https://github.com/yourusername/rag-chatbot.git
```

Move into the project

```bash
cd rag-chatbot
```

Install dependencies

```bash
pip install -r requirements.txt
```

Create an environment variable for your Groq API Key.

Run the application

```bash
python app.py
```

---

## 🖥️ Deployment

The application is deployed using **Hugging Face Spaces** with **Gradio**.

Deployment includes:

* Secure API key management using Hugging Face Secrets
* Automatic dependency installation
* Public web access
* Continuous deployment support

---

## 📸 Demo

The application allows users to:

* Upload PDF files
* Ask questions in natural language
* Receive context-aware answers
* View the document source and page reference used for each response

---

## 📜 License

This project is developed for educational and learning purposes.
