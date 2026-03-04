# Crafting-an-AI-powered-HR-Assistant
This project is Retrieval Augmented Generation based AI assistant built using Langchain, ChromaDB, LLM(OpenAI) and Gradio(User Interface). The chatbot answers employee queries based on Nestle HR policy documents ensuring accurate, context aware and hallucination reduced responses.

Architecture:
1.RAG Indexing Pipeline- 
Data loading 
Chunking
Embeddings
ChromaDB for storage of vector embeddings

2.Retrieval pipeline- 
Retrieval(search user prompt embeddings with similarity search in the vector database)
Augmentation(Agumenting the retrieved information with the user prompt along with custom prompt engineering and feed it as input to LLM)
Response(LLM response generation)

3.Gradio User Interface- Creation of a function to fetch the data, creation of prompt and response generation

End-to-End flow:

User Query-->Embedding-->Vector Search-->Retrieved Chunks-->Augmentation with custom prompt engineering-->LLM-->Response

Tech Stack:

Python
Langchain
ChromaDB
Custom Prompt Engineering
ChatOpenAI 
Gradio
