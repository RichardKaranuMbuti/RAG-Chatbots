# RAG-Chatbots

Empower LLMs to answer from custom knowledge, either as ingested text, PDFs, or from the web.

## Introduction

**Retrieval-Augmented Generation (RAG)** is a method that combines retrieval-based methods and generation-based methods to improve the accuracy and relevance of the generated text. In a RAG system, relevant documents or pieces of information are retrieved from a knowledge base and used to inform the generation of responses, making it particularly effective for tasks that require detailed and accurate information.

## About This Repository

In this repository, I show you how to implement custom RAG pipelines, including:

- Training from a set of PDF files
- Training from web sources
- Forwarding the final documents to OpenAI for more refined and contextualized answers

This approach leverages both AzureOpenAI and OpenAI models as LLMs, as well as free embedding models from the Hugging Face Hub. I have used both Pinecone (commented out) and Chroma DB as vector stores/retrievers.

Leave a comment if you have any questions or suggestions!

## Notebooks

There are 3 notebooks in this repository:

1. **Custom_bot_tool_selection** - Implements a custom knowledge-based trained bot that checks the user data and process and advises the best tool to use for compliance flair biomedical research tools.
2. **Train_on_your_pdfs_bot** - Shows the implementation of a chatbot that only answers from specified documents.
3. **Train_from_biorxiv** - Implements a bot that takes a query, scrapes articles from bioRxiv, and answers from those articles. This is ideal for research where references and authenticity/academic integrity are mandatory.
