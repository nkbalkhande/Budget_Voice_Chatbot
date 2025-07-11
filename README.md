# 📊 Indian Budget Voice Chatbot (Multilingual with Translation & Audio)

This is a Streamlit-based intelligent chatbot that lets users ask **budget-related questions** from an uploaded PDF file (e.g., Union Budget) using **voice or text**, in **multiple Indian languages**. It answers using **Gemini LLM**, with **translation**, **speech synthesis**, and **document-grounded retrieval** using **Pinecone**.

---

## 🚀 Features

✅ Upload and analyze Budget PDF documents  
✅ Ask questions using voice or text in 10+ Indian languages  
✅ Translation powered by Deep Translator  
✅ Embeddings via Gemini's embedding model  
✅ Retrieval-Augmented Generation (RAG) using Pinecone  
✅ Real-time voice-to-text and text-to-speech  
✅ Streaming answers with source chunk display  

---

## 🖥️ Tech Stack

- **Streamlit** – for UI
- **LangChain** – RAG and chaining
- **Google Gemini** – LLM & Embeddings (`gemini-2.0-flash`, `embedding-001`)
- **Pinecone** – Vector DB for document search
- **Deep Translator** – Language translation
- **SpeechRecognition + gTTS** – Voice input and output

---

## 🌐 Supported Languages

- English
- Hindi
- Telugu
- Tamil
- Kannada
- Marathi
- Gujarati
- Bengali
- Punjabi
- Malayalam

---

## 📦 Installation

1. **Clone the repo:**

```bash
git clone https://github.com/nkbalkhande/Budget_Voice_Chatbot.git
cd Budget_Voice_Chatbot
```

## Install dependencies:

```bash
pip install -r requirements.txt
```

---
## Set your API keys:
Create a .env file:
```bash
GEMINI_API_KEY=your_google_gemini_api_key
PINECONE_API_KEY=your_pinecone_api_key
```
-- 
## 🧠 How It Works
- Upload a Budget PDF

- PDF is split into chunks and embedded using Gemini

- Stored in Pinecone vector DB

- User asks question in their language (via voice or text)

- Translated to English → RAG with Gemini → Translated back

- Answer is spoken and shown in selected language

- Source document snippets shown for transparency

## 🧪 Run the App
```bash
streamlit run streamlit_app_transaltor.py
```
