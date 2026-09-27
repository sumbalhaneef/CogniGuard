# 🛡️ CogniGuard
## AI-Powered Misinformation Risk Analyzer

CogniGuard is an AI-powered system that analyzes news claims and statements to identify potential misinformation warning signals. It combines a local Large Language Model (Llama 3.2), Ollama embeddings, and Retrieval-Augmented Generation (RAG) to provide contextual analysis and verification guidance.

> **Note:** CogniGuard does not determine whether a claim is definitively true or false. It provides AI-assisted risk analysis and recommends ways to verify important claims using reliable sources.

---

## 🚀 Features

- 🧠 AI-powered claim analysis using Llama 3.2
- 🔎 Retrieval-Augmented Generation (RAG)
- 📚 Knowledge-base retrieval using semantic similarity
- 🛡️ Misinformation warning-signal detection
- 📊 Risk-oriented analysis
- ✅ Verification guidance
- 🔒 Runs locally using Ollama
- 💻 Simple Streamlit web interface

---

## 🏗️ System Architecture

```text
User Claim
    ↓
Ollama Embedding Model
    ↓
Knowledge Base Retrieval
    ↓
Relevant Context
    ↓
Llama 3.2
    ↓
AI Risk Analysis
    ↓
Warning Signals + Verification Advice
```

---

## 🛠️ Technologies Used

- Python
- Streamlit
- Ollama
- Llama 3.2
- Nomic Embed Text
- NumPy
- Retrieval-Augmented Generation (RAG)
- Cosine Similarity

---

## 📂 Project Structure

```text
CogniGuard/
│
├── app.py
├── analyzer.py
├── rag_pipeline.py
├── test_rag.py
├── requirements.txt
├── .gitignore
│
└── data/
    └── knowledge_base.txt
```

---

## ⚙️ How It Works

1. The user enters a news claim or statement.
2. CogniGuard converts the claim into an embedding using `nomic-embed-text`.
3. The system compares the claim with information stored in its knowledge base.
4. Relevant context is retrieved using cosine similarity.
5. The retrieved context is provided to Llama 3.2.
6. The model generates a risk-oriented analysis.
7. CogniGuard provides warning signals and verification advice.

---

## ▶️ Run Locally

### 1. Clone the repository

```bash
git clone https://github.com/sumbalhaneef/CogniGuard.git
cd CogniGuard
```

### 2. Create a virtual environment

```bash
python -m venv venv
```

### 3. Activate the virtual environment

**Windows PowerShell:**

```powershell
.\venv\Scripts\Activate.ps1
```

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

### 5. Make sure Ollama models are available

```bash
ollama pull llama3.2
ollama pull nomic-embed-text
```

### 6. Run the application

```bash
streamlit run app.py
```

---

## 🔍 Example

### Input

> Scientists have discovered a medicine that can cure every disease in the world.

CogniGuard can identify signals such as:

- Extraordinary claim
- Absolute language
- Universal promise
- Lack of specific supporting evidence

It then recommends verification using credible scientific and medical sources.

---

## ⚠️ Limitations

CogniGuard is an AI-assisted analysis tool, not a fact-checking authority.

The current version focuses primarily on text-based misinformation risk analysis. It does not currently perform direct image, video, or audio deepfake classification.

AI-generated analysis may also contain errors, so important claims should always be independently verified.

---

## 🎯 Future Improvements

- Image-based deepfake analysis
- Video deepfake detection
- Audio manipulation detection
- Web-based source verification
- Real-time news verification
- Larger verification knowledge base
- Source credibility scoring
- Multi-language claim analysis

---

## 👩‍💻 Author

**Sumbal Haneef**

BS Computational Science Student | AI & Agentic AI Learner

**GitHub:** [sumbalhaneef](https://github.com/sumbalhaneef)

---

⭐ If you find this project useful, consider giving the repository a star.