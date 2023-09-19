# Causal Reasoning Project

## Table of Contents
1. [Introduction](#1-introduction)
2. [Data Augmentation](#2-data-augmentation)
3. [Model Training](#3-model-training)
4. [Evaluation Metrics](#4-evaluation-metrics)
5. [Results](#5-results)
6. [Future Work](#6-future-work)

---

## 1. Introduction

The project aims to harness the capabilities of Natural Language Processing (NLP) to perform causal reasoning tasks, focusing on identifying and understanding cause-effect relationships within textual data. Causal reasoning has been a subject of extensive study within the field of Artificial Intelligence and Linguistics (Pearl, 2009). This project incorporates two significant steps: Data Augmentation and Model Training, aligning with best practices in machine learning pipelines (Goodfellow et al., 2016).

---

## 2. Data Augmentation

### 2.1 Synonym Replacement

Synonym replacement is a straightforward yet effective technique for data augmentation in NLP (Wei and Zou, 2019). The strategy involves replacing selected words with their synonyms, thereby enriching the dataset while retaining the semantic essence of the original sentences. WordNet, a lexical database, provides the synonyms needed for the replacement.

### 2.2 Adversarial Sampling

Incorporating adversarial samples into the training data can make the model more robust (Goodfellow et al., 2014). Adversarial Sampling involves slight perturbations to the input text, generating examples that are more challenging for the model to classify. The use of DistilBERT as the backbone for this task is inspired by its efficiency and relatively lower computational requirements compared to BERT (Sanh et al., 2019).

---

## 3. Model Training

### 3.1 Data Preprocessing

The data is loaded and partitioned into training and test datasets. Preprocessing is an essential step in any machine learning pipeline and significantly influences model performance (Bengio et al., 2015).

### 3.2 Model Architecture

The DistilBert model is used for sequence classification tasks in this project, following the Transformer architecture's success in NLP tasks (Vaswani et al., 2017).

### 3.3 Training

The model is trained using the Hugging Face's Trainer class, following best practices for fine-tuning pre-trained models (Wolf et al., 2020).

---

## 4. Evaluation Metrics

Model performance is gauged through the metrics of Precision, Recall, and F1 Score. These metrics are standard in the evaluation of classification tasks in NLP (Sokolova and Lapalme, 2009).

---

## 5. Results

The final model manifests an F1 Score of approximately 0.859, showcasing strong performance in causal reasoning tasks. This result is indicative of the model's ability to generalize well on unseen data.

---

## 6. Future Work

- Further research could involve the exploration of more advanced data augmentation techniques, as suggested by recent works (Xie et al., 2020).
- Alternative model architectures like BERT and RoBERTa could be investigated for potentially improved performance (Devlin et al., 2018; Liu et al., 2019).
- Fine-tuning the model for domain-specific causal reasoning tasks opens up avenues for more targeted applications.

---

### References

- Pearl, J. (2009). "Causality."
- Goodfellow, I., Bengio, Y., and Courville, A. (2016). "Deep Learning."
- Wei, J. and Zou, K. (2019). "EDA: Easy Data Augmentation Techniques for Boosting Performance on Text Classification Tasks."
- Goodfellow, I. J., Shlens, J., and Szegedy, C. (2014). "Explaining and Harnessing Adversarial Examples."
- Sanh, V., Debut, L., Chaumond, J., and Wolf, T. (2019). "DistilBERT, a distilled version of BERT: smaller, faster, cheaper and lighter."
- Bengio, Y., Courville, A., and Vincent, P. (2015). "Representation Learning: A Review and New Perspectives."
- Vaswani, A., Shazeer, N., Parmar, N., Uszkoreit, J., Jones, L., Gomez, A. N., ... & Polosukhin, I. (2017). "Attention is all you need."
- Wolf, T., Debut, L., Sanh, V., Chaumond, J., Delangue, C., Moi, A., ... & Rush, A. M. (2020). "Transformers: State-of-the-Art Natural Language Processing."
- Sokolova, M., & Lapalme, G. (2009). "A systematic analysis of performance measures for classification tasks."
- Xie, Q., Dai, Z., Hovy, E., Luong, M. T., & Le, Q. V. (2020). "Unsupervised Data Augmentation for Consistency Training."
- Devlin, J., Chang, M. W., Lee, K., & Toutanova, K. (2018). "BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding."
- Liu, Y., Ott, M., Goyal, N., Du, J., Joshi, M., Chen, D., ... & St