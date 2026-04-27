# Email Spam Classification

This project implements a machine learning model to classify emails as either **Spam** or **Ham** (not spam). Using a dataset of messages, the project demonstrates a complete end-to-end machine learning workflow, from data cleaning and feature extraction to model training and evaluation.

---

### ## Table of Contents
* [Overview](#overview)
* [Dataset](#dataset)
* [Technologies Used](#technologies-used)
* [Project Workflow](#project-workflow)
* [Installation and Usage](#installation-and-usage)
* [Results](#results)

---

### ## Overview
The goal of this project is to build a robust text classification model. It utilizes the **Multinomial Naive Bayes** algorithm, which is particularly effective for natural language processing tasks where features represent word frequencies or TF-IDF weights.

---

### ## Dataset
The project uses a dataset containing thousands of labeled messages.
* **Labeling:** Messages are categorized as `ham` or `spam`.
* **Cleaning:** The raw data is preprocessed by removing unnecessary columns and encoding categorical labels into numerical values (`ham: 0`, `spam: 1`).

---

### ## Technologies Used
The following Python libraries are essential for this project:
* **Pandas:** Data manipulation and analysis.
* **NumPy:** Numerical computing.
* **Scikit-learn:** Machine learning tools for feature extraction (TF-IDF), model training (Naive Bayes), and evaluation.
* **Matplotlib & Seaborn:** Data visualization.

---

### ## Project Workflow
1. **Data Loading:** Importing the dataset using Pandas with specific encoding handling.
2. **Data Cleaning:** Removing null or redundant columns and renaming features for clarity.
3. **Label Encoding:** Converting text labels into a binary format.
4. **Feature Extraction:** Using `TfidfVectorizer` to convert raw text into numerical features.
5. **Model Training:** Splitting the data into training (80%) and testing (20%) sets and training the `MultinomialNB` classifier.
6. **Evaluation:** Measuring performance using accuracy scores, confusion matrices, and classification reports.
