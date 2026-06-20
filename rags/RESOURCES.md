# RAG and GraphRAG Resources

## Knowledge

- [Paper: "Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks" - Lewis et al., NeurIPS 2020](https://arxiv.org/abs/2005.11401)
  Foundational RAG paper. Use for: why retrieval augments parametric model memory, provenance, updating knowledge, and the original dense-index formulation.
- [Paper: "From Local to Global: A Graph RAG Approach to Query-Focused Summarization" - Edge et al., 2024/2025](https://arxiv.org/abs/2404.16130)
  Primary GraphRAG paper from Microsoft Research. Use for: why global corpus questions differ from local retrieval questions, and how entity graphs plus community summaries help.
- [Microsoft GraphRAG Documentation](https://microsoft.github.io/graphrag/)
  Official implementation docs. Use for: GraphRAG indexing, query modes, global search, local search, DRIFT search, prompt tuning, and operational configuration.
- [LlamaIndex: Introduction to RAG](https://docs.llamaindex.ai/en/stable/understanding/rag/)
  Practical framework explanation of RAG stages. Use for: loading, indexing, storing, querying, evaluation, nodes/documents, retrievers, postprocessors, and response synthesis.
- [LlamaIndex: Loading Data (Ingestion)](https://docs.llamaindex.ai/en/stable/understanding/rag/loading/)
  Practical ingestion guide. Use for: documents, connectors/readers, transformations, chunking, metadata extraction, and embedding as an ingestion pipeline.
- [LlamaIndex: Indexing](https://docs.llamaindex.ai/en/stable/understanding/rag/indexing/)
  Practical indexing guide. Use for: vector store indexes, embeddings as semantic representations, top-k retrieval, and why indexing choices must match query strategy.
- [LlamaIndex: Querying](https://docs.llamaindex.ai/en/stable/understanding/rag/querying/)
  Practical querying guide. Use for: retrieval, postprocessing, response synthesis, retrievers, similarity cutoffs, and query engine composition.
- [LlamaIndex: Storing](https://docs.llamaindex.ai/en/stable/understanding/rag/storing/)
  Practical persistence guide. Use for: avoiding re-indexing cost, persisted indexes, vector stores, and incremental insertion.
- [LlamaIndex: Evaluation](https://docs.llamaindex.ai/en/stable/optimizing/evaluation/evaluation/)
  Practical evaluation overview. Use for: when to use end-to-end evaluation versus component-wise evaluation, and standard metrics such as precision, recall, F1, and exact match.
- [Paper: "Self-RAG: Learning to Retrieve, Generate, and Critique through Self-Reflection" - Asai et al., 2023](https://arxiv.org/abs/2310.11511)
  Advanced RAG variant. Use for: adaptive retrieval, reflection, critique, factuality, and citation accuracy after baseline mechanics are understood.
- [Weaviate Academy: Hands-on Weaviate with Python](https://weaviate.io/developers/academy/py/starter_text_data)
  Beginner-friendly vector database practice. Use for: semantic search, hybrid search, vector storage, and simple RAG implementation exercises.

## Wisdom (Communities)

- [Microsoft GraphRAG GitHub](https://github.com/microsoft/graphrag)
  High-signal project repository. Use for: implementation issues, release changes, practical limitations, and examples from real users.
- [LlamaIndex Discord](https://discord.com/invite/eN6D2HQ4aX)
  Active implementation community. Use for: debugging RAG pipelines, comparing retrieval strategies, and learning current framework patterns.
- [Weaviate Forum](https://forum.weaviate.io/)
  Vector database community. Use for: schema design, hybrid search, vector database operations, and performance troubleshooting.

## Gaps

- Need a later resource pass for graph databases, entity resolution, and knowledge graph quality evaluation.
- Need a later resource pass for production observability tools such as tracing, offline eval sets, and online feedback loops.
