
# README for Causal Reasoning Project

## 1. Introduction

This project focuses on the application of natural language processing (NLP) techniques to perform causal reasoning. The goal is to automatically identify and understand the cause-effect relationships expressed in text. The project involves two key stages: data augmentation and model training.

---

## 2. Data Augmentation

### 2.1 Synonym Replacement

In this technique, words in the sentences are replaced with their synonyms to generate new sentence variations while preserving the original meaning. This is achieved through the use of WordNet.

### 2.2 Adversarial Sampling

Adversarial sampling is used to create more complex and nuanced samples. We employ DistilBERT for this task.

---

## 3. Model Training

### 3.1 Data Preprocessing

The data is read from a CSV file and split into training and test sets.

### 3.2 Model Architecture

We use DistilBert for sequence classification.

### 3.3 Training

The model is trained using Hugging Face's Trainer class.

---

## 4. Evaluation Metrics

The model is evaluated using Precision, Recall, and F1 Score.

---

## 5. Results

The trained model achieves an F1 Score of approximately 0.859, indicating a high level of performance.

---

## 6. Future Work

- Experiment with more advanced data augmentation techniques.
- Try different model architectures like BERT, RoBERTa, etc.
- Fine-tune the model on domain-specific data.

---
