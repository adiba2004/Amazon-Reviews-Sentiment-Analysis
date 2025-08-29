# Amazon-Reviews-Sentiment-Analysis

This project fine-tunes DistilBERT on 1,000 Amazon product reviews to classify sentiments into Positive, Neutral, and Negative.
It uses Focal Loss for class imbalance and exports a ready-to-use package for Streamlit.

🔹Features

DistilBERT + Focal Loss

3 sentiment classes (Positive, Neutral, Negative)

Evaluation with Accuracy & F1

Auto ZIP export for Streamlit deployment

🔹Tech Stack

Python 3.10+

Transformers (Hugging Face) – Model & Tokenizer

PyTorch – Training backend

scikit-learn – Label encoding & class weights

Evaluate – Accuracy & F1 metrics

Joblib – Label encoder persistence

Streamlit – Deployment

🔹Process
1. **Load & Balance Dataset** – Import dataset, filter sentiments (Positive, Neutral, Negative), and balance classes (\~333 each).
2. **Preprocess & Encode** – Tokenize reviews using DistilBERT tokenizer and encode labels with scikit-learn.
3. **Train Model** – Fine-tune DistilBERT with **Focal Loss** for 5–8 epochs using Hugging Face `Trainer`.
4. **Evaluate** – Compute **Accuracy** and **Weighted F1** on test set.
5. **Export & Deploy** – Save model, tokenizer, label encoder, and auto-package into a **ZIP** for Streamlit deployment.
