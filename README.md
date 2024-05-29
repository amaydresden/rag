# rag
everything I doc about RAG

Eigenschaften beim erstellen der Daten für die VectorDatenbank / und die Weiterleitung
---
Max Context Snippets
This setting controls the maximum amount of context snippets the will be sent to the LLM for per chat or query.
Recommended: 4
---
Document similarity threshold
The minimum similarity score required for a source to be considered related to the chat. The higher the number, the more similar the source must be to the chat.
---
Context Prompt
The prompt that will be used on this workspace. Define the context and instructions for the AI to generate a response. 
You should to provide a carefully crafted prompt so the AI can generate a relevant and accurate response.
EXAMPLES
---> "Given the following conversation, relevant context, and a follow up question, reply with an answer to the current question the user is asking. 
Return only your response to the question given the above information following the users instructions as needed."
OR
--> "Use the following pieces of context to answer the question at the end.
    If you don't know the answer, just say that you don't know, don't try to make up an answer.
    Use three sentences maximum and keep the answer as concise as possible."
---
Text Embedding
Embedding is the process of turning text into vectors. These credentials are required to turn your files and prompts into a format which AnythingLLM can use to process.
---
Prompt Format
Related to the LLM  - every LLM has its own format how to set a prompt
https://lib.rs/crates/chat-prompts
EXAMPLE / codellama
[INST] Write code to solve the following coding problem that obeys the constraints and passes the example test cases. Please wrap your code answer using ```:
{prompt}
[/INST]
---
Text splitting & Chunking Preferences
Text Chunk Size
This is the maximum length of characters that can be present in a single vector.
Text Chunk Overlap
This is the maximum overlap of characters that occurs during chunking between two adjacent text chunks.
---
transformer models (or Embedding modell?)
This is a sentence-transformers model: It maps sentences & paragraphs to a 768 dimensional dense vector space and can be used for tasks like clustering or semantic search.
EXAMPLE: sentence-transformers/all-mpnet-base-v2
---
Database Query
Similarity (searchword/token similar to db-token)
Contexts / Search Results : 


