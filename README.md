<h1 align="center">Hi <img src="https://github.com/yosefshatila00/yosefshatila/blob/main/icons/Hi.gif" width="28px"/>, I'm yosef shatila</h1>
<h2 align="center">
  <img src="https://komarev.com/ghpvc/?username=[yosefshatila00]&color=dc143c&style=for-the-badge" alt="Profile Views" style="height:21px;">
  Fullstack Developer
  <a href="https://github.com/yosefshatila00">
    <img src="https://img.shields.io/badge/Portfolio-543DE0?style=for-the-badge&logo=About.me&logoColor=white" alt="Portfolio" style="height:22px;">
  </a>
</h2>
<div align="center">
 <img alt="GIF" src="https://media4.giphy.com/media/11KzOet1ElBDz2/giphy.gif?cid=6c09b952ufa3xxbbm0mpuadm2zaik3wjp4m9luz2ly0lyz8d&ep=v1_internal_gif_by_id&rid=giphy.gif&ct=g" />
</div>

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


loom video: https://www.loom.com/share/2f26decc98a140ef81787f0a28dee484

<details>
  <summary><h2> <img align="center" src="https://github.com/[yosefshatila00]/[yosefshatila]/blob/main/icons/stats.gif" width="32"/> Stats</h2></summary>
  <div align="center">
    ![](https://github-readme-stats.vercel.app/api?username=[yosefshatila00]&theme=tokyonight&hide_border=false&include_all_commits=true&count_private=false)<br/>
    ![](https://github-readme-streak-stats.herokuapp.com/?user=[yosefshatila00]&theme=tokyonight&hide_border=false)<br/>
    ![](https://github-readme-stats.vercel.app/api/top-langs/?username=[YourUsername]&theme=tokyonight&hide_border=false&include_all_commits=true&count_private=false&layout=compact)<br/>
    ![](https://github-readme-activity-graph.vercel.app/graph?username=[yosefshatila00]&theme=tokyo-night)
  </div>
</details>
