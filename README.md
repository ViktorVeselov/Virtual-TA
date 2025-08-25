# AI Chatbot for Student Assistance

## Project Summary

This project aims to create an AI chatbot using a RAG (Retrieval-Augmented Generation) vector store. The chatbot is specifically designed to assist students during a course without providing direct answers to the current module.
Currently the AI_TA_LL2-Template.ipynb is the most advanced copy ready for use. Other files are for testing purposes or metadata.

## Project Team

- **Name:** Christopher J. Watson, Joseph Binny, Viktor Veselov
- **School:** Marcos School of Engineering, University of San Diego
- **Research:** MSAAI Machine Learning TA
- **Date:** 2/27/2024
- **Revision:** 1

## Contents

1. [Introduction](#introduction)
2. [Setup](#setup)
3. [Components](#components)

## Introduction

This project leverages a RAG vector store, powered by a GPT (Generative Pre-trained Transformer) model, to create an AI chatbot tailored for student assistance. The chatbot is designed to provide valuable information without directly answering questions related to the current course module.

## Setup

### Prerequisites

- Python
- PyTorch
- Transformers Library
- Hugging Face Pipeline
- ChromaDB

### Installation

1. Clone the repository.
2. Install the required dependencies.

```bash
pip install -r requirements.txt
```

3. Set up the Hugging Face authentication token.

```python
hf_auth = "You-Need-Your-Own-Key"  # This can be kept in secrets and memory keys
```

4. Configure the model ID and other parameters.

```python
model_id = "meta-llama/Llama-2-7b-chat-hf"
```

## Components
1. Basic Imports
    - Torch
    - Joblib
    - Transformers Library
    - GPTQ Libraries
2. Setup CUDA
    - Check for GPU availability.
    - Set up the default device.
3. Initialize HuggingFace Authentication Token
    - Set up the Hugging Face authentication token.
4. Tokenizing and Model Setup
    - Set up the tokenization and model configuration.
    - Pipeline the model for text generation.
5. Chatbot Function
    - Define a function (AskMeAnything) for chatbot interaction.
6. RAG Vector Store Setup
    - Load documents from a text file.
    - Split documents into chunks.
    - Set up Hugging Face embeddings.
    - Create a RAG vector store using ChromaDB
7. Testing
    - Test the chatbot with sample queries.
8. Future Enhancements
    - Implement model quantization for performance improvement.


