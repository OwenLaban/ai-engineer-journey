# 🤖 AI Engineer Journey

Rekap perjalanan belajar **AI Engineer selama 24 minggu** — dari Python dasar sampai
RAG, agent, MCP, evaluasi, dan deploy. Setiap proyek punya repo sendiri agar history
dan README-nya fokus; repo ini menjadi **pintu masuk dan papan progres**-nya.

> Roadmap acuan: [roadmap.sh/ai-engineer](https://roadmap.sh/ai-engineer) (2026)
> Status saat ini: **Minggu 12 selesai** ✅ — berikutnya Minggu 13 (Embeddings)

---

## 📦 Proyek

Repo ini memakai **git submodule**. Klik nama proyek untuk membuka repo aslinya.

| # | Proyek | Deskripsi | Teknologi | Status |
|---|---|---|---|---|
| 1 | [todo-cli](https://github.com/OwenLaban/todo-cli) | Manajemen tugas di terminal dengan CRUD, filter, pencarian, dan JSON persistence | Python | ✅ |
| 2 | [notes-api](https://github.com/OwenLaban/notes-api) | REST API catatan + Docker Compose dan volume persistence | FastAPI, Pytest, Docker | ✅ |
| 3 | [chatbot-api](https://github.com/OwenLaban/chatbot-api) | Chatbot dengan memory per sesi dan structured output JSON | FastAPI, Pydantic, OpenRouter | ✅ |
| 4 | [ringkas-dokumen](https://github.com/OwenLaban/ringkas-dokumen) | API summarizer dokumen lokal dengan chunking, map-reduce/refine, validasi output, dan benchmark 3 model | FastAPI, Ollama, Pytest | ✅ |
| — | [python-dasar](https://github.com/OwenLaban/python-dasar) | Lab Minggu 1–12: Python, HTTP/JSON, tokenizer, prompt engineering, pemilihan model, model lokal, dan context engineering | Python, FastAPI, Pytest, Ollama | ✅ |

---

## 📚 Dokumen

| File | Isi |
|---|---|
| [`rencana-ai-engineer.md`](rencana-ai-engineer.md) | Rencana lengkap 24 minggu, target akhir, dan daftar proyek wajib |
| [`checklist-progres.md`](checklist-progres.md) | Checklist mingguan, portfolio tracker, dan catatan pelajaran per minggu |

---

## 🚀 Cara Clone

Karena proyek berupa submodule, clone dengan:

```bash
git clone --recurse-submodules https://github.com/OwenLaban/ai-engineer-journey.git
```

Kalau sudah terlanjur clone biasa:

```bash
git submodule update --init --recursive
```

Untuk menarik update terbaru dari semua proyek:

```bash
git submodule update --remote --merge
```

---

## 🗺️ Peta Perjalanan

| Fase | Minggu | Fokus | Status |
|---|---|---|---|
| 0. Fondasi Software | 1–6 | Python, Git, CLI, REST API, Docker | ✅ |
| 1. Inti LLM | 7–9 | Cara kerja LLM, prompt engineering, chatbot API | ✅ |
| 2. Model & Konteks | 10–12 | Jenis model, Hugging Face, Ollama, context engineering | ✅ |
| 3. RAG | 13–16 | Embeddings, vector DB, RAG + sitasi | ⬜ |
| 4. Agent + MCP + Safety | 17–20 | Agent multi-tool, MCP, AI safety | ⬜ |
| 5. Eval + Deploy + Karier | 21–24 | Observability, evaluation, capstone, deploy | ⬜ |

---

## 🔐 Keamanan

Semua kredensial disimpan di `.env` dan **tidak pernah** di-commit. Yang dibagikan
hanya `.env.example`. Jangan menaruh API key di kode, prompt, atau README.
