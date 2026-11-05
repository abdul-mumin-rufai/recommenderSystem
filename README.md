# Recommender Systems: From Foundations to Deep Learning 🚀

Welcome to my comprehensive learning repository on **Recommender Systems**! This repository tracks my journey learning recommendation algorithms from the ground up—covering traditional statistical approaches, matrix factorization, evaluation metrics, and modern deep learning models.

---

## 📌 Table of Contents

- [Overview](#-overview)
- [Project Roadmap & Core Concepts](#-project-roadmap--core-concepts)
  - [1. Foundations & Datasets](#1-foundations--datasets)
  - [2. Evaluation Metrics](#2-evaluation-metrics)
  - [3. Classical Recommendation Algorithms](#3-classical-recommendation-algorithms)
  - [4. Custom Evaluator Architecture](#4-custom-evaluator-architecture)
  - [5. Deep Learning & Advanced Models](#5-deep-learning--advanced-models)
- [Tech Stack & Libraries](#-tech-stack--libraries)
- [Getting Started](#-getting-started)
- [Repository Structure](#-repository-structure)
- [Future Goals](#-future-goals)

---

## 🎯 Overview

Recommender Systems power modern digital platforms by personalizing content, products, and media. The goal of this repository is to systematically build, evaluate, and benchmark different recommendation strategies using real-world data like the **MovieLens** dataset.

---

## 🛣️ Project Roadmap & Core Concepts

### 1. Foundations & Datasets
- **Introduction to Recommender Systems:** Explored explicit vs. implicit feedback, cold-start problems, and recommendation pipelines.
- **MovieLens Dataset:** Worked with MovieLens (100k / 1M) datasets for benchmark testing.
- **Surprise Library (`scikit-surprise`):** Used Python’s Surprise library for quick prototyping of memory-based and model-based algorithms.

### 2. Evaluation Metrics
Understanding accuracy and ranking metrics to measure recommendation performance:
- **Error Metrics:** 
  - Mean Absolute Error (**MAE**)
  - Root Mean Squared Error (**RMSE**)
- **Ranking & Diversity Metrics:**
  - Precision@K & Recall@K
  - Mean Average Precision (**MAP**)
  - Normalized Discounted Cumulative Gain (**NDCG**)
  - Novelty, Coverage, and Diversity metrics.

### 3. Classical Recommendation Algorithms
- **Content-Based Filtering:** Built recommendations based on item features and metadata (using TF-IDF, Cosine Similarity).
- **Collaborative Filtering:**
  - **User-Based:** Recommending items liked by similar users.
  - **Item-Based:** Recommending items similar to those a user liked in the past.
- **Matrix Factorization:**
  - Singular Value Decomposition (**SVD** / SVD++)
  - Non-Negative Matrix Factorization (**NMF**)

### 4. Custom Evaluator Architecture
- Implemented a reusable **`Evaluator` class** to systematically compare multiple algorithms side-by-side across various evaluation metrics (cross-validation, train-test splits, leave-one-out cross-validation).

### 5. Deep Learning & Advanced Models
- **Neural Networks for Recommendations:** Applying deep architectures to capture complex non-linear user-item interactions.
- **Restricted Boltzmann Machines (RBM):** Generative neural network models for collaborative filtering.
- **TensorFlow Recommenders (TFRS):** Building scalable, production-ready multi-task deep learning recommenders using TensorFlow.

---

## 🛠️ Tech Stack & Libraries

- **Language:** Python 3.10+
- **Data & Math:** `numpy`, `pandas`, `scipy`
- **Machine Learning & Recommenders:** `scikit-learn`, `scikit-surprise`
- **Deep Learning Frameworks:** `tensorflow`, `tensorflow-recommenders (TFRS)`
- **Visualization:** `matplotlib`, `seaborn`

---

## 💻 Getting Started

### Prerequisites
Make sure you have Python 3.10+ installed on your system.

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/abdul-mumin-rufai/recommenderSystem
   ```

2. **Create a virtual environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

---

## 📁 Repository Structure

```text
├── recommenderSystem/                  # Interactive Spyder project
│   ├── 01_Evaluating
│   ├── 02_Framework                    
│   ├── evaluator.py            
│   ├── ml-latest-small
│   └──
└── README.md                   # Repository documentation
```

---

## 🚀 Future Goals

- [ ] Integrate Real-Time Inference using **FastAPI** to serve recommendations via API.
- [ ] Implement Graph Neural Networks (GNNs) for recommendation networks.
- [ ] Explore Context-Aware Recommenders (incorporating time, location, and device metadata).

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more details.