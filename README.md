# 🩺 Physician Notetaker – NLP Pipeline

![Physician Notetaker](images/doctor.png)

## 📌 Project Overview
Physician Notetaker is an AI-powered NLP system designed to process doctor–patient medical conversations and transform unstructured text into structured clinical information. The project demonstrates how Natural Language Processing (NLP) and Transformer-based models can be applied for:

- Medical data extraction  
- Patient sentiment and intent analysis  
- Automated SOAP note generation  

This project was developed as part of an **AI Engineer Intern assignment**.

---

## 🎯 Objectives
- Extract key medical details from conversation transcripts  
- Analyze patient sentiment and intent  
- Generate structured clinical documentation (SOAP Notes)  

---

## 🧠 Features Implemented

### 1️⃣ Medical NLP Summarization
- Extracts:
  - Symptoms  
  - Diagnosis  
  - Treatment  
  - Prognosis  
- Techniques:
  - **spaCy** for sentence processing  
  - Rule-based keyword matching  
  - **KeyBERT** for keyword extraction  
- Output: Structured medical data in JSON format  

### 2️⃣ Sentiment & Intent Analysis
- Model: HuggingFace Transformers (DistilBERT)  
- Sentiment classification:
  - Anxious  
  - Neutral  
  - Reassured  
- Intent detection:
  - Seeking reassurance  
  - Reporting symptoms  
  - Reassured  

### 3️⃣ SOAP Note Generation (Bonus Feature)
Automatically converts transcripts into a SOAP Note:

- **Subjective** – Patient symptoms and history  
- **Objective** – Physical examination findings  
- **Assessment** – Diagnosis and condition severity  
- **Plan** – Treatment plan and follow-up instructions  

Output: Structured JSON format SOAP notes  

---

## 🛠️ Tech Stack
- Python 3  
- Google Colab / Jupyter Notebook  
- spaCy  
- HuggingFace Transformers  
- KeyBERT  
- PyTorch  
- scikit-learn  

---

## ⚙️ Setup Instructions

### 1️⃣ Install Required Libraries

pip install spacy transformers torch keybert scikit-learn
python -m spacy download en_core_web_sm
2️⃣ Run the Project

Open the .ipynb notebook in Google Colab.

Run all cells sequentially.

Final outputs include:

Medical Summary (JSON)

Sentiment & Intent (JSON)

SOAP Note (JSON)

📝 Design Notes

Rule-based techniques used for medical entity extraction

Pre-trained transformer models applied without fine-tuning

Project emphasizes pipeline design, not clinical deployment

Easily extendable with fine-tuned medical NLP models

🚀 Future Improvements

Fine-tune BERT on medical datasets

Use clinical NLP models like BioBERT or ClinicalBERT

Improve NER accuracy using medical ontologies

Add speech-to-text support for real-time transcription

👤 Author

Ritik Srivastava
