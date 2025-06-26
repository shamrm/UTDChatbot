# 🤖 UTDChatbot

A conversational AI chatbot for the University of Texas at Dallas (UTD).  
It scrapes official site data and uses Retrieval-Augmented Generation (RAG) with OpenAI, LangChain, and FAISS to answer questions from students, faculty, and staff.
🔗 https://github.com/Arjun-Madhusoodanan/UtdChatBot

## 🔧 Tech Stack
- Python
- LangChain
- OpenAI GPT-4
- FAISS
- Web Scraping (BeautifulSoup)
- CLI Interface

## 💡 Features
- Real-time query answering using scraped UTD data
- Document chunking with `RecursiveCharacterTextSplitter`
- Fast vector search using FAISS

## Process
- Web Scraping: Used Python to scrape data across multiple sitemaps and nested links
- Preprocessing: Cleaned the data to format non-ascii characters 
- Embedding: Used RecursiveCharacterTextSplitter and stored their embeddings in FAISS for efficient vector based similarity search
- RAG Pipeline: connected LangChain with OpenAI’s GPT-4 to build RetrievalQA pipeline
- Memory: Used LangChain’s memory module to implement conversation awareness


