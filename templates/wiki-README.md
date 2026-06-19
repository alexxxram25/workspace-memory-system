# {{Your Name}} — LLM Wiki

A personal, LLM-maintained knowledge base built on [Andrej Karpathy's LLM Wiki pattern](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f).

**The idea:** instead of re-reading raw documents every time you ask a question (RAG), an LLM reads each source *once* and files it into a persistent, cross-linked wiki. Knowledge **compounds** — the cross-references, contradictions, and synthesis are already there and stay current. You curate and ask; the LLM does the reading, summarizing, and bookkeeping.

## How to use it
1. **Add a source** — drop a file into the relevant domain's `raw/` folder.
2. **Ingest** — tell your LLM agent "ingest this." It summarizes, files, cross-links, and logs.
3. **Ask** — query the wiki; good answers get filed back as new pages so explorations compound.
4. **Lint** — occasionally ask for a health-check (contradictions, stale claims, orphans, gaps).

## Layout
- `CLAUDE.md` — the **schema** (how the wiki works; the LLM reads this first).
- `index.md` — master catalog of everything.
- `log.md` — timeline of every ingest / query / lint.
- Domain folders (your work areas + a `General` catch-all), each with its own `index.md` and a `raw/` folder for sources.

Open the folder in **Obsidian** for the best experience (graph view, backlinks), or just browse the markdown directly. Nothing here requires any software to start.
