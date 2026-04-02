# 🎬 GenAI Movie Recommendation System

> A Netflix-style intelligent movie recommendation system powered by **Machine Learning + Generative AI** — featuring embeddings, semantic search, and vector databases.

This project demonstrates how modern recommendation systems evolve into **LLM-powered personalized assistants**.

---

## 🚀 Features

- 🎯 Content-based movie recommendation
- 🧠 Semantic search using embeddings
- ⚡ Fast similarity search with FAISS (vector database)
- 🤖 LLM-powered recommendations (GenAI enhancement)
- 💬 Chat-based movie suggestion system
- 🌐 API + Interactive UI

---

## 🧱 System Architecture

```
Dataset → Preprocessing → Embeddings → FAISS Vector DB
                                              ↓
User Query → Embedding → Similarity Search → Recommendations
                                              ↓
                                    LLM Enhancement
```

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Language | Python |
| ML Libraries | scikit-learn, pandas, numpy |
| Embeddings | Sentence Transformers / OpenAI |
| Vector DB | FAISS |
| Backend | FastAPI |
| Frontend | Streamlit |
| LLM (optional) | OpenAI API |

---

## 📂 Project Structure

```
movie-recommender-genai/
│
├── data/                   # Dataset files
├── notebooks/              # EDA & experiments
├── src/                    # Core logic
│   ├── preprocessing.py
│   ├── embeddings.py
│   ├── recommender.py
│   ├── faiss_index.py
│   └── llm_module.py
│
├── app/                    # Application layer
│   ├── main.py             # FastAPI backend
│   └── ui.py               # Streamlit frontend
│
├── requirements.txt
└── README.md
```

---

## 📊 Dataset

Uses **MovieLens / TMDB** dataset containing:
- Movie title
- Genres
- Overview / description

---

## ⚙️ Installation

```bash
git clone https://github.com/your-username/movie-recommender-genai.git
cd movie-recommender-genai

pip install -r requirements.txt
```

---

## ▶️ Usage

### 1. Run Backend (FastAPI)

```bash
uvicorn app.main:app --reload
```

### 2. Run Frontend (Streamlit)

```bash
streamlit run app/ui.py
```

---

## 🧠 How It Works

### 1. Content-Based Filtering
- Combines movie genres + descriptions
- Uses cosine similarity for matching

### 2. Embedding-Based Search *(GenAI Core)*
- Converts movies into dense semantic vectors
- Captures meaning beyond keyword matching

### 3. Vector Search with FAISS
- Fast nearest-neighbor search
- Enables scalable, real-time recommendations

### 4. LLM Enhancement
- Generates human-like recommendation responses
- Explains *why* a movie is recommended

---

## 💡 Example Queries

```
"Recommend movies like Inception"
"Suggest emotional sci-fi movies"
"Give me thriller movies with plot twists"
```

---

## 📈 Evaluation Metrics

- Precision@K
- Recall@K
- Cosine Similarity Scores

---

## 🔥 Future Improvements

- [ ] Hybrid recommendation (collaborative + content-based)
- [ ] Real-time user personalization
- [ ] Cloud deployment (AWS / GCP)
- [ ] Integration with user watch history
- [ ] Advanced RAG pipeline

---

## 🎯 Key Learnings

- Recommendation system design
- Embeddings & semantic search
- Vector databases (FAISS)
- LLM integration in ML systems
- End-to-end ML system building

---

## 🤝 Contributing

Contributions are welcome! Feel free to open issues or submit pull requests.

---

## 📜 License

This project is open-source and available under the [MIT License](LICENSE).

---

⭐ **If you found this useful, give it a star!**
