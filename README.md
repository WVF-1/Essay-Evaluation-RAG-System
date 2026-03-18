# Essay-Evaluation-RAG-System
Retrieval Augmented Generating (RAG) system for evaluating and grading student essays, with the main purpose of helping students understand their scores and improve their writing.

# 📚 Essay Evaluation RAG System

A data-driven, retrieval-based system for evaluating student essays using feature engineering and Retrieval-Augmented Generation (RAG) principles.

---

## 🧠 Overview

This project builds an **end-to-end essay evaluation system** that mimics how human graders compare writing by leveraging similar examples.

Rather than relying on a black-box language model, this system:

* Retrieves similar essays from a dataset
* Compares structural and linguistic features
* Generates feedback grounded in real examples
* Evaluates performance using RAG-specific diagnostics

---

## 🎯 Key Features

### ✍️ Essay Evaluation

* Predicts essay scores using similar retrieved examples
* Provides structured, human-readable feedback
* Supports multiple modes:

  * Feedback generation
  * Score explanation
  * Improvement suggestions
  * Score prediction

---

### 🔍 Retrieval-Augmented System (RAG)

* Hybrid retrieval using:

  * Semantic similarity
  * Feature-based similarity (length, vocabulary richness)
* Weighted scoring system (60/40 blend)

---

### 📊 Evaluation Framework (Notebook 4)

A dedicated evaluation pipeline analyzing:

* **Top-K Consistency** → stability of retrieved scores
* **Score Alignment** → predicted vs actual scores
* **Context Relevance** → similarity of retrieved essays
* **Groundedness (Proxy)** → feature alignment with retrieved context
* **Retrieval Diversity** → variation in retrieved examples

---

### 🎨 Visualization & Design

* Custom “classroom-style” theme:

  * Cream backgrounds
  * Gold, red, and brown accents
  * Serif fonts for an academic feel

---

## 🗂️ Project Structure

```
├── Notebook 1: Feature Engineering
├── Notebook 2: Retrieval System
├── Notebook 3: Feedback Generation + Styling
├── Notebook 4: Evaluation & Diagnostics
├── data/
│   └── ASAP2_train_sourcetexts.csv
└── README.md
```

---

## ⚙️ How It Works

### 1. Feature Engineering

Extracts key essay characteristics:

* Length
* Vocabulary richness
* Additional structural signals

---

### 2. Retrieval System

Given an input essay:

* Computes similarity to dataset essays
* Retrieves Top-K most relevant examples
* Uses a weighted similarity function

---

### 3. Feedback Generation

Generates feedback by:

* Comparing query essay to retrieved examples
* Identifying strengths and weaknesses
* Producing structured suggestions

---

### 4. Evaluation Pipeline

Measures system performance using:

* Statistical diagnostics
* Distribution analysis
* Alignment plots

---

## 📈 Example Output

```
- This essay shows solid understanding but could be refined further.
- Your vocabulary richness (0.52) is below stronger essays (~0.55).
- Using a wider range of vocabulary could improve your essay.

Predicted Score: 3.4
```

## Demo Screenshot

<img width="551" height="341" alt="First Iteration Demo" src="https://github.com/user-attachments/assets/47183a96-4f21-4d3d-8cc6-dbf4a51e5e3f" />
---

---

## 🧪 Technologies Used

* Python
* Pandas / NumPy
* Scikit-learn
* Matplotlib

---

## 🚀 Future Improvements

* Add semantic embeddings (e.g., sentence transformers)
* Deploy as a Streamlit web app
* Incorporate human grading benchmarks
* Expand feature set (syntax, coherence, grammar)

---

## 🧠 Key Insight

This project demonstrates that:

> Effective essay evaluation can be achieved through **retrieval-based reasoning**, combining interpretability with strong performance—without requiring large language models.

---

## 👤 Author

William V. Fullerton
Statistics & Data Science | Finance Minor
Robert Morris University (Dec 2025)

---

## 📬 Notes

This project was developed as part of a broader exploration into:

* Explainable AI
* Retrieval-Augmented Generation (RAG)
* Educational technology systems

---

⭐ If you found this interesting, feel free to explore the notebooks and reach out!
