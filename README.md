# Deadlock Wiki — NotebookLM Knowledge Base

A pre-built, AI-optimized knowledge base scraped from [deadlock.wiki](https://deadlock.wiki/), ready to load directly into **Google NotebookLM** or any other LLM tool.

No coding required. Download and import.

---

##  Open in NotebookLM

**[Open the Notebook](https://notebooklm.google.com/notebook/84d89a11-d1f9-437b-ae7a-570d6dfe7322)**

Already configured with all sources loaded. Just open and start asking.

---

##  What's Inside

| Path | Contents |
| --- | --- |
| `for_notebooklm/deadlock_wiki_english_part1–4.md` | Full wiki split into ~400k word chunks (within NotebookLM's 500k limit) |
| `for_notebooklm/deadlock_wiki_explanation.md` | AI decypher key — Spirit Scaling, upgrade tiers, stat growth |
| `for_notebooklm/README4MEATBAGS.md` | User guide with example prompts |
| `wiki_pages_en/*.md` | 826 individual article files (browseable) |

**Knowledge cutoff**: May 22, 2026 — all heroes up to and including *Apollo*.

---

##  Load Into Your Own Notebook

If you want your own private copy:

1. Go to [notebooklm.google.com](https://notebooklm.google.com/) and create a new notebook.
2. Click **Add Source → Upload Files**.
3. Upload in this order:
   - `for_notebooklm/deadlock_wiki_explanation.md` ← **first**
   - `for_notebooklm/deadlock_wiki_english_part1.md`
   - `for_notebooklm/deadlock_wiki_english_part2.md`
   - `for_notebooklm/deadlock_wiki_english_part3.md`
   - `for_notebooklm/deadlock_wiki_english_part4.md`

> The `deadlock_wiki_explanation.md` file teaches the AI how to read Spirit Power scaling values, upgrade tier costs, and per-level stat growth. Upload it first.

---

##  Multilingual

Source files are in English, but NotebookLM is fully multilingual — ask in **Russian**, **English**, or any other language.

---

##  Updates & Contribution

This knowledge base will be updated with new patches and community proposals. To suggest improvements or report issues:

*   **GitHub**: [IDemmoI](https://github.com/IDemmoI)

Want to generate a fresh dump for a different wiki? The scraper is open-source and works with **any MediaWiki site**:

**[IDemmoI/mediawiki-to-notebooklm](https://github.com/IDemmoI/mediawiki-to-notebooklm)**

---

##  Legality & Licensing

All content belongs to [deadlock.wiki](https://deadlock.wiki/) contributors and is licensed under **Creative Commons Attribution-ShareAlike (CC BY-SA)**. Data is fetched via the official public MediaWiki API with polite rate limits.

---

##  Credits

*   **Concept, Pipeline Architecture & AI Decypher Framework**: [IDemmoI](https://github.com/IDemmoI)
*   **Code Implementation**: vibesloped by [IDemmoI](https://github.com/IDemmoI)
