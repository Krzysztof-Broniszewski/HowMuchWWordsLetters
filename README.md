# Word & Letter Counter (Unicode / Polish-ready)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1aKILIO_mLZZXF6CHF4lZtZIDuh4nHzVg?usp=sharing)
<br>
**Direct link:** https://colab.research.google.com/drive/1aKILIO_mLZZXF6CHF4lZtZIDuh4nHzVg?usp=sharing

A small, dependency-free Python utility that counts **words** and **letters** in text and reports frequency distributions.  
It is **Unicode-aware** and supports Polish diacritics (e.g., ą, ć, ę, ł, ń, ó, ś, ź, ż).

---

## Features
- **Word counting** via regex for letter sequences (Latin + Polish diacritics)
- **Letter counting** using `str.isalpha()` (letters only; punctuation excluded)
- **Frequencies** for both letters and words (`collections.Counter`)
- **Case-insensitive** via `str.casefold()` (better than `lower()` for Unicode)
- **No external dependencies**

---

## Run in Colab
1. Click the **Open in Colab** badge (or the direct link) above.  
2. In Colab, go to **Runtime → Run all**.  
3. The notebook demonstrates analysis on the bundled sample text; you can paste your own text and re-run.

---

## Run locally

```bash
# Python 3.10+ recommended
python -m venv .venv && . .venv/Scripts/activate  # (Windows)
# or: python -m venv .venv && source .venv/bin/activate  # (macOS/Linux)

# no extra packages required
python text_stats.py
