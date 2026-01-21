An AI-powered Study Assistant that allows users to:
1. Ingest study notes
2. Ask questions using Retrieval-Augmented Generation (RAG)
3. Simplify notes for revision
4. Generate quizzes automatically


architecture overview:
User Notes
   ↓
Text Chunking
   ↓
Embeddings (MiniLM)
   ↓
Pinecone Index
   ↓
Retriever
   ↓
LLaMA 3.1 (Groq)
   ↓
Answer / Simplified Notes / Quiz


Features:
1. Notes Ingestion
Upload or paste notes, which are split into chunks, embedded, and stored in a vector database.
2. Question Answering (RAG)
Answers questions strictly based on the ingested notes using semantic search + LLM reasoning.
3. Notes Simplification
Converts complex notes into clear, easy-to-study bullet points.
4. Quiz Generation
Automatically generates multiple-choice questions from your notes.
5. Interactive UI
User-friendly Gradio interface with a sidebar layout.


How It Works
1. Chunking: Large notes are split into smaller chunks to improve retrieval accuracy and stay within LLM context limits.
2. Embeddings: Each chunk is converted into a numerical vector using a sentence-transformer model.
3. Indexing: Vectors are stored in a Pinecone index, enabling fast similarity search.
4. Retrieval-Augmented Generation (RAG):
-When a question is asked
-Relevant chunks are retrieved from Pinecone
-Only those chunks are passed to the LLM
-This reduces hallucination and improves accuracy



