
# 🧠 SafeSpace AI – Mental Health Diagnosis & Agent System

Transforming mental health support with voice-enabled diagnosis and AI-powered emotional intelligence.

---

## 🧾 Project Overview

**SafeSpace AI** is an innovative mental health diagnostic platform designed to provide AI-powered emotional support and psychological assessments. Leveraging Large Language Models (LLMs), Whisper-based voice recognition, and Retrieval-Augmented Generation (RAG), SafeSpace AI enables early identification of mental health conditions based on user-reported symptoms. It features a multi-modal interface that supports both text and voice inputs and offers contextualized, evidence-based diagnostic suggestions for better mental wellness outcomes.

---

## 🌟 Key Achievements

- Voice-enabled mental health assistant with Whisper integration
- Gemma-2 9B fine-tuned for mental health reasoning via chat templates
- RAG-based context construction using FAISS and BGE embeddings
- Generated personalized responses with diagnosis, symptoms, treatment, helpline
- CSV feedback logger and PDF generator for session summaries

---

## 🧠 Technology Stack

| Component             | Technology Used                      | Purpose                                      |
|-----------------------|---------------------------------------|----------------------------------------------|
| LLM                   | `gemma-2-9b-it`                       | Mental health diagnosis via text generation  |
| Embeddings            | `BAAI/bge-base-en-v1.5`               | Semantic encoding of user input              |
| Voice Input           | `openai/whisper-base`                | Speech-to-text for mental health queries     |
| Interface             | `Gradio`                              | Web-based voice/text app interface           |
| Retrieval Engine      | `FAISS`                               | Contextual document retrieval                |
| Emotion Classifier    | `nateraw/bert-base-uncased-emotion`   | Optional user sentiment tagging              |
| PDF/CSV Tools         | `Fpdf`, `csv`, `Pandas`               | Report generation and feedback storage       |

---

## 🧩 Core Modules

### 🔍 Retrieval-Augmented Generation (RAG)
- Chunked documents stored and indexed via FAISS
- Top-5 documents retrieved based on semantic similarity
- Combined into context prompt for Gemma LLM

### 🤖 Mental Health Diagnosis Engine
- Prompts LLM to return:
  1. **Diagnosed Mental Disorder**
  2. **Matching Symptoms**
  3. **Personalized Treatment**
  4. **Helpline Numbers**
  5. **Source Link (if available)**

### 🎙️ Voice Interface
- User speaks symptoms
- Whisper converts voice to text
- Pipeline processes response same as text query

---

## 📊 Sample Model Output

| Input Query                            | Diagnosis       | Treatment Provided             |
|----------------------------------------|-----------------|-------------------------------|
| "I’ve lost interest in everything..."  | Depression      | CBT, journaling, support lines |
| "I want to end everything..."          | Suicidal        | Crisis helpline & emergency   |
| "I get panic attacks often"            | Anxiety         | Breathing techniques, therapy |

---

## 🗂 Dataset & Preprocessing

- Internal dataset with 150+ user queries across 6 major disorders
- Stratified sampling for balanced class-wise performance
- Text normalization, prompt tuning, semantic embedding

---

## 📈 Performance Evaluation

| Phase              | Metric            | Value         |
|--------------------|-------------------|---------------|
| Classification     | Accuracy (manual) | ~83%          |
| Retrieval quality  | Top-5 relevance   | High (FAISS)  |
| Output readability | Human eval score  | Strong        |

---

## 🧪 Installation & Setup

```bash
git clone https://github.com/JaamieMaarsh/SafeSpace-AI.git
cd SafeSpace-AI
pip install -r requirements.txt
```

Create a `.env` file with:

```bash
HF_TOKEN=your_huggingface_token
```

Run the application:

```bash
python app.py
```

---

## 🏥 Clinical Use Cases

- First-line psychological screening in telemedicine apps  
- Emotional wellness support for anonymous users  
- Mental health triage assistant for universities and workplaces

---

## 🎓 Academic Context

- **Institution**: Northeastern University  
- **Course**: Generative AI Systems  
- **Duration**: January 2025 – April 2025  
- **Project Lead**: Kalyan Kumar Chenchu Malakondaiah  
- **LinkedIn**: [linkedin.com/in/chenchumalakondaiah](https://linkedin.com/in/chenchumalakondaiah)

---

## 🪪 License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

---

## 🚀 Quick Start

```bash
git clone https://github.com/JaamieMaarsh/SafeSpace-AI.git
cd SafeSpace-AI
pip install -r requirements.txt
python app.py
```

---

## 🙋 Contact

For queries, ideas, or collaborations:  
📬 [LinkedIn – Kalyan Kumar Chenchu Malakondaiah](https://linkedin.com/in/chenchumalakondaiah)

