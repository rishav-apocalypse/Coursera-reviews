## Project Summary: AI-Powered Query Assistant with Web Scraping, RAG, and Gemini Integration

This project is a AI-powered query assistant that combines **automated web scraping**, **Retrieval-Augmented Generation (RAG)**, and **LLM integration (Gemini)** to deliver intelligent, summarized answers from unstructured data.
---
## 🔧 Installation

Install the required dependencies using pip:
-pip install langchain
-pip install openai  # or pip install google-generativeai for Gemini
-pip install faiss-cpu  # or pip install lancedb
-pip install tiktoken
-pip install python-dotenv
-in your project terminal -> bash -> playwright install 
# Optional
-pip install pydantic
-pip install fastapi
-pip install uvicorn
---
### @ Key Components:

- **Web Scraping with Playwright**  
  Dynamically scrapes user reviews from Coursera using Playwright to handle JavaScript-rendered content across multiple paginated pages, storing raw textual data for processing.

- **Vector Database with LanceDB**  
  The scraped reviews are cleaned, split using `RecursiveCharacterTextSplitter`, embedded, and stored in LanceDB—a lightweight and fast vector store for semantic search.

- **Query Processing and RAG Pipeline**  
  User queries are embedded and semantically matched with relevant documents from LanceDB. The retrieved documents are used as contextual grounding for a Retrieval-Augmented Generation (RAG) pipeline.

- **Gemini LLM Integration**  
  Google’s Gemini LLM processes the query along with the retrieved context to generate high-quality, context-aware summaries or responses.
  ---
 ## 🗒️ Developer Note

LangChain proved to be exceptionally powerful and more robust compared to Agno.  
Its documentation was well-structured and easy to navigate, which significantly streamlined the development process.

Despite being more complex than Agno, LangChain offered a more engaging and rewarding experience.  
The modularity and flexibility of its components allowed for smooth integration between various parts of the RAG pipeline.

Each library within the LangChain ecosystem was cohesively designed, enabling seamless cross-communication and making the entire development workflow more intuitive and efficient.

