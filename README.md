# RAG with GEN AI and FAISS PDF chat with streamlit

This Streamlit application allows users to chat with PDF documents using Google's Gemini AI model. Users can upload PDF files, process them, and then ask questions about the content of those PDFs.

## Features

- Extract text from PDFs
- Process and vectorize text for efficient querying
- Use Google's Gemini AI model for question answering
- Interactive chat interface

## Requirements

- Python 3.7+
- Streamlit
- PyPDF2
- LangChain
- FAISS
- Google GenerativeAI
- python-dotenv

## Setup

1. Clone this repository 
2. Install the required packages:
   ```
   pip install streamlit pypdf2 langchain faiss-cpu google-generativeai python-dotenv
   ```
3. Set up your Google API key in a `.env` file:
   ```
   GOOGLE_API_KEY=your_api_key_here
   ```

## Usage

1. Run the Streamlit app:
   ```
   streamlit run chatpdf.py
   ```
2. Upload PDF files using the sidebar
3. Click "Submit & Process" to extract and vectorize the text
4. Ask questions in the main text input field
5. View AI-generated responses based on the PDF content

## How it works

1. PDF text extraction using PyPDF2
2. Text chunking with LangChain's RecursiveCharacterTextSplitter
3. Text embedding using Google's Generative AI Embeddings
4. Vector storage and similarity search with FAISS
5. Question answering using Google's Gemini Pro model and LangChain

