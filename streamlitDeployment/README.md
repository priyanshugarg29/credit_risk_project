 Credit Risk Policy Assistant (RAG-Powered)
This Streamlit app is an AI-powered assistant for interpreting internal credit policy documents. It uses Retrieval-Augmented Generation (RAG) to answer queries based on synthesized UK FCA-aligned credit policies for personal loans, auto finance, and SME lending.

 Features
 - Ask domain-specific questions about creditworthiness, approvals, risk flags, etc.

- Answers are grounded in actual policy documents using FAISS + Gemini.

- Based on a real-world financial compliance use case.

- Streamlit interface with example queries and interactive input.

Tech Stack
- Streamlit for the UI

- LangChain for chunking & document management

- FAISS for semantic search

- Gemini API for language generation

- HuggingFace BAAI/bge-base-en for embedding text

DIRECTORY STRUCTURE
├── app.py                  # Main Streamlit application
├── requirements.txt        # Python dependencies
├── faiss_index/            # Vector index for document search
│   ├── index.faiss
│   └── index.pkl
└── .streamlit/
    └── secrets.toml        # API key (not pushed to GitHub)

Example Queries
- What is the minimum income required for a personal loan?

- Are startups eligible for SME loans?

- Who can approve loans above £25,000?

- What are the risk flags for personal loan applicants?

License
For academic use only. Synthesized documents are not real bank policies.
