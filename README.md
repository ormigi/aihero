# 🧠 AIHero – GitHub Project Reader

This mini project builds an **AI-ready data ingestion script** that downloads and parses Markdown files from any public GitHub repository.  
It’s part of the 7-day AI Agent course by Alexey Grigorev — *Day 1: Ingest and Index Your Data*.

---

## 🚀 Features
- Fetches a full GitHub repository (using the `codeload` API).
- Extracts and parses all `.md` / `.mdx` files.
- Uses [`python-frontmatter`](https://github.com/eyeseast/python-frontmatter) to read metadata and content.
- Returns a clean Python list I can later use for **search, embeddings, or AI agent training.**

---

## 🧩 How It Works
1. Downloads the repo as a ZIP file using `requests`.
2. Opens it in memory with `zipfile`.
3. Loops through files and extracts Markdown content.
4. Stores each file’s metadata and text in a structured dictionary.

---

## 🧰 Requirements
Install dependencies (using `uv` or `pip`):

```bash
uv add requests python-frontmatter
# or
pip install requests python-frontmatter
