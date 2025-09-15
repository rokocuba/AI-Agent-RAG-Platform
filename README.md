# AI Agent Factory: Intelligent Document Processing Platform (Internship Project Showcase)

This repository serves as a detailed showcase of the comprehensive AI Agent and Retrieval-Augmented Generation (RAG) platform I co-developed during my summer 2025 internship at Abysalto. The platform is designed to create, configure, and deploy specialized AI agents capable of intelligent document processing and complex reasoning.

**Note:** The source code for this project is proprietary to Abysalto and cannot be shared publicly. This repository serves as a detailed portfolio piece to document the project's architecture, my technical contributions, and the results achieved.

---

### My Role & Key Contributions

As an AI Academy Intern, I was deeply involved in the entire development lifecycle. I played an integral role in architectural design and hands-on implementation, focusing on building a system that was not just functional but also scalable, reliable, and extensible.

*   **System Architecture:** I took a leading role in key architectural decisions, championing the use of the **Strategy design pattern** to create a modular system. This allowed for pluggable components for RAG methods, document chunking, and evaluation, which accelerated our experimentation cycles by **3x**.
*   **RAG System Implementation:** I designed and implemented an extensible Retrieval-Augmented Generation (RAG) system, developing several of the nine specialized retrieval methods. This core system achieved **95%+ retrieval precision** in our internal testing benchmarks.
*   **API & Microservices:** I developed robust microservices using Python and FastAPI, creating over 50 RESTful endpoints for comprehensive system control, from document ingestion to agent interaction.
*   **Database Optimization:** I optimized PostgreSQL queries and designed dynamic table generation logic that automatically adapted to different embedding model dimensions, ensuring efficient vector operations with `pgvector`.

---

### Technical Deep Dive: Core Features

The platform was built with a focus on modern software architecture and cutting-edge AI techniques.

#### 1. Scalable Microservices Architecture
The system was designed using a clean, multi-layered architecture to ensure a clear separation of concerns.

*   **Service Layer Pattern:** Abstracted all business logic from data persistence, enabling reliable and testable operations.
*   **Strategy Design Pattern:** Implemented across four core domains (Embedding Models, Chunking Methods, RAG Methods, and Evaluation Strategies), allowing for runtime selection and easy A/B testing of different approaches without core system modifications.
*   **Project-Based Multi-Tenancy:** Ensured that resources, configurations, and data were securely isolated between different projects and agents.

#### 2. Advanced Retrieval-Augmented Generation (RAG) System
The platform featured a sophisticated RAG system with nine distinct retrieval strategies, allowing users to select the optimal method for their specific use case.

*   **Multi-Vector Embeddings:** We stored separate embeddings for document content, generated summaries, and potential questions, enabling more nuanced and accurate semantic search.
*   **Specialized Retrieval Methods:** Included strategies like `Multi-Query RAG` (using LLMs for query expansion), `Hybrid Meta RAG` (combining semantic search with keyword filtering), and `Graph-Walk RAG` (exploring relationships between document chunks).

#### 3. Intelligent Document Processing Pipeline
The system automated the transformation of raw documents into a queryable knowledge base.

*   **Multi-Format Support:** Handled PDF, DOCX, and TXT files with automatic content extraction.
*   **Sophisticated Chunking:** Implemented five advanced chunking algorithms, including `Semantic Chunking` (using embedding models to find logical breaks) and `Chunking by Title`, to preserve the contextual integrity of the source documents.

---

### Tech Stack

*   **Backend:** Python, FastAPI
*   **AI/ML:** LangChain, LangGraph, OpenAI API
*   **Database:** PostgreSQL with pgvector extension
*   **Infrastructure:** Docker
