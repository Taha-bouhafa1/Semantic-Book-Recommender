# 📚 Semantic Book Recommender with LLMs

This project is a **semantic book recommendation system** powered by **sentence-transformer embeddings**, **LangChain**, and an interactive **Gradio** UI. It allows users to receive personalized book recommendations based on natural language queries, category filters, and emotional tones extracted from book descriptions.

> Dataset source: [7k Books with Metadata – Kaggle](https://www.kaggle.com/datasets/dylanjcastillo/7k-books-with-metadata)

---

## 🚀 Features

- 🔍 **Semantic Search** — Uses MiniLM sentence embeddings to retrieve books similar to user prompts.
- 🏷️ **Category Filtering** — Classifies books into categories like Fiction, Biography, etc.
- 🎭 **Emotional Sorting** — Ranks books based on emotions (joy, sadness, fear, etc.).
- 🌐 **Gradio UI** — Clean user interface for querying and browsing results visually.

---

## 🧠 Main Components

| File                       | Description                                                       |
|----------------------------|-------------------------------------------------------------------|
| `dashboard_gradio.py`      | Main Python app with Gradio interface and book retrieval logic.  |
| `books_with_emotions.csv`  | Final dataset with cleaned metadata, category, and emotion scores.|
| `tagged_description.txt`   | Preprocessed book descriptions with `isbn13` used for vector DB.  |
| `data-exploration.ipynb`   | Initial data cleaning and preprocessing steps.                    |
| `text_classification.ipynb`| Assigns simple categories using LLM-based classification.         |
| `sentiment_analysis.ipynb` | Uses a transformer model to extract emotion scores per book.      |
| `vector-search (1).ipynb`  | Manual test of vector search using LangChain + Chroma.            |

---

## 🧰 Tech Stack

- `Python 3.11+`
- `sentence-transformers` (MiniLM-L6-v2)
- `langchain-community`, `langchain-chroma`
- `Gradio`
- `Pandas`, `NumPy`
- `dotenv` (optional, not used for OpenAI keys in this project)

---

## 📂 Project Structure

