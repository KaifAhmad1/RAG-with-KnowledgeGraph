# Retrieval Augmented Generation with LangChain and Neo4J Graph DB
Project: Enhanced Question Answering Integrating Unstructured and Graph Knowledge using Neo4j and LangChain.

Description: Implementation of a sophisticated question-answering system, combining Neo4j and LangChain. The process focuses on integrating unstructured data and graph knowledge to enhance response generation using Mistral-7b.

Installation: Python dependencies are installed using pip. Additional dependencies include LangChain, OpenAI, Wikipedia, Tiktoken, Neo4j, and Transformers. The SageMaker library is also updated.

Neo4j Vector Index: Requisite libraries and modules are imported to set up the Neo4j Vector Index. Environment variables are securely loaded using dotenv.

Data Preparation: The code selects a Wikipedia page about Leonhard Euler, uses the "bert-base-uncased" model for text tokenization, and loads the raw content. Text is chunked into smaller pieces using RecursiveCharacterTextSplitter to maintain context.

Neo4j Vector Indexing: The chunked documents are converted into the Neo4j vector index, combining Neo4j graph database and OpenAI embeddings.

Vector Similarity Search: A sample user query ("Who were the siblings of Leonhard Euler?") is used to perform vector similarity search, and the top 2 most similar documents are retrieved and printed.

Knowledge Graph: An open-source project, inspired by the NaLLM project, is used to construct a knowledge graph from unstructured data.

Neo4j DB QA Chain: Necessary libraries are imported to set up the Neo4j Database QA Chain. A Neo4jGraph instance is created, connected to the Neo4j database, and its schema is visualized.

Question Answering Chain: The GraphCypherQAChain abstracts details and generates a natural language response for a natural language question (NLQ). It uses LLMs to generate a Cypher query, retrieves graph results from the database, and generates a final natural language response.

Result: The code demonstrates how to generate a response to the question "Who were the siblings of Leonhard Euler?" from the knowledge graph.



