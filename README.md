# Ethical AI: Bias Detection and Fairness Optimization in Large Language Models

## Overview
This repository contains the work carried out for the dissertation project **“Ethical AI: Bias Detection and Fairness Optimization in Large Language Models”**, submitted to the **University of Essex** for the MA981 Dissertation module.

The project explores how Large Language Models (LLMs) can inherit and amplify social biases from their training data. It focuses on identifying biased outputs and evaluating different techniques that aim to improve fairness while keeping model performance largely unchanged.

---

## Project Aim
The aim of this study is to better understand bias and fairness in LLM outputs by:
- Identifying and measuring different types of bias in generated text  
- Comparing machine learning models used to detect biased content  
- Evaluating fairness mitigation techniques  
- Examining how computational bias metrics relate to human fairness judgments  

---

## Dataset
The dataset consists of **200 LLM-generated outputs** collected across multiple application areas, including healthcare, hiring, education, legal advice, customer support, and general chat systems.

Each sample includes information about:
- The type of bias involved (gender, religion, age, socioeconomic status, culture, disability, or race)
- Bias scores before and after mitigation
- Toxicity and sentiment scores
- Accuracy-related metrics
- Human-assigned fairness ratings

The data was cleaned, encoded, and extended to support detailed analysis and modelling.

---

## Methodology

### Bias Detection Models
To detect biased outputs, several machine learning models were implemented and compared:

1. **Logistic Regression**  
   Used as a simple and interpretable baseline to understand how different features influence bias detection.

2. **Random Forest**  
   A more powerful model capable of capturing non-linear relationships. It achieved the strongest overall performance in identifying biased content.

3. **Support Vector Machine (RBF Kernel)**  
   Applied to handle complex decision boundaries where linear separation was not sufficient.

### Fairness Prediction
In addition to classification, **Linear Regression** was used to predict human fairness ratings based on computational metrics such as bias, toxicity, and sentiment. This helped evaluate how well automated signals align with human judgments.

---

## Fairness Mitigation Strategies Evaluated
The project examines several commonly used bias-reduction techniques, including:
- Reinforcement Learning from Human Feedback (RLHF)
- Adversarial Debiasing
- Data Balancing
- Fairness Regularization
- Prompt Engineering
- Output Filtering

Bias levels before and after applying these methods were compared to understand their effectiveness and potential trade-offs.

---

## Evaluation Metrics
Model performance and fairness were assessed using:
- Accuracy
- Precision, Recall, and F1-score
- Cohen’s Kappa Score
- Mean Squared Error (MSE)
- Correlation analysis between human fairness ratings and computational metrics

---

## Key Findings
Some of the main observations from the study include:
- Random Forest consistently outperformed Logistic Regression and SVM in detecting biased outputs
- Bias and toxicity are strongly negatively correlated with human fairness ratings
- Accuracy alone does not strongly influence how fair an output is perceived to be
- Several mitigation strategies significantly reduced bias without causing noticeable drops in accuracy
- Outputs from sensitive domains such as healthcare and education benefit from increased human oversight

---

## Tools and Technologies
- Python  
- Pandas and NumPy  
- Scikit-learn  
- Matplotlib  
- Jupyter Notebook  

---

## Author
**Mada Sai Kiran**  
University of Essex
