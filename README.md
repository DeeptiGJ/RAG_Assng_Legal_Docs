# Legal Document RAG Pipeline with ROUGE / BLEU / RAGAS Evaluation
This project demonstrates an end-to-end Retrieval-Augmented Generation (RAG) pipeline for answering questions over legal documents (e.g., NDAs, acquisition agreements, privacy policies). It includes document preprocessing, chunking, vector storage, open-source LLM inference, reranking, and RAG evaluation using ROUGE, BLEU, and RAGAS.

# Features

✅ Load and clean .txt documents from Google Drive

🧹 Preprocess and normalize legal text (noise removal, stop word filtering)

📚 Store embeddings in FAISS vector database

🤖 Open-source LLM response generation 

🔁 Optional reranking using Cohere or custom similarity models

📊 Benchmark-based QA evaluation from datasets like CUAD, ContractNLI, and Privacy-QA

🧪 Evaluation of generated answers using:

ROUGE-L

BLEU

RAGAS (Answer Relevancy, Faithfulness, Context Recall)


🔧 Usage:

Upload legal .txt files to your Colab-connected Google Drive folder

Preprocess and clean text 

Chunk text 

Embed using SentenceTransformers or Qwen3-Embedding (GGUF)

Store in FAISS or ChromaDB

Run RAG using LangChain and an open-source LLM

Evaluate using ROUGE, BLEU, and RAGAS metrics

Inspect low-performing examples and tune chunking/reranking

📉 Evaluation Metrics

ROUGE-L: 0.1184

BLEU: 0.0093

RAGAS (context recall, faithfulness, answer relevancy): Included in notebook

# Future Enhancements
Add streaming LLM output (LangChain tools)

Expand chunking to support more formats (PDFs, HTML)

Integrate QLoRA-fine-tuned models

Deploy via FastAPI for interactive querying
