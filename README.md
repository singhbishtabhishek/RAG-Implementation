# RAG (Retrieval Augmented Generation)-Implementation

RAG (Retrieval-Augmented Generation) is a method that enhances LLMs (like GPT) by allowing them to access external information during generation. 

This project implements a simple RAG pipeline using Google Generative AI, Langchain and chroma vector database.It retrieves relevant documents using embeddings, then passes them to a language model to generate grounded and context-aware answers.

# How RAG work

**Ingest**

Loads the files, link or given data.

**Embed**

Convert the document into vector representations.

**Store**

Save vectors in a vector database (in this case Chroma)

**Retrieve**

When the question is asked, RAG converts it to vector and retrieve the most relevant answer to the question frm the given document or link.

**Generate**

Generate acccurate and relevant answer.

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

https://smith.langchain.com

You can use your API keys in the code (replacing the API keys with GoogleAPIkey and LangchainAPIkey). 

# Working 

**-** Documents are embedded using Google Generative AI embeddings.

**-** Chroma stores these embeddings and retrieves relevant chunks.

**-** A Gemini/Gemma model answers questions using the retrieved chunks as context.

**You can change the reading document link with another link of your choice**



