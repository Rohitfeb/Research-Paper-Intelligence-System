# 📚 Research Paper Intelligence System (Agentic AI Based)

An AI-powered Research Paper Intelligence System that enables semantic search, paper comparison, keyword extraction, and intelligent question answering using Large Language Models (LLMs), Sentence Transformers, FAISS, and LangChain.



## 📌 Project Overview

Researchers often spend significant time searching for relevant literature and comparing research papers manually. This project automates these tasks by combining semantic embeddings, vector search, and generative AI.

The system converts research papers into vector embeddings, stores them in a FAISS vector database, and retrieves the most relevant papers based on user queries. It also compares research papers, extracts keywords, and generates AI-powered responses.



## 🚀 Features

- 📄 Research Paper Processing
- 🔍 Semantic Search using Sentence Transformers
- ⚡ Fast Vector Search using FAISS
- 🤖 AI-powered Question Answering using Gemini
- 📊 Research Paper Comparison
- 🏷️ Keyword Extraction
- 🧠 LangChain Integration
- 📚 Embedding-based Information Retrieval
- 💬 Prompt Engineering Examples



## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Sentence Transformers
- FAISS
- LangChain
- Google Gemini API
- Scikit-learn
- Hugging Face Transformers
- Jupyter Notebook



## 📂 Project Structure

```text
CBSOT-PROJECT-3/
│
├── 📓 Research_Paper_Intelligence_System.ipynb
│   └── Complete Jupyter Notebook containing data loading,
│       preprocessing, semantic search, FAISS indexing,
│       keyword extraction, research paper comparison,
│       and LLM-powered question answering.
│
├── 📄 README.md
│   └── Project documentation, setup instructions,
│       features, and usage guide.
│
├── 📦 requirements.txt
│   └── List of all Python libraries required
│       to run the project.
│
├── 🚫 .gitignore
│   └── Specifies files and folders that Git
│       should ignore (cache, virtual environments,
│       secrets, etc.).
│
└── 📜 LICENSE
    └── MIT License describing the permissions
        for using and distributing this project.
```

## 📂 Dataset

This project uses the **ML-ArXiv-Papers** dataset available on Hugging Face. The dataset contains machine learning research papers with titles, abstracts, and related metadata, making it suitable for semantic search, document comparison, keyword extraction, and question answering tasks.

**Dataset Source:**  
https://huggingface.co/datasets/CShorten/ML-ArXiv-Papers

### Dataset Loading

The dataset is downloaded automatically when the notebook is executed using the Hugging Face `datasets` library.

```python
from datasets import load_dataset

dataset = load_dataset(
    "CShorten/ML-ArXiv-Papers",
    split="train"
)
```

### Dataset Features

- 📄 Research paper titles
- 📝 Abstracts
- 🏷 Metadata and paper information
- 🤖 Ready for semantic search and NLP applications

> **Note:** The dataset is **not included** in this repository because it is automatically downloaded from Hugging Face during execution.


## 🔑 API Key Setup

This project uses the **Groq API** to power the Large Language Model (LLM).

### Get a Groq API Key

1. Visit https://console.groq.com/
2. Sign in or create an account.
3. Generate a new API key.

### Configure in Google Colab

1. Open the **Secrets** panel (🔑 icon).
2. Create a new secret.

Name:

```
GROQ_API_KEY
```

Value:

```
Paste your Groq API key here
```

3. Enable **Notebook access**.

The notebook automatically loads the API key using:

```python
from google.colab import userdata

api_key = userdata.get("GROQ_API_KEY")
```



## ⚙️ Installation

Clone the repository

```bash
git clone https://github.com/your-username/Research-Paper-Intelligence-System.git
```

Move into the project directory

```bash
cd Research-Paper-Intelligence-System
```

Install dependencies

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook

```bash
jupyter notebook
```

Open

```
Research_Paper_Intelligence_System.ipynb
```


## 📊 Workflow

```
Research Papers
       │
       ▼
Data Preprocessing
       │
       ▼
Sentence Transformer
       │
       ▼
Vector Embeddings
       │
       ▼
FAISS Vector Database
       │
       ▼
Semantic Search
       │
       ▼
LangChain
       │
       ▼
Google Gemini
       │
       ▼
AI Generated Response
```


## 📈 Functionalities

### 1. Data Loading

Loads and preprocesses research paper datasets.


### 2. Embedding Generation

Converts research papers into dense semantic embeddings using Sentence Transformers.


### 3. Vector Database

Stores embeddings efficiently using FAISS for fast similarity search.


### 4. Semantic Search

Retrieves research papers based on semantic similarity rather than exact keyword matching.


### 5. Research Paper Comparison

Compares multiple research papers based on their content and identifies similarities and differences.


### 6. Keyword Extraction

Extracts important keywords from research papers for quick understanding.


### 7. AI Question Answering

Uses Google Gemini through LangChain to answer research-related questions using retrieved papers.


## 📷 Sample Outputs

- Semantic Search Results
- Similar Research Papers
- Keyword Extraction
- AI Generated Answers
- Research Paper Comparison


## 📌 Applications

- Academic Research
- Literature Review
- Research Assistance
- Knowledge Discovery
- Educational Applications
- AI-powered Search Systems


## 🔮 Future Improvements

- PDF Upload Support
- Streamlit Web Application
- Citation Generation
- Research Paper Summarization
- Multi-document Question Answering
- Hybrid Search (Keyword + Semantic)
- Cloud Deployment


## 👨‍💻 Author

Rohit Kumar Thakur

Machine Learning & Data Science Enthusiast
