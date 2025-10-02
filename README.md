# AI-Powered Document Search Engine  

An intelligent document search system that uses **Natural Language Processing (NLP)** and **semantic embeddings** to allow users to search large collections of documents using natural language queries. Unlike keyword-based search, this system understands **context and meaning** to return more relevant results.  

---

## 🚀 Features
- Semantic search using vector embeddings (Sentence-BERT / Transformers).  
- Supports ingestion of PDF, TXT, and DOCX files.  
- REST API for uploading documents and querying.  
- React-based UI for interactive search.  
- Scalable architecture with Docker + PostgreSQL + FAISS/Elasticsearch.  

---

## 🛠️ Technologies Used
- **Backend:** Python, FastAPI  
- **NLP & ML:** HuggingFace Transformers, Sentence-BERT, scikit-learn  
- **Database / Search Index:** PostgreSQL, FAISS, Elasticsearch  
- **Frontend:** React.js, TailwindCSS  
- **Containerization:** Docker, Docker Compose  
- **Cloud (Optional):** Google Cloud / AWS (S3, Pub/Sub, Lambda)  

---

## ⚙️ Installation

### 1. Clone the Repository
```bash
git clone https://github.com/AmishNavadia/AI-Powered-Document-Search-Engine.git
cd AI-Powered-Document-Search-Engine
```
### 2. Backend Setup
```bash
cd backend
python -m venv venv

# Activate environment
# On Linux/Mac:
source venv/bin/activate
# On Windows:
venv\Scripts\activate
pip install -r requirements.txt
```
### 3. Frontend Setup
```bash
Copy code
cd frontend
npm install
npm start
```
### 4. Run with Docker (Alternative)
```bash
Copy code
docker-compose up --build
```
📊 Usage
Upload documents via the web interface or API.

Enter a natural language query (example: "What are the challenges in distributed systems?").

Receive semantically ranked results.
