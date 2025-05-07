# Coursera-reviews
This project is a full-stack AI-powered query assistant that combines automated web scraping, Retrieval-Augmented Generation (RAG), and LLM integration (Gemini) to deliver intelligent, summarized answers from unstructured data.

Key Components:
Web Scraping with Playwright:
Dynamically scrapes user reviews from Coursera using Playwright to handle JavaScript-rendered content across multiple paginated pages, storing raw textual data for processing.
Vector Database with LanceDB:
The scraped reviews are cleaned, split using RecursiveCharacterTextSplitter, embedded, and stored in LanceDB—a lightweight and fast vector store for semantic search.
Query Processing and RAG Pipeline:
User queries are embedded and semantically matched with relevant documents from LanceDB.
The retrieved documents are used as contextual grounding for a Retrieval-Augmented Generation (RAG) pipeline.
Gemini LLM Integration:
Google’s Gemini LLM processes the query along with the retrieved context to generate high-quality, context-aware summaries or responses.
