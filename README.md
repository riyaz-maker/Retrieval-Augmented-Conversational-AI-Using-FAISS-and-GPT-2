
# Retrieval-Augmented Conversational AI Using FAISS and GPT-2

This project implements an AI-driven chatbot using a **FAISS-based search engine** for document retrieval, integrated with **GPT-2** for generating natural language responses. The system leverages retrieval-augmented generation (RAG) to enhance conversational capabilities by providing relevant, context-aware responses from a large document dataset (Wikipedia).

## Features
- **FAISS-powered document retrieval**: Efficient similarity search across large text datasets.
- **GPT-2 response generation**: Coherent and contextually relevant responses based on retrieved documents.
- **SentenceTransformer embeddings**: High-quality sentence embeddings for accurate document retrieval.
- Fine-tuned generation parameters for diverse, meaningful responses.

## How It Works
1. The query is encoded into an embedding using **SentenceTransformer**.
2. FAISS performs a similarity search against pre-indexed document embeddings to retrieve relevant documents.
3. The retrieved documents are combined with the user query and passed to **GPT-2**, which generates a context-aware response.

## Setup & Installation

### Requirements
Clone the repository:
```bash
git clone https://github.com/yourusername/faiss-gpt2-chatbot.git
cd faiss-gpt2-chatbot
```

Install dependencies:
```bash
pip install -r requirements.txt
```

### Usage
To run the chatbot:
```bash
python chatbot.py
```

Sample query:
```bash
> User: Tell me about Fyodor Dostoevsky.
> Bot: Fyodor Dostoevsky was a Russian novelist best known for works such as "Crime and Punishment" and "The Brothers Karamazov"...
```

## Example Outputs
Here’s an example of a query and response:
- **Query**: "Tell me about natural language processing."
- **Response**: "Natural Language Processing (NLP) is a field of artificial intelligence focused on the interaction between computers and humans using natural language..."

## Technologies Used
- **FAISS**: Facebook AI Similarity Search for document indexing and retrieval.
- **GPT-2**: OpenAI's pre-trained language model for text generation.
- **SentenceTransformer**: A BERT-based model to generate embeddings for document similarity search.
- **PyTorch**: Framework for deep learning and model training.

## License
This project is licensed under the MIT License.
