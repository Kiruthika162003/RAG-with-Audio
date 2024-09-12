## Problem Statement

This project demonstrates how to use LangChain for Retrieval Augmented Generation (RAG) with an audio file. The problem is to efficiently retrieve relevant information from an audio transcription and use it to answer questions.

## Results Interpretation

The results show that the LangChain model can effectively retrieve and interpret information from an audio transcription. This means that the model can be used to automate the process of extracting useful information from audio content.

## Steps Done

1. **Install Dependencies**: Installed necessary libraries such as LangChain, Pinecone, DocArray, PyPDF, and Whisper.
2. **Install ffmpeg**: Installed ffmpeg based on the platform (Ubuntu, Arch Linux, MacOS, Windows).
3. **Download Audio**: Downloaded an example audio file.
4. **Transcribe Audio**: Used Whisper to transcribe the audio to text.
5. **Save Transcription**: Saved the transcribed text to a file.
6. **Select LLM Model**: Chose the llama3 model and downloaded it.
7. **Instantiate Models**: Initialized the LLM and embedding models using LangChain.
8. **Load Transcription**: Loaded the transcription using TextLoader.
9. **Split Document**: Split the transcription into chunks using RecursiveCharacterTextSplitter.
10. **Store in Vector Space**: Stored the transcription content in a vector space using DocArrayInMemorySearch.
11. **Create Retriever**: Created a retriever to find similar vectors for context.
12. **Generate Conversation**: Used the retriever to generate context and answer questions based on the transcription content.

## Dataset

- **Source**: The dataset is a transcription of an audio file using Whisper.
- **Size**: The size of the dataset depends on the length of the audio transcription.
- **Features**: Key features include the text content of the audio transcription.
- **Preprocessing**: The transcription is split into chunks and stored in a vector space for efficient retrieval.



