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

### What FAISS does not do
- ❌ No server
- ❌ No persistence (unless you manage it)
- ❌ No metadata filtering
- ❌ No CRUD semantics
- ❌ No auth / scaling / replication

```
index = faiss.IndexHNSWFlat(384, 32)
index.add(embeddings)
scores, ids = index.search(query, k=10)
```


## Qdrant
- Full vector database
- Runs as a server
- Built on HNSW
- Stores vectors + payloads (metadata)

### What Qdrant gives you
- ✅ REST & gRPC API
- ✅ Disk persistence
- ✅ Filtering (price < 50, brand = apple)
- ✅ Hybrid search (vector + filters)
- ✅ Sharding & replication
- ✅ Versioned updates
- ✅ Production-ready

| If you want…                                        | Choose     |
| --------------------------------------------------- | ---------- |
| **Fast local ANN, simple setup**                    | **FAISS**  |
| **Production vector DB with filters & persistence** | **Qdrant** |
| **Offline indexing / research**                     | **FAISS**  |
| **Online semantic search service**                  | **Qdrant** |
| **Hybrid (vector + metadata) search**               | **Qdrant** |


