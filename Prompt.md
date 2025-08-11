# ReAct (Reasoning + Acting)
A framework where a language model interleaves reasoning steps with actions (like querying a knowledge source, searching, or calling APIs) in a single process.

For example:

Thought: “I need to check the weather.”

Action: Calls a weather API or retrieves info.

Interaction: Dynamic, step-by-step problem-solving

# RAG (Retrieval-Augmented Generation)
A method that combines retrieval from a large document/database with a generative model to produce more accurate and fact-based outputs.

1. The input query is used to retrieve relevant documents or passages from a large corpus (using a retriever like dense embeddings or BM25).
2. These retrieved documents are fed into a generator model (like a transformer) that conditions its answer on the retrieved content.
3. The model generates the answer based on both the query and retrieved knowledge.

Interaction: Retrieval happens before generation
