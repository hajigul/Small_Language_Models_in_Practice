# Small Language Models in Practice
### by Haji Gul

A compact, code-first book on building, fine-tuning, retrieving, quantizing, and
deploying small language models on your own hardware — plus matching Jupyter
lecture notes and the full LaTeX source.

## What's inside
```
Small_Language_Models_in_Practice/
├── Small_Language_Models_in_Practice_Haji_Gul.pdf   ← the finished book (read this)
├── LaTeX_Source/                                    ← rebuild or edit the book
│   ├── main.tex, slmstyle.sty, make_notes.py
│   ├── chapters/00_preface.tex … 08_capstone.tex
│   └── README.md  (build instructions)
└── Lecture_Notes/                                   ← run the code as you read
    ├── 00_Index.ipynb
    ├── Chapter_01 … Chapter_08 (.ipynb)
    └── README.md
```

## The 8 chapters
1. Why Small Language Models
2. Running Models Locally (transformers + Ollama)
3. Fine-Tuning with LoRA
4. Retrieval-Augmented Generation (LanceDB)
5. Agents and Tool Use
6. Quantization for Small Hardware (bitsandbytes, GGUF)
7. Serving and Deployment (FastAPI, streaming, vLLM)
8. Capstone: a full local document assistant tying it all together

## How to use it
- **Read** the PDF.
- **Run** the matching notebook in `Lecture_Notes/` alongside each chapter.
- **Rebuild/edit** via `LaTeX_Source/` (`pdflatex main.tex`, run twice).

Model and dataset IDs refer to public hubs and may change over time; verify
current names before running. For personal/educational use.
