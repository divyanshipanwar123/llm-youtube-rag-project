# 🎬 Chat with YouTube Videos using GenAI (RAG Pipeline)
This project demonstrates how to build a **Retrieval-Augmented Generation (RAG)** pipeline using **LangChain**, **HuggingFace**, and **ChromaDB**, allowing users to chat with the content of any YouTube video by extracting and embedding its transcript.
## 🧠 What I Learned
As someone with a Python background but new to LLMs and LangChain, this project helped me understand:

- The basics of Hugging Face pipelines
- How to extract and process transcripts using LangChain
- What a vector database (Chroma) is and how embeddings work
- How to build a RAG-based chatbot over video content

## 🚀 Features
- 📥 Extracts transcript from YouTube videos automatically
- 📚 Splits long transcripts into manageable chunks
- 🔍 Embeds and stores transcript in Chroma vector DB
- 🤖 Lets you ask questions and get AI-generated answers based only on the video
- 🧾 Accurate, context-based retrieval using LangChain's retrieval chain

## 🛠️ Tech Stack
| Component        | Purpose                                |
|------------------|----------------------------------------|
| Python           | Programming language                   |
| Google Colab     | Cloud-based Development environment    |
| LangChain        | LLM chaining and RAG pipeline          |
| OpenAI API       | Embedding and GPT-based answering      |
|Hugging Face Transformers | Free LLMs & Embeddings (used instead of OpenAI) |
| Chroma           | Vector store for document retrieval    |
| youtube-transcript-api | Fetch video transcript without using youtube DATA API |

## 💡 Why Hugging Face Instead of OpenAI?

Initially, I planned to use OpenAI's GPT models and embeddings in this project. However, due to API quota limitations and the requirement to add billing details (which are not ideal for early experimentation), I switched to using **Hugging Face models**.

Hugging Face provides free and open alternatives for both: 
 - 🔹 Text Embeddings (`all-MiniLM-L6-v2`)
 - 🔹 Text Generation (`flan-t5-large`)

This allows the project to remain:
- ✅ Free to run
- ✅ Fully functional in Google Colab
- ✅ Beginner-friendly for anyone who wants to test GenAI without paying


## 📘 Future Improvements

- 🔄 Add a user interface using **Streamlit** for a more interactive experience
- 📝 Display full transcript and allow on-demand summarization
- 💬 Include a chat history panel for user queries
- 🔒 Add basic authentication to restrict access
- 📁 Allow user to upload their own video or document for Q&A

