#  Fine-Tuning BERT for Sentiment Analysis (NLP)

##  Project Overview
This project focuses on fine-tuning a pre-trained BERT (Bidirectional Encoder Representations from Transformers) model on the IMDB Movie Reviews dataset for sentiment classification.

The objective is to classify movie reviews as **positive** or **negative** using advanced Natural Language Processing (NLP) techniques.

---

##  Key Features
- Data preprocessing and cleaning
- Train, validation, and test split
- Tokenization using BERT tokenizer (`bert-base-uncased`)
- Fine-tuning a pre-trained transformer model
- Model evaluation using:
  - Accuracy
  - Precision
  - Recall
  - F1 Score
- Confusion Matrix analysis

---

##  Tech Stack
- Python
- Hugging Face Transformers
- PyTorch
- Scikit-learn
- Jupyter Notebook

---

##  Model Performance

| Metric     | Score |
|------------|------|
| Accuracy   | 0.82 |
| Precision  | 0.80 |
| Recall     | 0.84 |
| F1 Score   | 0.82 |

---

##  Workflow
Raw Data → Preprocessing → Tokenization → Model Building → Fine-Tuning → Evaluation → Analysis

---

##  Experiments
- Freeze BERT layers and train only the classifier
- Fine-tune the last few layers of BERT

**Observation:** Fine-tuning improves performance compared to freezing all layers.

---

##  Optimization Techniques
- Reduced dataset size for faster training
- Limited token length (`max_length=128`)
- Adjusted batch size for better performance on CPU

---

##  Results & Insights
The model achieved good performance with balanced precision and recall.  
Confusion matrix analysis shows that most predictions are correct with minimal misclassification.
