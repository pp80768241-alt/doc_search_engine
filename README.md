# 📄 Doc Search Engine

A document search engine that allows users to search through documents using **Natural Language Processing (NLP)** and **semantic similarity**. Instead of relying only on exact keyword matching, the system understands the meaning of the user's query and retrieves the most relevant document content.

## 🚀 Features

* 📂 Upload and process documents
* 🔍 Search documents using natural-language queries
* 🧠 Semantic search using sentence embeddings
* ⚡ Fast similarity search with FAISS
* 📑 Extract text from documents
* 🖼️ OCR support for extracting text from scanned documents
* 🎯 Retrieve the most relevant document sections
* 🐍 Python-based backend

## 🛠️ Tech Stack

* **Python**
* **Flask**
* **Sentence Transformers**
* **FAISS**
* **OCR**
* **NumPy**
* **Pandas**

## 🔄 How It Works

```text
Document
   ↓
Text Extraction / OCR
   ↓
Text Processing
   ↓
Sentence Embeddings
   ↓
FAISS Vector Index
   ↓
User Query
   ↓
Query Embedding
   ↓
Similarity Search
   ↓
Relevant Results
```

## 📌 Project Workflow

1. The user provides a document.
2. Text is extracted from the document.
3. If the document is scanned or image-based, OCR is used to extract the text.
4. The extracted text is divided into searchable sections.
5. Each section is converted into a numerical vector using sentence embeddings.
6. The vectors are stored in a FAISS index.
7. The user enters a natural-language query.
8. The query is converted into an embedding.
9. FAISS searches for the most semantically similar document sections.
10. The most relevant results are returned to the user.

## 🧠 Why Semantic Search?

Traditional keyword search mainly looks for exact words.

For example:

> **Query:** "How can I reset my password?"

A keyword-based system may look specifically for the words *reset* and *password*.

A semantic search system can identify related content such as:

> "Steps to recover access to your account"

even when the exact words in the query are not present.

This makes the search experience more flexible and useful.

## 📁 Project Structure

```text
Doc-Search-Engine/
│
├── app.py
├── requirements.txt
├── README.md
│
├── templates/
│   └── index.html
│
├── static/
│   └── ...
│
└── documents/
    └── ...
```

> Update the structure above if your actual project contains different files or folders.

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone <your-repository-url>
cd Doc-Search-Engine
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

Activate it on Windows:

```bash
.venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the application

```bash
python app.py
```

Open the application in your browser using the local URL shown by Flask.

## 💡 Example

**User Query:**

```text
What are the requirements for applying for a passport?
```

**System:**

```text
Searches the document collection
        ↓
Finds semantically relevant sections
        ↓
Returns the most relevant content
```

## 🎯 Use Cases

The Doc Search Engine can be used for:

* 📚 Searching academic documents
* 📄 Searching company policies
* 📑 Searching reports and manuals
* ⚖️ Searching legal documents
* 🏢 Enterprise document search
* 🔎 Knowledge-base search
* 📖 Research document retrieval

## 🔮 Future Improvements

* Add support for more document formats
* Improve OCR accuracy
* Add document ranking and filtering
* Add conversational question answering
* Integrate Large Language Models (LLMs)
* Add authentication and user-specific document collections
* Deploy the application using cloud services
* Add a modern frontend interface

## 👨‍💻 Author

**Prince Panwar**

B.Tech — Computer Science & Engineering (Data Science)

---

⭐ If you find this project useful, consider giving the repository a star.
