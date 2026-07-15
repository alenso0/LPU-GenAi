<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&amp;color=0:6366F1,100:22D3EE&amp;height=180&amp;section=header&amp;text=LPU%20GenAI&amp;fontSize=46&amp;fontColor=ffffff&amp;animation=fadeIn&amp;fontAlignY=35&amp;desc=Notes%20%2B%20notebooks%20%2B%20transcripts&amp;descAlignY=58&amp;descSize=18" />
</p>


<p align="center">
  <img src="https://github.com/alenso0/LPU-GenAi/actions/workflows/sync-notes.yml/badge.svg" alt="Notes sync status" />
  <img src="https://img.shields.io/badge/python-3.11-blue?logo=python&amp;logoColor=white" />
  <img src="https://img.shields.io/badge/notes-auto--synced-22D3EE" />
</p>

---

## What's in here

| Path | Description |
|---|---|
| `Notes/` | Course notes, auto-synced as PDFs (see below) |
| `NLP/` | Natural Language Processing basics — SMS spam classification, GloVe embeddings |
| `NN/` | Neural network fundamentals — perceptron, ANN, CNN, RNN, from-scratch implementations |
| `GEN-AI/` | Generative AI notebooks — BERT, diffusion models, RAG (LangChain + from-scratch with Ollama) |
| `OLLAMA_APP/` | Standalone Python project scaffold for an Ollama-based app (uv-managed) |
| `scripts/` | Automation scripts (e.g. `sync_notes.py` for the Notes auto-sync below) |
| `requirements.txt` | Python dependencies |

Folders with their own setup steps or extra data files have their own `README.md` — see [`NLP/README.md`](NLP/README.md), [`GEN-AI/README.md`](GEN-AI/README.md), and [`OLLAMA_APP/README.md`](OLLAMA_APP/README.md).

## Notes auto-sync

`Notes/` is kept in sync with [v0idgy/LPU_GenAI](https://github.com/v0idgy/LPU_GenAI)'s `Notes/` folder by [`.github/workflows/sync-notes.yml`](.github/workflows/sync-notes.yml):

- Runs **Mon–Fri at 10:00 and 16:00 IST**, plus on-demand via `workflow_dispatch`
- Pulls any new or changed file from the source repo
- Converts anything that isn't already a PDF (images, Office docs, text) into one
- Commits only when content actually changed, authored by **NotBOT**
- Stops running after **2026-07-31** and disables itself

The sync logic lives in [`scripts/sync_notes.py`](scripts/sync_notes.py).

## Setup

```bash
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
jupyter notebook
```

## Privacy & secrets

This repo is a public collection of coursework notebooks — no real API keys, credentials, or personal data should ever be committed.


---

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&amp;color=0:22D3EE,100:6366F1&amp;height=100&amp;section=footer" />
</p>
