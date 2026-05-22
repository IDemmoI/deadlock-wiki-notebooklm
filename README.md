# Deadlock Wiki — NotebookLM Knowledge Base

A pre-built, AI-optimized knowledge base scraped from the official [deadlock.wiki](https://deadlock.wiki/), ready to be loaded directly into **Google NotebookLM** (or any other LLM tool that accepts documents).

No coding required. Just download and upload to your notebook.

---

##  What's Inside

```
for_notebooklm/
├── deadlock_wiki_english_part1.md   (~400k words)
├── deadlock_wiki_english_part2.md   (~393k words)
├── deadlock_wiki_english_part3.md   (~399k words)
├── deadlock_wiki_english_part4.md   (~301k words)
├── deadlock_wiki_explanation.md     AI decypher key — Spirit Scaling, upgrade tiers, stat growth
└── README4MEATBAGS.md               User guide for notebook users

wiki_pages_en/
└── *.md                             826 individual article files (browseable)
```

**Knowledge cutoff**: May 22, 2026 — includes all heroes up to and including *Apollo*.

---

##  How to Load into NotebookLM

1. Go to [notebooklm.google.com](https://notebooklm.google.com/) and create a new notebook.
2. Click **Add Source → Upload Files**.
3. Upload in this order:
   - `for_notebooklm/deadlock_wiki_explanation.md` ← **upload first**
   - `for_notebooklm/deadlock_wiki_english_part1.md`
   - `for_notebooklm/deadlock_wiki_english_part2.md`
   - `for_notebooklm/deadlock_wiki_english_part3.md`
   - `for_notebooklm/deadlock_wiki_english_part4.md`
4. Done. Ask anything.

> The `deadlock_wiki_explanation.md` file teaches the AI how to read Spirit Power scaling values, upgrade tier costs, and per-level stat growth from the wiki format. Without it, the AI may misread some numbers.

---

##  Multilingual

Source files are in English, but NotebookLM is fully multilingual — ask your questions in **Russian**, **English**, or any other language.

---

##  Want to Generate a Fresh Dump?

The scraper script that generated these files is open-source and works with **any MediaWiki wiki** — just change one line:

👉 [IDemmoI/mediawiki-to-notebooklm](https://github.com/IDemmoI) *(link TBD)*

---

##  License & Credits

All wiki content belongs to [deadlock.wiki](https://deadlock.wiki/) contributors and is licensed under **Creative Commons Attribution-ShareAlike (CC BY-SA)**.

*   **Pipeline & AI Decypher Framework**: [IDemmoI](https://github.com/IDemmoI)
*   **Technical Implementation**: vibesloped by [IDemmoI](https://github.com/IDemmoI)
