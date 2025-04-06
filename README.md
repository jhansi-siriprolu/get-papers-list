# 🧬 get-papers-list

A command-line Python tool to fetch research papers from PubMed based on a user-specified query, identify papers with at least one **non-academic author affiliated with a pharmaceutical or biotech company**, and return the results as a CSV.

---

## 🚀 Features

- 🔍 **Query PubMed** using full query syntax
- 🧠 **Filter for pharma/biotech author affiliations**
- 📤 Export as CSV or display in console
- 🧪 Typed Python with clean, modular architecture
- 🛠️ Packaged using Poetry with CLI support via Typer

---

## 📦 Project Structure

```bash
get-papers-list/
├── cli.py                     # Entry-point CLI interface
├── pyproject.toml             # Poetry project config
├── get_papers/
│   ├── __init__.py
│   ├── fetch.py               # PubMed API interaction
│   ├── parse.py               # XML parsing & author filtering
│   ├── writer.py              # Output writing to file/console
│   ├── utils.py               # Affiliation classification heuristics
│   └── main.py                # Pipeline orchestrator
└── tests/
    ├── test_fetch.py
    ├── test_parse.py
    └── test_utils.py
