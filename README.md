# Small Language Models in Practice — Lecture Notes

Jupyter notebook companion to the book **_Small Language Models in Practice_** by
**Haji Gul**. One notebook per chapter, in book order, **code-first** with short
markdown notes between cells.

## Contents
- `00_Index.ipynb` — clickable overview and reading order
- `Chapter_01` … `Chapter_08` — one notebook per chapter

## Chapters
1. **Why Small Language Models** — when small beats large; the local stack; first generation.
2. **Running Models Locally** — transformers vs. Ollama; tokenization; sampling; streaming.
3. **Fine-Tuning with LoRA** — data prep, adapters, training, saving/reusing the adapter.
4. **Retrieval-Augmented Generation** — chunk, embed, LanceDB, retrieve, grounded answers.
5. **Agents and Tool Use** — the tool-calling loop from scratch, then with smolagents.
6. **Quantization for Small Hardware** — 4-bit with bitsandbytes; GGUF for llama.cpp/Ollama.
7. **Serving and Deployment** — FastAPI endpoint with streaming; Ollama OpenAI-compatible API.
8. **Capstone** — quantized model + RAG + tools + serving in one local document assistant.

## Getting started
```bash
pip install jupyterlab
jupyter lab        # open 00_Index.ipynb first
```

Base environment used across chapters:
```bash
pip install transformers datasets accelerate torch
pip install peft bitsandbytes               # ch 3, 6
pip install lancedb sentence-transformers   # ch 4, 8
pip install smolagents                       # ch 5
pip install fastapi uvicorn openai           # ch 7, 8
```

## Notes
- Run chapters in order the first time — later notebooks reuse earlier concepts.
- Model and dataset IDs on the Hugging Face Hub drift; verify before running.
- Heavy cells (fine-tuning, 4-bit loading, serving) may need a GPU and large downloads.
- These notebooks mirror the book's code listings exactly so you can run as you read.
