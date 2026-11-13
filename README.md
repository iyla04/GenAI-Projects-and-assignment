# RAG-TASKS

Step-by-step Retrieval-Augmented Generation (RAG) notebooks by [@iyla04](https://github.com/iyla04).

```
Load -> Chunk -> Embed -> Store -> Retrieve -> Augment -> Generate -> Evaluate
```

## Notebooks

| Step | Notebook | What it covers |
|------|----------|----------------|
| 1 | `RAG_Step1_Document_Loading_and_Chunking.ipynb` | Loading text/PDF, fixed and recursive chunking, metadata |
| 2 | `RAG_Step2_Embeddings_and_Vector_Store.ipynb` | Sentence embeddings, storing chunks in ChromaDB |
| 3 | `RAG_Step3_Retrieval_and_Similarity_Search.ipynb` | Top-k search, metadata filters, thresholds, MMR |
| 4 | `RAG_Step4_Prompt_Augmentation.ipynb` | Prompt templates, citations, context budget |
| 5 | `RAG_Step5_Generation_End_to_End_Pipeline.ipynb` | Full pipeline with a local LLM, RAG vs no RAG |
| 6 | `RAG_Step6_Evaluation.ipynb` | Hit rate, MRR, faithfulness checks |

Run them in order: each step builds on files created by the previous one (`chunks.json`, `chroma_store/`).

## Getting started

```bash
git clone https://github.com/iyla04/RAG-TASKS.git
cd RAG-TASKS
pip install -r requirements.txt
jupyter notebook
```

Each notebook also installs its own dependencies in the first cell, so they run in Google Colab as-is.

## Roadmap

- [ ] Hybrid search (BM25 + vectors)
- [ ] Re-ranking with a cross-encoder
- [ ] RAG over your own PDFs
