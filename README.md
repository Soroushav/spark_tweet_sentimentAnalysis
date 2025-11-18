# Sentiment Analysis with PySpark in a Big Data Context

## 📌 Overview
This project performs **sentiment analysis** using the **Sentiment140** dataset within a **Big Data ecosystem**.  
Our goal is to show how PySpark can be used not only for large-scale **data preprocessing**, but also for **model training and evaluation** using Spark MLlib.

To ensure reproducibility and an isolated environment, the entire workflow is **containerized using Docker**, with Jupyter Notebook as the main development interface.

The main phases of the project include:
- Large-scale preprocessing using PySpark DataFrames
- Feature extraction (TF-IDF / HashingTF)
- Training multiple ML models (SVM, Logistic Regression, Naive Bayes, etc.)
- Evaluating model performance with Spark MLlib
- Optional comparison with BERT embeddings in a separate Colab notebook

---

## 🛠️ Technologies Used

### 🔹 **PySpark**
- Distributed preprocessing  
- ML model training with Spark MLlib  
- Efficient handling of large-scale text data

### 🔹 **Jupyter Notebook**
- Interactive environment for development and analysis  
- Documenting the step-by-step pipeline

### 🔹 **Docker**
- Containerizes PySpark notebook environment  
- Ensures consistent dependencies and reproducible results  

---

## 📁 Dataset

We use the **Sentiment140** dataset, available on Kaggle:

👉 https://www.kaggle.com/datasets/kazanova/sentiment140/data

The dataset contains **1.6 million tweets** labeled as:
- `0` → negative  
- `4` → positive  

This scale makes it suitable for a Big Data approach with PySpark.

---

## 🚀 How to Run the Project

### 1. Clone the repository
```bash
git clone <your-repo-url>
cd <project-folder>
```

### 2. Start the Docker environment
```bash
docker compose up -d
```

### 3. Open Jupyter Notebook

Check the container logs:
```bash
docker compose logs pyspark
```

Open the Jupyter Lab URL with the token printed in the logs.
### 4. Run the notebooks
Load the dataset (from database/ directory)
Follow the preprocessing and modeling pipeline
