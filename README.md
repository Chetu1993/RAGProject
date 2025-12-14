Implemented the RAG method using OLLAMA LLM

1).Used the FASTAPI to upload the Image file in getting_image_file.py file
2).copied the path of the file, used the poppler-path to convert the image file into OCR, then used the tesseract library to convert the image file into string format
3).used the RecursiveCharacterTextSPlitter from langchain to split the text 
4).used the OnnxMiniEmbeddings class to utilize the huggingface Xenova/all-MiniLLM-L6-V2 model and used the sentence-transformers/all-MiniLM-L6-v2 token to call and load the model 
in callable input function, adopted the embed_query and embed_documents to make use of single line text and multi-line texts to make use of in OCR format
5). used the OnnxMiniEmbeddings class in RAG_Request.py file as embeddings as a method, then I have applied the Chroma as a database library to convert and store the numerical values as a vector DB format
6).used the uvicorn to call the FastApi method to get the RAG request through FastAPI
7).validated the RAG response using Requests Library
