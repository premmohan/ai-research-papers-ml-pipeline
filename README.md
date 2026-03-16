# 🧠 AI Research Papers - ML Algorithms (2020-2026)

[![Kaggle Dataset](https://img.shields.io/badge/Kaggle-Dataset-blue?logo=kaggle)](https://www.kaggle.com/datasets/impremmohan/global-ai-research-papers-2020-2026)
[![Kaggle Notebook](https://img.shields.io/badge/Kaggle-Notebook-orange?logo=kaggle)](https://www.kaggle.com/code/impremmohan/complete-ml-analysis-on-ai-research-papers)
[![Kaggle Model](https://img.shields.io/badge/Kaggle-Model-green?logo=kaggle)](https://www.kaggle.com/models/impremmohan/ai-research-papers-2020-2026)



> End-to-End Machine Learning Pipeline built on 10,000 real AI research papers collected from arXiv (2020-2026)

---

## 📊 Project Overview

This project analyzes 10,000 real AI/ML research papers from arXiv and builds a complete machine learning pipeline from data collection to model deployment.

### What This Project Covers:
- ✅ Real data collection using arXiv API
- ✅ Feature Engineering and Preprocessing
- ✅ Exploratory Data Analysis (EDA)
- ✅ 7 ML Models trained and compared
- ✅ Overfitting vs Underfitting analysis
- ✅ Trained model published on Kaggle

---

## 🔗 Project Links

| Asset | Platform | Link |
|-------|----------|------|
| 📊 Dataset | Kaggle | [Global AI Research Papers 2020-2026](https://www.kaggle.com/datasets/impremmohan/global-ai-research-papers-2020-2026) |
| 📓 Notebook | Kaggle | [ML Algorithms](https://www.kaggle.com/code/impremmohan/complete-ml-analysis-on-ai-research-papers) |
| 🤖 Model | Kaggle | [AI Research Paper Classifier](https://www.kaggle.com/models/impremmohan/ai-research-papers-2020-2026) |
| 💻 Code | GitHub | [This Repository](https://github.com/impremmohan/ai-research-papers-ml-pipeline) |

---

## 📁 Repository Structure
ai-research-papers-ml-pipeline/
├── complete-ml-analysis-on-ai-research-papers.ipynb # Complete ML analysis notebook
├── global_ai_research_papers_2020_2026.csv # Dataset
├── README.md # Project documentation
└── LICENSE # MIT License

## 📋 Dataset Details

| Detail | Value |
|--------|-------|
| Source | arXiv.org |
| Total Papers | 10,000 |
| Time Period | 2020-2026 |
| Categories | cs.AI, cs.LG, stat.ML |
| Columns | 12 |

### Column Dictionary:

| Column | Description |
|--------|-------------|
| paper_id | Unique arXiv identifier |
| title | Full title of the research paper |
| published_year | Year of publication (2020-2026) |
| published_month | Month of publication (01-12) |
| first_author | Lead author name |
| authors_count | Total number of authors |
| primary_category | Main arXiv category |
| all_categories | All associated categories |
| abstract_length | Character count of abstract |
| word_count | Word count of abstract |
| journal_ref | Journal reference if published |
| pdf_url | Direct link to PDF |

## 🤖 Models Implemented

| # | Model | Type |
|---|-------|------|
| 1 | Linear Regression | Regression |
| 2 | Logistic Regression | Classification |
| 3 | Naive Bayes | Classification |
| 4 | K-Nearest Neighbors | Classification |
| 5 | Decision Tree | Classification |
| 6 | Random Forest | Classification |
| 7 | SVM | Classification |

## 🏆 Results

### Classification Target:
- **Individual**: 5 or fewer authors
- **Collaborative**: More than 5 authors

### Model Comparison:

| Model | Performance |
|-------|------------|
| SVM | 🏆 Best |
| Random Forest | Strong |
| KNN | Good |
| Decision Tree | Good |
| Logistic Regression | Moderate |
| Naive Bayes | Moderate |

---

## 📈 Visualizations Included

- Papers published per year
- Top research categories
- Authors count distribution
- Research type distribution
- KNN K-value vs Accuracy
- Feature importance
- Model comparison chart
- Confusion matrices for all models
- Overfitting vs Underfitting demonstration

---

## 🚀 Quick Start

### Use the Trained Model:

```python
pip install kagglehub joblib numpy

import kagglehub
path = kagglehub.model_download("impremmohan/ai-research-papers-2020-2026/Scikit-learn/svm-classifier-v1")

import joblib
import numpy as np

model = joblib.load(f"{path}/svm_model.joblib")
scaler = joblib.load(f"{path}/scaler.joblib")

sample = np.array([[150, 900, 3, 6.0]])
sample_scaled = scaler.transform(sample)
prediction = model.predict(sample_scaled)
print("Collaborative" if prediction[0] == 0 else "Individual")

🛠️ Tech Stack
Tool	Purpose
Python	Programming Language
Pandas	Data Manipulation
NumPy	Numerical Computing
Scikit-learn	Machine Learning
Matplotlib	Visualization
Seaborn	Statistical Plots
arXiv API	Data Collection
Kaggle	Dataset and Model Hosting

📝 Key Learnings
Real-world data collection using APIs
Feature engineering from raw metadata
Comparing multiple ML algorithms
Understanding overfitting vs underfitting
End-to-end ML pipeline development
Model deployment on Kaggle

⚖️ License
This project is licensed under the MIT License.

## 👤 Author                    

**Prem Mohan**

- 🌐 Website: [premmohan.com](https://premmohan.com)
- 📊 Kaggle: [kaggle.com/impremmohan](https://www.kaggle.com/impremmohan)
- 💻 GitHub: [github.com/impremmohan](https://github.com/impremmohan)
- 💼 LinkedIn: [linkedin.com/in/premmohan](https://www.linkedin.com/in/premmohan)

