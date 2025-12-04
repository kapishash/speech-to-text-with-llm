# 🔊 Speech-to-Text with Intent Classification (Whisper + LLM)

This project captures **real-time speech**, converts it into **text using OpenAI Whisper**, and then classifies the user's intent using an **LLM-based few-shot learning approach**.  
It is a complete end-to-end voice understanding pipeline suitable for customer support bots, voice assistants, and NLP experimentation.

---

## 🚀 Features

- 🎤 **Real-time speech recording** with automatic silence detection  
- 📝 **High-quality speech-to-text** using `openai/whisper-small`  
- 🎯 **Intent classification** using `Serj/intent-classifier` (Seq2Seq LLM)  
- 🧠 **Few-shot prompt engineering** for enhanced accuracy  
- ⚡ Fully automated end-to-end workflow  
- 🧩 Clean, production-friendly, modular Python code  

---

## 🧠 Model Architecture

### 1️⃣ Speech-to-Text (STT)  
- **Model:** `openai/whisper-small`  
- Converts 16 kHz audio into accurate text  
- Efficient & lightweight for local use  

### 2️⃣ Intent Classification  
- **Model:** `Serj/intent-classifier`  
- Enhanced using a **custom few-shot prompt** containing examples such as:  
  - Shopping  
  - Technical Issues  
  - Bill/Payment Issues  
  - Customer Support  
  - Product Inquiry  
  - Returns & Refunds  
  - Delivery/Tracking  
  - Subscription Queries  

---


---

## ⚙️ Installation

### 1. Clone the Repository
```bash
git clone https://github.com/kapishash/speech-to-text-with-llm.git
cd speech-to-text-with-llm
```

### 2. Create Virtual Environment
```bash
python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate
```
### 3. Install Dependencies
```bash
pip install sounddevice numpy librosa torch soundfile transformers
```
### Run the Project
```bash
python scripts.py
```
