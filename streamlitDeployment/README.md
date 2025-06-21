# 📄 Credit Risk Policy Assistant (RAG-Powered)

This Streamlit app is an AI-powered assistant for interpreting internal credit policy documents.
It uses **Retrieval-Augmented Generation (RAG)** to answer queries based on simulated UK FCA-aligned credit policies.

## 🚀 Features
- 💬 Ask questions about creditworthiness, approvals, risk flags, and exceptions
- 🔍 Answers are grounded in real (simulated) policy documents
- 🧠 Uses FAISS for retrieval and Gemini LLM for generation
- 🖥️ Streamlit frontend with interactive input and downloadable results

## 🧪 Sample Queries
- What is the minimum income required for a personal loan?
- Are startups eligible for SME loans?
- Can a customer with a high-performance car apply for auto finance?
- Who can approve loans above £25,000?
- What are the risk flags for personal loan applicants?

## 🧱 Tech Stack
- Streamlit
- LangChain
- FAISS
- HuggingFace Transformers
- Gemini API

## 📁 Project Structure
```
streamlitDeployment/
├── app.py                  # Streamlit UI logic
├── requirements.txt        # All required packages
├── .streamlit/
│   └── secrets.toml        # Contains GEMINI_API_KEY (set on Streamlit Cloud)
├── faiss_index/
│   └── index files         # Precomputed document embeddings
```

## 🔐 Secrets Setup (Streamlit Cloud)
Add the following under **App Settings > Secrets** on [Streamlit Cloud](https://streamlit.io/cloud):
```toml
GEMINI_API_KEY = "your_google_gemini_api_key"
```

## 📎 License
For academic/demo use only. The policies are AI-simulated based on public regulatory guidance.

## 👨‍💻 Author
Priyanshu Garg – MSc Business Analytics, Warwick Business School