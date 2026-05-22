# 🤝 Contributing to RAG-CookBook

First off — thank you for taking the time to contribute! This repo grows through community effort, and every contribution matters, whether it's a new RAG pattern, a bug fix, a cleaner explanation, or a typo correction.

---

## 📋 Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
- [Adding a New RAG Notebook](#adding-a-new-rag-notebook)
- [Notebook Standards](#notebook-standards)
- [Pull Request Process](#pull-request-process)
- [Reporting Issues](#reporting-issues)
- [Style Guidelines](#style-guidelines)

---

## 📜 Code of Conduct

This project follows a simple rule: **be kind and constructive**. Harassment, discrimination, or toxic behaviour of any kind will not be tolerated. Treat everyone the way you'd want to be treated.

---

## 💡 How Can I Contribute?

There are many ways to contribute — you don't have to write a brand-new notebook to help:

| Contribution Type | Examples |
|-------------------|----------|
| 🆕 New RAG pattern | Graph RAG, Multi-Modal RAG, Speculative RAG |
| 🐛 Bug fix | Broken code cell, wrong imports, deprecated API calls |
| 📝 Documentation | Better explanations, clearer markdown, fix typos |
| 🎨 Improved examples | Better test queries, richer sample PDFs |
| ⭐ Improvements | Refactor existing notebooks, add missing steps |

---

## 📓 Adding a New RAG Notebook

### 1. Fork & Clone

```bash
git fork https://github.com/yanshiSharma/RAG-CookBook
git clone https://github.com/<your-username>/RAG-CookBook.git
cd RAG-CookBook
```

### 2. Create a Branch

Use a descriptive branch name:

```bash
git checkout -b add/graph-rag
# or
git checkout -b fix/corrective-rag-web-search
```

### 3. Create Your Notebook

Follow the naming convention:

```
<number>__<RAG-Type-Name>.ipynb
```

Examples:
- `8__Graph-RAG.ipynb`
- `9__Multimodal-RAG.ipynb`

If you're unsure what number to use, pick the next available one or leave it to the maintainer to assign during review.

### 4. Follow the Notebook Structure

Every notebook should follow this structure (see existing notebooks as reference):

```
[Title Cell]         → Bold title: "**<Type> RAG Implementation**"
[Spec Cell]          → Stack used (DB, embedding model, LLM, etc.)
[Workflow Cell]      → Step-by-step workflow description
[Numbered Steps]     → # Step 1: ..., # Step 2: ..., etc.
[Comments in code]   → Section headers inside code cells
```

### 5. Commit & Push

```bash
git add .
git commit -m "feat: add Graph RAG notebook"
git push origin add/graph-rag
```

### 6. Open a Pull Request

Go to the original repo and open a PR against the `main` branch. Fill out the PR template (if provided) or briefly describe:
- What RAG pattern you've added
- What stack/tools are used
- Any caveats or known limitations

---

## 📐 Notebook Standards

Please ensure your notebook meets these standards before submitting:

### ✅ Required

- [ ] Runs end-to-end in Google Colab without manual intervention (except API keys)
- [ ] All dependencies installed in the first cell via `!pip install`
- [ ] API keys are placeholder strings (`"YOUR_GROQ_API_KEY"`) — never real keys
- [ ] Workflow is documented in a markdown cell near the top
- [ ] Each major step has a `# Step N: Title` markdown heading
- [ ] Code cells have inline comments explaining non-obvious logic

### ✅ Recommended

- [ ] A brief explanation of *why* this RAG variant improves on the basic approach
- [ ] Notes on where this pattern shines vs. where it falls short
- [ ] At least one working test query at the end

### ❌ Do Not

- [ ] Hardcode real API keys, database URLs, or passwords
- [ ] Include large binary files or datasets
- [ ] Submit notebooks with execution output from cells containing sensitive data
- [ ] Duplicate an existing pattern without meaningfully extending it

---

## 🔁 Pull Request Process

1. Ensure your notebook passes the standards checklist above.
2. Update `README.md` — add a row to the RAG Patterns table for your new notebook.
3. Keep PRs focused: one notebook (or one fix) per PR.
4. Be responsive to review feedback — maintainers may request changes.
5. Once approved, your PR will be merged and you'll be credited in the repo.

**PR Title Format:**
```
feat: add <RAG Type> notebook
fix: correct <issue> in <notebook name>
docs: improve explanation in <notebook name>
```

---

## 🐛 Reporting Issues

Found a bug or a broken notebook? [Open an issue](https://github.com/yanshiSharma/RAG-CookBook/issues) with:

- **Notebook name** and step number where the error occurs
- **Error message** (copy the full traceback)
- **Environment** (Colab / local Jupyter / Python version)
- **What you expected** vs. **what happened**

---

## 🎨 Style Guidelines

### Markdown Cells
- Use `**Bold**` for titles and key terms
- Use `#`, `##` heading levels for steps — keep them consistent with existing notebooks
- Explain *what* the step does and briefly *why* before showing code

### Python Code
- Follow PEP 8 loosely — readability over strict compliance
- Use ALL_CAPS for constants (`SUPABASE_URL`, `GROQ_API_KEY`)
- Add section-header comments inside long cells:
  ```python
  # ==============================
  # FUNCTION TO EMBED TEXT
  # ==============================
  ```

---

## 🙏 Thank You

Every star, issue, and pull request helps make RAG-CookBook better for everyone learning about retrieval-augmented generation. You're awesome for being here.

---

<div align="center">
<a href="https://github.com/yanshiSharma/RAG-CookBook">⬅️ Back to RAG-CookBook</a>
</div>
