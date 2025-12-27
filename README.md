# Spam Email Detection

Project Overview : This project focuses on building a machine learning–based email spam detection system using Python. The objective is to automatically classify emails as Spam or Not Spam by learning textual patterns from historical email data. The project demonstrates a complete Natural Language Processing (NLP) and machine learning workflow, including data preprocessing, feature extraction, model training, evaluation, and real-time prediction for custom emails.

Objectives :

- To analyze textual patterns that distinguish spam emails from legitimate emails.
- To preprocess raw email text into a machine-learning-ready format.
- To convert textual data into numerical features using vectorization techniques.
- To build a supervised classification model for spam detection.
- To evaluate model performance using appropriate classification metrics.
- To enable spam prediction for custom, user-defined email content.

Dataset Description :

- The dataset contains labeled email messages.
- Each row represents a single email.
- The dataset includes both spam and non-spam (ham) emails.

Key Features :
- label (Target Variable):
    - 1 → Spam
    - 0 → Not Spam (Ham)
- email:
    - Raw email text content.

Problem Type :

- Supervised Learning
- Binary Classification Problem
- The target variable is categorical, requiring classification-based machine learning models.

Tools and Technologies :

1. Programming Language: Python
2. Development Environment: Jupyter Notebook / VS Code
3. Libraries Used :
  - NumPy – numerical operations
  - Pandas – data manipulation and analysis
  - Matplotlib & Seaborn – data visualization
  - Scikit-learn – preprocessing, feature extraction, model training, and evaluation
  - Regular Expressions (re) – text cleaning

Methodology :

  1. Data Understanding :
      - Inspected dataset structure and class distribution.
      - Identified email text as input feature and label as target variable.
  2. Data Preprocessing :
      - Converted text to lowercase.
      - Removed URLs, special characters, numbers, and extra spaces.
      - Cleaned raw text to improve feature extraction quality.
  3. Feature Engineering :
      - Applied TF-IDF Vectorization to convert email text into numerical feature vectors.
      - Limited feature size to reduce dimensionality and noise.
      - Used built-in English stopword removal for efficiency.
  4. Model Building :
      - Split dataset into training and testing sets (80:20 ratio) using stratified sampling.
      - Trained a Multinomial Naive Bayes classifier, suitable for text-based data.
  5. Model Evaluation :
      - Evaluated performance using:
      - Accuracy Score
      - Confusion Matrix
      - Precision, Recall, and F1-Score (Classification Report)
  6. Prediction :
      - Implemented a function to classify custom email content.
      - Enabled real-time spam detection for user-provided emails.

Key Insights :

1. Spam emails often contain repetitive keywords, promotional language, and urgency-based phrases.
2. TF-IDF effectively captures important word patterns while reducing noise.
3. Multinomial Naive Bayes performs well for text classification with high-dimensional sparse data.
4. The model generalizes well to unseen email content.

Conclusion :
This project demonstrates how machine learning and NLP techniques can be effectively applied to solve real-world classification problems. The spam detection system provides a reliable and scalable solution for filtering unwanted emails, while also serving as a strong foundational project for understanding text-based machine learning workflows.
