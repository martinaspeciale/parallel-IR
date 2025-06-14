# ParallelIR

**ParallelIR** is an academic project developed as part of a course on Multimedia Information Retrieval. It implements a full Information Retrieval system from scratch, with a focus on **parallelism, ranking models, and performance evaluation**.

## 📌 Features

- **Parallel Inverted Index Construction**  
  Efficient document indexing using parallelized data structures and multiprocessing techniques.

- **Parallel Query Processing**  
  Fast retrieval enabled by concurrent query execution and optimized memory access.

- **Ranking with TF-IDF and BM25**  
  Evaluation and comparison of classical scoring functions on benchmark datasets.

- **Caching Mechanisms**  
  Implementation and testing of various caching strategies to enhance response time.

- **Relevance Feedback**  
  Rocchio-style feedback algorithm to refine query results based on user preferences.


## 📚 Dataset

This project uses the **ANTIQUE** dataset, a large-scale benchmark for ad-hoc information retrieval with natural language queries.

- **Dataset name**: `antique/test`
- **Source**: [`ir_datasets`](https://ir-datasets.com/antique.html)
- **Documents**: ~403,666
- **Queries**: Natural-language, open-ended
- **Relevance Judgments**: Binary qrels for a subset of queries
- **Use case**: Evaluating classic retrieval models (TF-IDF, BM25) in a realistic, large-scale IR setting

The dataset is automatically downloaded and handled via the `ir_datasets` Python package.


## 🚀 Technologies

- `python-terrier`, `ir_datasets`, `ir_measures`
- `nltk`, `pandas`, `scikit-learn`, `tqdm`
- Designed and tested in the Kaggle notebook environment.


## ⚙️ Setup

To run this project locally, it is recommended to use a Python virtual environment.

```bash
# 1. Clone the repository
git clone https://github.com/martinaspeciale/parallel-IR.git
cd parallel-IR

# 2. Create and activate a virtual environment
python3 -m venv .venv
source .venv/bin/activate  

# 3. Install all required dependencies
pip install -r requirements.txt

# 4. (Optional) Register Jupyter kernel for the notebook
python -m ipykernel install --user --name=parallelIR --display-name "Python (parallelIR)"


## 👥 Authors

Filippo Lucchesi, Francesco Pio Crispino, Martina Speciale
