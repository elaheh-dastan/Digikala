# Qdrant vs FAISS
- FAISS is a vector indexing library
- Qdrant is a vector database / search service

## FAISS
- C++ / Python library
- Focused purely on vector similarity search
- In-process (runs inside your app)

### What FAISS does extremely well
- Very fast ANN
- Many index types:
    - Flat
    - IVF
    - HNSW
    - PQ / OPQ

- GPU support
- Full control over memory & performance

| If you want…                                        | Choose     |
| --------------------------------------------------- | ---------- |
| **Fast local ANN, simple setup**                    | **FAISS**  |
| **Production vector DB with filters & persistence** | **Qdrant** |
| **Offline indexing / research**                     | **FAISS**  |
| **Online semantic search service**                  | **Qdrant** |
| **Hybrid (vector + metadata) search**               | **Qdrant** |


