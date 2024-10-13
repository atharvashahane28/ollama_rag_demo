# CS320 Ollama Rag Demo

RAG LLM demo with CAMS Banking Instructions PDF, for presentation 3.

Link to PDF on ISONE website: 

## Requirements

- [Ollama](https://ollama.ai/) verson 0.1.26 or higher.

## Setup

1. Clone this repository to your local machine.
2. Create a Python virtual environment by running `python3 -m venv .venv`.
3. Activate the virtual environment by running `source .venv/bin/activate` on Unix or MacOS, or `.\.venv\Scripts\activate` on Windows.
4. Install the required Python packages by running `pip install -r requirements.txt`.

## Running the Project

**Note:** The first time you run the project, it will download the necessary models from Ollama for the LLM and embeddings. This is a one-time setup process and may take some time depending on your internet connection.

1. Ensure your virtual environment is activated.
2. In the terminal, navigate to the current project folder and run `python app.py -m mistral -p .\ISO_Docs\`

This will load the PDFs and Markdown files, generate embeddings, query the collection, and start a question-answer program that runs in the terminal. Enter the question that you want to ask. Depending on the specs of your laptop/PC, it might take about 45-60 seconds (sometimes more) to load the answer. To quit, enter `exit` or use the keyboard interrupt (CTRL + C) on Windows.

## Technologies Used

- [Langchain](https://github.com/langchain/langchain): A Python library for working with Large Language Model
- [Ollama](https://ollama.ai/): A platform for running Large Language models locally.
- [Chroma](https://docs.trychroma.com/): A vector database for storing and retrieving embeddings.
- [PyPDF](https://pypi.org/project/PyPDF2/): A Python library for reading and manipulating PDF files.
