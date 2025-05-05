# Multi-Label Text Classification for Scientific Papers

This project implements and compares multiple approaches for categorizing arXiv paper summaries into scientific domains using multi-label classification. It includes traditional ML models, deep learning (LSTM), and transformer-based methods.


## Features

- **Diverse Approaches**
  - **Traditional ML**: Logistic Regression, Naive Bayes
  - **Deep Learning**: LSTM with GloVe embeddings
  - **Transformers**: SciBERT fine-tuning
- **Class Imbalance Solutions**
  - Focal Loss
  - Weighted Random Sampling
  - Class Weighting
- **Comprehensive Evaluation**
  - Macro/Micro F1, Precision, Recall
  - Hamming Loss, Jaccard Index
  - Detailed Classification Reports

## Installation

```bash
git clone https://github.com/yourusername/arxiv-classification.git
cd arxiv-classification
python -m venv .venv
source .venv/bin/activate  # Linux/Mac
# OR
.venv\Scripts\activate  # Windows
pip install -r requirements.txt 
```

## Usage 
- Open each notebook and execute line by line

## Results

| Model           | F1 (Macro) | Precision | Recall | Hamming Loss |
|-----------------|------------|-----------|--------|--------------|
| Logistic Reg | 0.74       | 0.73      | 0.75   | 0.12         |
| Naive Bayes   | 0.75       | 0.70      | 0.81   | 0.13         |
| LSTM      | 0.78       | 0.80      | 0.77   | 0.07         |
| SciBERT ( without hyper-parameter tuning)         | 0.79       | 0.82      | 0.77   | 0.07         |
