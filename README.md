# Crafting-an-AI-powered-HR-Assistant
This project is Retrieval Augmented Generation based AI assistant built using Langchain, ChromaDB, LLM(OpenAI) and Gradio(User Interface). The chatbot answers employee queries based on Nestle HR policy documents ensuring accurate, context aware and hallucination reduced responses.

Architecture:
RAG Indexing Pipeline- Data loading, Chunking, Embeddings and storage of vector representations in ChromaDB
Retrieval pipeline- Retrieval(search user prompt embeddings with similarity search in the vector database), Augmentation(Agumenting the retrieved information with the user prompt along with custom prompt engineering and feed it as input to LLM), Response(LLM response generation)
Gradio User Interface- Creation of a function to fetch the data, creation of prompt and response generation

User Query-->Embedding-->Vector Search-->Retrieved Chunks-->Augmentation with custom prompt engineering-->LLM-->Response

Tech Stack:
Python
Langchain
ChromaDB
Custom Prompt Engineering
ChatOpenAI 
Gradio
