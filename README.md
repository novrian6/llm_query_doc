Developer : Nova Novriansyah
PDF Question Answering with Sentence Transformers and GPT-4

This Python script uses Sentence Transformers and GPT-4 to answer questions based on the content of a PDF document. The script performs the following steps:

Reads a PDF file using PyPDF2 and pdfplumber.
Splits the text into paragraphs using RecursiveCharacterTextSplitter.
Encodes each paragraph using Sentence Transformers.
Chooses the most relevant paragraph based on the user's query.
Queries a GPT-4 model for a final answer.
Requirements

Python 3.6+
Required Python libraries:
PyPDF2
pdfplumber
langchain (for RecursiveCharacterTextSplitter)
sentence-transformers
sentence_transformers models
gpt4all (for GPT-4)
You can install the required libraries using pip:
bash
Copy code
pip install PyPDF2 pdfplumber langchain sentence-transformers gpt4all
Usage

Place the PDF file (mydoc.pdf in the example) in the same directory as the script.
Run the script:
bash
Copy code
python pdf_question_answering.py
Enter your question when prompted.
The script will provide the answer using Sentence Transformers and GPT-4.
Additional Notes

The script uses a GPT-4 model from the GPT4All library. You can change the model by modifying the llm variable.
Ensure you have an active internet connection for the GPT-4 model to work.
The script provides a progress bar to indicate the progress of each step.
Example

Here is an example usage of the script:

Run the script:
bash
Copy code
python pdf_question_answering.py
Enter your question when prompted:
python
Copy code
Enter your question (or type 'exit' to quit):
What is the capital of France?
The script will provide the answer based on the content of the PDF.
