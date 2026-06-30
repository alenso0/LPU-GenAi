<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&amp;color=0:6366F1,100:22D3EE&amp;height=180&amp;section=header&amp;text=LPU%20GenAI&amp;fontSize=46&amp;fontColor=ffffff&amp;animation=fadeIn&amp;fontAlignY=35&amp;desc=Notes%20%2B%20notebooks%20%2B%20transcripts&amp;descAlignY=58&amp;descSize=18" />
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&amp;size=18&amp;pause=1000&amp;color=22D3EE&amp;center=true&amp;vCenter=true&amp;width=480&amp;lines=GenAI+transcripts+%3B%29;Notes+auto-synced+as+PDFs;Mon-Fri+10%3A00+%2B+16%3A00+IST" alt="typing animation" />
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
| `requirements.txt` | Python dependencies |

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

---

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&amp;color=0:22D3EE,100:6366F1&amp;height=100&amp;section=footer" />
</p>
