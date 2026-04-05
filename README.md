# xRxtance Dataset: Drug Use Stance Detection

## Access the notebooks in colab
  🔗 **Open in Colab:** [00_classification_xRxtance](https://colab.research.google.com/drive/1S8Bu3o9TciI8jpcmXx4WRQBhsy9Cudpw?usp=sharing)
  
  🔗 **Open in Colab:** [01_classification_xRxtance](https://colab.research.google.com/drive/1Zrzl1I8LKPKa3azMJoBGsnmfuZFFnOqt?usp=sharing)
  
  🔗 **Open in Colab:** [02_classification_xRxtance](https://colab.research.google.com/drive/1fk38N721CbSH0HyDsv6qCb0yDM3uswnE?usp=sharing)
  
  🔗 **Open in Colab:** [03_classification_xRxtance](https://colab.research.google.com/drive/1bYdGZUUic3m4He3e5VBReV-YgvYFy-ET?usp=sharing)
  
  🔗 **Open in Colab:** [04_classification_xRxtance](https://colab.research.google.com/drive/1ToMDv83l9-Afj-9uOpAH0FmY2JGRdUWM?usp=sharing)
  
  🔗 **Open in Colab:** [05_classification_xRxtance](https://colab.research.google.com/drive/1VBnBtAXybLQH6y7klsptntZRPtWMVZX4?usp=sharing)

## Overview

Drug abuse is one of the most significant concerns of the 21st century. With the growing use of social media over the past decade, drug-related conversations have increasingly shifted to platforms such as X (Twitter) and YouTube.

Understanding the **stance of users in these conversations** is a crucial task because social media has a strong influence on drug awareness, drug discovery, and public behavior—especially among vulnerable groups such as teenagers.

However, **stance detection on drug use remains an underexplored research area**, largely due to the lack of high-quality datasets.

---

## xRxtance Dataset

This study introduces **xRxtance**, an extended version of the **Rxtance dataset**, designed to address the scarcity of datasets in this domain.

**Key characteristics:**

- **Total posts:** 8,146  
- **Sources:** X (Twitter) and YouTube comments  
- **Annotation:** Three independent annotators  
- **Quality assurance:** Strong inter-annotator agreement  
- **Purpose:** Drug use stance detection research

To validate the dataset quality, multiple **Machine Learning, Deep Learning, and Transformer models** were trained and evaluated.

---

## Model Evaluation Results

| Category | Feature / Embedding | Model | Macro F1 Score |
|---------|---------------------|------|---------------|
| **Machine Learning** | TF-IDF | KNN | **0.51** |
| **Machine Learning** | TF-IDF | Naïve Bayes | **0.50** |
| **Machine Learning** | TF-IDF | SVM | **0.60** |
| **Machine Learning** | TF-IDF | Decision Tree | **0.49** |
| **Machine Learning** | TF-IDF | Random Forest | **0.58** |
| **Deep Learning** | PyTorch Embedding | MLP | **0.57** |
| **Deep Learning** | PyTorch Embedding | BiLSTM | **0.54** |
| **Deep Learning** | PyTorch Embedding | CNN | **0.59** |
| **Transformer** | BERT | Neural Network | ⭐ **0.72 (Best Performance)** |

---

## Key Findings

- **BERT-base achieved the highest performance** with a **Macro-F1 score of 0.712**.
- Among deep learning models, **CNN performed best** with **0.5923**.
- Traditional machine learning models such as **SVM and Random Forest** also showed competitive results.
- High **inter-annotator agreement** confirms the reliability of dataset annotations.

---

## Conclusion

The **xRxtance dataset** addresses the **data scarcity problem in drug stance detection research**. By providing a carefully annotated dataset and baseline benchmarks across multiple model types, this work supports further research in:

- Social media stance detection  
- Public health awareness  
- Drug abuse prevention research

Ultimately, the dataset contributes toward **better understanding drug-related discourse online and promoting drug awareness initiatives**.

---
