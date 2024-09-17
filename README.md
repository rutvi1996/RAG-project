Project Name: Cover Letter Generator with RAG (Retrieval-Augmented Generation)

Objective: The goal of this project was to build a system that uses a retrieval-augmented generation approach to create tailored cover letters based on previous resumes, cover letters, and project descriptions. The system retrieves relevant text segments using semantic similarity and then feeds this context to a generative model to craft a personalized cover letter.

Technologies Used:

Python: Main programming language.
Hugging Face Transformers: Used for leveraging pre-trained models for both text embedding and generation.
PyTorch: Utilized for managing model operations and embeddings.
scikit-learn: Employed for cosine similarity calculations to retrieve the most relevant documents based on the query.
Process Overview:

Text Extraction: Extracted text data from PDF and DOCX files containing resumes, cover letters, and project descriptions.
Text Embedding: Generated embeddings for the extracted texts using a pre-trained Sentence-BERT model to capture semantic meanings.
Semantic Retrieval: Implemented a retrieval system using cosine similarity to find texts most relevant to a given job description.
Text Generation: Utilized a pre-trained GPT-2 model to generate cover letters based on the retrieved context and specific job requirements.
Evaluation: Conducted basic testing of the system’s effectiveness and noted potential areas for improvement.
Key Findings:

The output quality was limited by the capabilities of the GPT-2 model, particularly in terms of generating contextually rich and highly relevant content.
Future enhancements could include upgrading to more advanced models like GPT-3 for improved performance.
