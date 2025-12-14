# Duplicate Question Detection

This repository is about detecting whether two questions are **duplicates** or **not**, meaning they convey the same intent even if the wording is different.

The project is divided into **two clear parts**:
- **Machine Learning approach**
- **Deep Learning approach**

Both are implemented separately so that the difference in performance and capability is easy to observe.

---

## Repository Structure

The repository mainly contains **two folders**:

### 1. Machine Learning Folder
This folder contains a traditional machine learning–based approach.

Here, the problem is solved using:
- Text preprocessing
- Feature extraction
- Classical ML models

This approach works, but it has **clear limitations** when understanding semantic similarity between questions.

---

### 2. Deep Learning Folder
This folder contains the **main contribution** of this project.

The deep learning approach performs **significantly better** compared to the machine learning approach.

Key points:
- Uses **word embeddings** to represent text numerically
- Uses **LSTM-based architectures**
- Implements **double (stacked) LSTMs** for better sequence understanding
- Learns semantic similarity instead of relying only on surface-level features

If you go through the Jupyter Notebook in this folder, you can clearly follow:
- How the data is processed
- How embeddings are used
- How the LSTM model is built
- How predictions are generated

---

## Why LSTMs?

Questions are sequences of words, and their meaning depends on **order and context**.

LSTMs are used because:
- They handle variable-length sequences naturally
- They preserve contextual information
- They work well for sentence-level meaning comparison

Using **stacked (double) LSTMs** improves representation learning and gives more stable results.

---

## Comparison Summary

| Aspect | Machine Learning | Deep Learning |
|------|------------------|---------------|
| Feature handling | Manual | Learned automatically |
| Context understanding | Limited | Strong |
| Performance | Moderate | Better |
| Scalability | Limited | Better for larger data |

The deep learning model clearly outperforms the machine learning approach in this problem.

---

## How to Understand the Work

The best way to understand this project is to:
1. Start with the machine learning folder
2. Then move to the deep learning folder
3. Read the Jupyter Notebook step by step

The notebooks are written in a way that makes it easy to follow the full pipeline.

---

## What This Project Shows

- Practical implementation of duplicate question detection
- Clear comparison between ML and DL approaches
- Effective use of LSTMs for text similarity
- End-to-end NLP pipeline in practice

---

## Final Note

This project focuses on **learning and correctness**, and complexity.

Everything included in this repository is directly related to the problem of duplicate question detection, without adding unrelated techniques or claims.

Feel free to explore, experiment, and build on top of it.
