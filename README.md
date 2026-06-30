<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:6366F1,100:22D3EE&height=180&section=header&text=LPU%20GenAI&fontSize=46&fontColor=ffffff&animation=fadeIn&fontAlignY=35&desc=Notes,%20notebooks%20%26%20transcripts&descAlignY=58&descSize=18" />
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=18&pause=1000&color=22D3EE&center=true&vCenter=true&width=480&lines=GenAI+transcripts+%3B);Notes+auto-synced+as+PDFs;Mon-Fri+%C2%B7+10%3A00+%26+16%3A00+IST" alt="typing animation" />
</p>

<p align="center">
  <img src="https://github.com/alenso0/LPU-GenAi/actions/workflows/sync-notes.yml/badge.svg" alt="Notes sync status" />
  <img src="https://img.shields.io/badge/python-3.11-blue?logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/notes-auto--synced-22D3EE" />
</p>

---

## What's in here

| Path | Description |
|---|---|
| `Notes/` | Course notes, auto-synced as PDFs (see below) |
| `perceptron.ipynb` | Perceptron implementation notebook |
| `perceptron_for_multiclass.ipynb` | Multiclass perceptron notebook |
| `requirements.txt` | Python dependencies |

## Notes auto-sync

`Notes/` is kept in sync with [v0idgy/LPU_GenAI](https://github.com/v0idgy/LPU_GenAI)'s `Notes/` folder by [`.github/workflows/sync-notes.yml`](.github/workflows/sync-notes.yml):

- Runs **Mon–Fri at 10:00 and 16:00 IST**, plus on-demand via `workflow_dispatch`
- Pulls any new or changed file from the source repo
- Converts anything that isn't already a PDF (images, Office docs, text) into one
- Commits only when content actually changed
- Stops running after **2026-07-31** and disables itself

The sync logic lives in [`scripts/sync_notes.py`](scripts/sync_notes.py).

## Setup

```bash
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
jupyter notebook
```

---

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:22D3EE,100:6366F1&height=100&section=footer" />
</p>
