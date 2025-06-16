# RAG (Retrieval Augmented Generation)-Implementation

This project implements a simple RAG pipeline using Google Generative AI, Langchain and chroma vector database.It retrieves relevant documents using embeddings, then passes them to a language model to generate grounded and context-aware answers.

# Features
**-** Document retrieval with ChromaDB

**-** Embedding powered by Google Generative AI

**-** Question answering using Gemini/Gemma via LangChain

**-** PDF/Text/Markdown file ingestion

**-** Fully customizable and extendable

# Requirements

You need to install the required libraries in requirements.txt file.

# Setting your API keys

**Google Studio API key** 

To use Google's Gemini models (e.g., gemini-pro, gemma-*), you need to create an API key from Google AI Studio.

https://aistudio.google.com/app/apikey

**Langchain API key**

To enable LangSmith (LangChain’s tracing and observability platform), you’ll need to get an API key.

https://smith.langchain.com/

You can use your API keys in the code (replacing the API keys with GoogleAPIkey and LangchainAPIkey). 

# Working 

**-** Documents are embedded using Google Generative AI embeddings.

**-** Chroma stores these embeddings and retrieves relevant chunks.

**-** A Gemini/Gemma model answers questions using the retrieved chunks as context.

**You can change the reading document link with another link of your choice**

# Output 

**Question asked**

![image](https://github.com/user-attachments/assets/f486d269-fd43-48bc-905f-77de1ea9ff6a)

**Answer generated**

![image](https://github.com/user-attachments/assets/0701d4af-d368-44d2-9035-d1f165534812)


