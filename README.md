# 🏥 SLM-Powered Healthcare Policy Chatbot with RAG & LoRA

This project is a Retrieval-Augmented Generation (RAG) chatbot fine-tuned with LoRA on healthcare policy documents, designed to assist users in querying Medicaid-related compliance and insurance questions. It integrates a lightweight language model (Flan-T5) with LangChain for policy-aware QA.

---

## 🚀 Project Overview

Traditional large language models often lack domain-specific knowledge or are too resource-heavy for real-time use. This chatbot addresses that by:

- Fine-tuning a compact model using **LoRA** for efficiency
- Leveraging **RAG architecture** to dynamically retrieve policy context
- Utilizing **LangChain** to structure the QA pipeline
- Providing regulatory responses based on Medicaid documentation

---

## 🧠 Model Architecture

- **Base Model**: Flan-T5 (Small or Base)
- **Adaptation**: LoRA fine-tuning on healthcare policy corpus
- **RAG Stack**:
  - Document Loader (PDF, TXT)
  - Text Splitter
  - Embedding Generator (e.g., HuggingFace or OpenAI embeddings)
  - Vector Store (e.g., FAISS, ChromaDB)
- **LangChain**: Used for chaining retrieval + generation

---

## 🛠️ Tech Stack

- `Python`
- `Flan-T5` via HuggingFace Transformers
- `LoRA` via PEFT or HuggingFace
- `LangChain`
- `FAISS` or `ChromaDB` (for vector search)
- Optional: `Streamlit` for demo interface

---

## 🌟 Key Features

- ⚙️ **LoRA-Finetuned SLM**: Reduced resource usage while retaining contextual understanding.
- 🧾 **Policy-Aware QA**: Capable of answering Medicaid-related compliance and regulation questions.
- 🔍 **Document-Aware Retrieval**: Uses vector embeddings to fetch context before response generation.
- 🔄 **Modular Pipeline**: Built with LangChain for flexibility and easy extension.
- 🧠 **Explainable Retrieval**: Shows retrieved document snippets used in generating responses.

---

## 🧑‍💻 Contributions

- Fine-tuned Flan-T5 using LoRA on a custom Medicaid policy dataset.
- Built an end-to-end QA pipeline using LangChain and RAG principles.
- Integrated vector database (FAISS/ChromaDB) with embedding search.
- Developed a use-case focused on real-world Medicaid policy queries.
- Documented evaluation and impact for academic submission.

---

## 📈 Results & Evaluation

- **Inference Latency**: Reduced by ~40% vs full model baseline
- **Accuracy**: Passed 20+ curated policy scenario queries
- **Interpretability**: Retrieval stage logs exposed for transparency

---
