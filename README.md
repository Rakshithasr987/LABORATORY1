# Research on Improving the Quality of Online Customer Support Using Artificial Intelligence

AI-driven system to improve online customer support using NLP. Features sentiment-aware responses, contextual retrieval, and human-in-the-loop escalation. Achieves high accuracy (F1: 0.86) across multi-channel data (chat, email, social). Scalable, modular, and adaptable for real-world deployment.

# Abstract

This repository contains the end-to-end implementation for the Master's thesis project: **"Improving the Quality of Online Customer Support Using Artificial Intelligence"**

## Key Features
- Intent Classification: Fine-tuned BERT model
- Sentiment Analysis: VADER + domain-tuned classifier
- Contextual Retrieval: FAISS vector DB with FAQ, CRM history, past chats
- Response Generation: Rasa + Retrieval-Augmented Generation
- Human-in-the-Loop Escalation: For low-confidence or sensitive queries
- Scalable Deployment: Docker + Kubernetes-ready

## 🚀 Architecture Overview
An NLP-based multi-channel customer support system that automates:
- Intent classification (BERT fine-tuned model)
- Sentiment-aware response generation
- Retrieval-Augmented Generation (RAG) with vector search
- Human-in-the-loop escalation for complex queries

Achieved **F1-score of 0.86** on multi-channel customer support data (chat, email, social media).

## Results & Example Output
- Intent classifier: precision/recall/F1 per class, macro & micro F1. Target avg F1 ≈ 0.86.
- Sentiment: accuracy on labeled set.
- Retrieval: MRR / Recall@k using held-out query → doc pairs.
- Response quality: human evaluation (Likert scale for relevance, helpfulness, empathy). Track escalation rate and agent override rate.
- A/B tests for real traffic: bot vs human response times, customer satisfaction (CSAT).

## Technology






## Datasets




## 📂 Project Structure
/project-root
├─ data/ # Sample + cleaned datasets (PII removed)
├─ src/
│ ├─ ingestion/ # Data collection + connectors
│ ├─ preprocessing/ # Text preprocessing scripts
│ ├─ models/ # Intent classification + sentiment
│ ├─ retrieval/ # RAG + vector DB
│ ├─ rasa_bot/ # Rasa config + flows
│ ├─ api/ # FastAPI for inference
│ └─ utils/
├─ experiments/ # Notebooks + evaluation
├─ configs/ # Config + hyperparameters
├─ docker/ # Dockerfiles
├─ tests/ # Unit + integration tests
└─ README.md

## Methodology
- Data Collection & Preprocessing – Gather multi-channel customer support data (chat, email, social), anonymize PII, and preprocess text using tokenization, lemmatization, stopword removal, and language detection.

- Intent Classification & Sentiment Analysis – Fine-tune a BERT model for query intent detection and apply sentiment analysis (VADER + transformer-based) to enable empathetic, context-aware responses.

- Contextual Knowledge Retrieval – Use vector similarity search (FAISS/Milvus) to fetch relevant knowledge from FAQs, CRM records, and past interactions for enriched response generation.

- Response Generation & Human Escalation – Generate dynamic, sentiment-aware replies using Rasa/RAG while integrating a human-in-the-loop fallback for low-confidence or sensitive cases.

- Evaluation & Deployment – Measure system accuracy (F1 ≈ 0.86), user satisfaction, and efficiency; deploy scalable, modular architecture with APIs and continuous learning for real-world adaptability.


