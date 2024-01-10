# Multi PDF Chat Application

## Overview

This Python script provides a Streamlit web application for interacting with a chat-based system that answers questions based on the content of multiple PDF files. The application leverages various natural language processing and generative AI models to facilitate a conversational experience with the user.

## Prerequisites

Before running the script, make sure to install the required Python packages. You can install them using the following command:

```bash
pip install streamlit PyPDF2 langchain langchain-google-genai google-generativeai faiss-cpu
```

Additionally, you need to set up a Google API key by creating a `.env` file in the project directory with the following content:

```env
GOOGLE_API_KEY=your_google_api_key_here
```

## Usage

Run the Python script to start the Streamlit web application:

```bash
python your_script_name.py
```

Access the application through the provided URL and interact with it by asking questions related to the content of the uploaded PDF files.

## Features

### 1. PDF Processing

- Users can upload multiple PDF files.
- The application extracts text from the PDF files.

### 2. Text Chunking

- The extracted text is split into manageable chunks for efficient processing.

### 3. Embedding and Vector Storage

- Text chunks are embedded using Google Generative AI embeddings.
- The embeddings are stored in a vector store using FAISS.

### 4. Question Answering Chain

- A conversational chain is established using a generative AI chat model (Google Gemini-Pro).
- Users can ask questions related to the uploaded PDF content.

## How to Use

1. Upload PDF files through the sidebar.
2. Click the "Submit & Process" button to extract text and create embeddings.
3. Ask questions in the provided input box and receive answers based on the content of the PDFs.

## Note

Ensure that you use the Google API key responsibly and comply with any terms of service provided by Google for using their APIs. Additionally, be aware of any licensing restrictions on the PDF files you upload and process with this application.