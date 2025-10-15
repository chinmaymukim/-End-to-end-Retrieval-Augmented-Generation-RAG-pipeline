# Retrieval-Augmented Generation (RAG) Pipeline Chatbot

## Project Overview 🚀
This repository contains the complete codebase for a **Retrieval-Augmented Generation (RAG) Pipeline** application. This project demonstrates the full lifecycle of building a robust, grounded, and scalable Generative AI solution, moving beyond simple API calls to constructing a full-stack, context-aware system. The final deliverable is an interactive chatbot interface built with Streamlit.

**My Role:** I personally engineered and implemented all components of this RAG architecture, focusing on reliability and modularity.

## Key Features & Technical Stack
The pipeline is designed around best-in-class open-source libraries to manage data, vectorization, LLM orchestration, and the user interface.

| Category | Tool / Library | Purpose |
| :--- | :--- | :--- |
| **Orchestration** | **LangChain** / **LangGraph** | Building complex, state-aware agentic workflows for advanced conversational logic. |
| **Vector Database** | **ChromaDB** | High-performance, persistent storage for vector embeddings (the project's knowledge base). |
| **Data Handling** | `WebBaseLoader` | Ingesting and retrieving unstructured data (web scraping). |
| **Preprocessing** | `RecursiveCharacterTextSplitter` | Implementing an optimized chunking strategy for better retrieval accuracy. |
| **Embeddings** | `OpenAIEmbeddings` | Generating high-quality vector representations of the documents. |
| **Frontend** | **Streamlit** | Creating the interactive, user-friendly web interface for deployment. |

## Architecture & Workflow
The application follows the standard RAG paradigm:

1.  **Ingestion:** Data is loaded and split into optimized chunks.
2.  **Indexing:** Chunks are vectorized and indexed in ChromaDB.
3.  **Retrieval:** The user query is embedded and used to fetch the most relevant document chunks from ChromaDB.
4.  **Generation:** The retrieved context and the user's query are passed to the LLM (via LangChain) to generate a grounded, accurate response.

## Installation & Setup

1.  **Clone the repository:**
    ```bash
    git clone [YOUR_REPO_URL]
    cd [YOUR_REPO_NAME]
    ```

2.  **Create a virtual environment (recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3.  **Install dependencies:**
    *(Assuming you have a `requirements.txt` based on the provided code snippets)*
    ```bash
    pip install -r requirements.txt
    ```

4.  **Set Environment Variables:**
    Create a file named `.env` in the root directory and add your keys.
    ```
    OPENAI_API_KEY="YOUR_API_KEY_HERE"
    ```

5.  **Run the application:**
    ```bash
    streamlit run app.py
    ```

## Project Efforts & Accomplishments
This project validates my skills in moving beyond basic LLM prompt engineering and successfully taking a Generative AI application through its entire development cycle.

* Successfully implemented **LangGraph** to manage complex, stateful conversational memory and logic.
* Achieved high retrieval accuracy through careful tuning of the text chunking strategy.
* Demonstrated proficiency in full-stack AI development by deploying the model via a **Streamlit** interface.
