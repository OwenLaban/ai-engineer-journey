# ✅ Checklist Progres — AI Engineer 24 Minggu

> Update file ini setiap minggu. Centang `[x]` jika selesai.
> Target: setiap minggu ada commit ke GitHub!

---

## 📦 Fase 0 — Fondasi Software

### Minggu 1 — Setup + Python Dasar
- [x] Install Python 3.12+, VS Code, Git *(terverifikasi: Python 3.13.5, Git 2.45.1)*
- [x] Variabel, tipe data, list/dict, loop, fungsi *(3 latihan + proyek utama selesai)*
- [x] Virtual environment + pip *(selesai: `.venv` + upgrade pip 26.2.1 + `.gitignore`)*
- [x] Latihan: kalkulator + konverter suhu *(lulus review 8.5→10 setelah cleanup)*
- [x] Commit minggu ini ✅

### Minggu 2 — Python Lanjutan
- [x] Error handling, file I/O, modul *(latihan 05 + 06)*
- [x] OOP dasar: class, method *(latihan 07)*
- [x] f-string, list comprehension, typing hints *(latihan 08)*
- [x] Latihan: CLI manajemen tugas *(proyek 09: CRUD + JSON persistence)*
- [x] Commit minggu ini ✅

### Minggu 3 — Git + GitHub + Proyek #1
- [x] Git: init, commit, branch, merge *(branch `rapikan/latihan-09` → PR #1 → merge)*
- [x] GitHub: push, pull, PR *(PR #1 merged + branch terhapus)*
- [x] README.md rapi *(diperbarui: latihan 05–09 + proyek 09)*
- [x] **Proyek #1: CLI To-do app → GitHub** 🎯 *(repo `todo-cli`, 17/17 uji lulus)*
- [x] Commit minggu ini ✅

### Minggu 4 — HTTP + REST API
- [x] Konsep HTTP: method, status code *(latihan 10, SOAL 5: 4/4 benar)*
- [x] JSON parsing/serialisasi *(`json.loads` / `json.dumps`, olah list of dict)*
- [x] API key + environment variable (.env) *(`GITHUB_USER` di `.env`, file di-gitignore)*
- [x] Latihan: script consume public API *(latihan 11: GitHub API + Open-Meteo, 5/5)*
- [x] Commit minggu ini ✅ *(PR #3 merged)*

### Minggu 5 — FastAPI + Testing + Proyek #2
- [x] FastAPI: endpoint, Pydantic validation *(latihan 12: 5 endpoint + validasi 422)*
- [x] pytest: test endpoint *(latihan 13: 7/7 lulus)*
- [x] **Proyek #2: REST API notes app (CRUD + test)** 🎯 *(repo `notes-api`, 10/10 test)*
- [x] Commit minggu ini ✅ *(PR #5 merged)*

### Minggu 6 — Docker
- [x] Docker: image vs container, Dockerfile *(`python:3.13-slim`, layer cache, `.dockerignore`)*
- [x] API jalan dalam container *(build `notes-api:1.0`, port 8001:8000, health + CRUD OK)*
- [x] Volume + persistence *(`notes-data:/app/data` + `NOTES_FILE`; data selamat setelah container dibuat ulang)*
- [x] Docker Compose *(`docker compose up -d --build`, config valid)*
- [x] **🏁 LULUS FASE 0:** Proyek #2 lokal + Docker + test hijau + README
- [x] Commit minggu ini ✅ *(`notes-api` commit `62c2d1c`)*

---

## 🧠 Fase 1 — Inti LLM

### Minggu 7 — Introduction + Cara Kerja LLM
- [x] Intro: AI Engineer vs ML Engineer, roles & responsibilities *(dibahas: fokus membangun produk di atas model)*
- [x] Common terminology: AI vs AGI, LLM, embeddings, fine-tuning, RAG *(latihan 14 + kuis RAG vs fine-tuning)*
- [x] Token, context window, training vs inference *(latihan 14: tokenizer + 5/5 test)*
- [x] Temperature, top-k, top-p, repetition penalty *(dibahas + contoh penggunaan)*
- [x] Coba tokenizer playground *(`latihan_llm/`: hitung & pecah token, bandingkan encoding)*
- [x] Commit minggu ini ✅ *(PR #6 merged)*

### Minggu 8 — Prompt Engineering
- [x] Prompt anatomy: system prompt, role, constraints *(role + task + context + schema + constraints)*
- [x] Zero-shot, few-shot, CoT, ReAct, function calling *(dibahas; lab memakai zero-shot, few-shot, CoT, robust)*
- [x] Latihan: 5 variasi prompt untuk 1 tugas *(latihan 15: ekstraksi email → JSON + evaluasi Email 1/2)*
- [x] Commit minggu ini ✅ *(PR #8 merged)*

### Minggu 9 — Proyek #3: Chatbot API
- [x] Chatbot + memory percakapan *(JSON per sesi; live test ingat nama “Rina”)*
- [x] Structured output JSON via Pydantic *(`ChatResponse`: balasan, topik, sentimen, butuh_eskalasi)*
- [x] **Proyek #3 selesai + README** 🎯 *([chatbot-api](https://github.com/OwenLaban/chatbot-api), 16/16 test)*
- [x] **🏁 LULUS FASE 1:** output JSON valid + evaluasi manual *(live OpenRouter + tabel evaluasi di README)*
- [x] Commit minggu ini ✅ *(PR #1 merged)*

---

## 🔌 Fase 2 — Model & Konteks

### Minggu 10 — Ekosistem Model
- [ ] Closed vs open-source vs self-hosted
- [ ] Kriteria memilih model
- [ ] Commit minggu ini ✅

### Minggu 11 — Hugging Face + Model Lokal
- [ ] Hugging Face: Hub, tasks, model card
- [ ] Install Ollama → jalankan model lokal
- [ ] Coba OpenRouter
- [ ] Latihan: 1 tugas di 3 model
- [ ] Commit minggu ini ✅

### Minggu 12 — Context Engineering + Proyek #4
- [ ] Sumber konteks, memory, compaction
- [ ] Context failure modes
- [ ] **Proyek #4: app model lokal (Ollama)** 🎯
- [ ] **🏁 LULUS FASE 2:** laporan tradeoff 2–3 model

---

## 🗄️ Fase 3 — RAG

### Minggu 13 — Embeddings
- [ ] Konsep embedding + semantic similarity
- [ ] Use case 4 jenis
- [ ] Latihan: semantic search 20 kalimat
- [ ] Commit minggu ini ✅

### Minggu 14 — Vector Database
- [ ] Pilih 1 DB: Chroma atau Qdrant
- [ ] Indexing + similarity search + metadata filter
- [ ] Latihan: 100 dokumen + query semantik
- [ ] Commit minggu ini ✅

### Minggu 15 — Pipeline RAG
- [ ] Chunking → embedding → retrieval → generation
- [ ] Chunking strategy + impact
- [ ] Coba LangChain/LlamaIndex setelah SDK langsung
- [ ] Commit minggu ini ✅

### Minggu 16 — Proyek #5: RAG Dokumen
- [ ] **Proyek: tanya-jawab dokumen pilihanmu** 🎯
- [ ] Sitasi sumber per jawaban
- [ ] Laporan evaluasi sederhana
- [ ] **🏁 LULUS FASE 3:** RAG akurat + sitasi + README

---

## 🤝 Fase 4 — Agent + MCP + Safety

### Minggu 17 — AI Agents
- [ ] Konsep agent: LLM + tools + loop
- [ ] Tools & function calling, ReAct
- [ ] Latihan: agent 1 tool dari nol (tanpa framework)
- [ ] Commit minggu ini ✅

### Minggu 18 — Agent Framework
- [ ] Pilih: Claude Agent SDK atau OpenAI Agent SDK
- [ ] Agent 2–3 tools
- [ ] Commit minggu ini ✅

### Minggu 19 — MCP + Proyek #6
- [ ] Komponen MCP: host, client, server, transport
- [ ] **Proyek #6: MCP server sederhana** 🎯
- [ ] Connect ke Claude Code/desktop
- [ ] Commit minggu ini ✅

### Minggu 20 — AI Safety & Ethics
- [ ] Prompt injection, data leak, bias
- [ ] Mitigasi: sanitasi, batasan output, adversarial testing
- [ ] **🏁 LULUS FASE 4:** agent + MCP + lolos 5 skenario injection

---

## 📊 Fase 5 — Eval + Deploy + Karier

### Minggu 21 — Evaluation & Observability
- [ ] Eval: deterministik, model-based, human
- [ ] DeepEval/RAGAS + tracing (Langfuse)
- [ ] Regression testing prompt/RAG/agent
- [ ] Commit minggu ini ✅

### Minggu 22 — Multimodal + Dev Tools
- [ ] Image/audio/TTS dasar
- [ ] Pakai Claude Code/Cursor untuk mempercepat
- [ ] Commit minggu ini ✅

### Minggu 23 — Capstone
- [ ] **Capstone: RAG + agent + MCP + eval + observability** 🏆
- [ ] Deploy: Docker + API publik + monitoring
- [ ] Commit minggu ini ✅

### Minggu 24 — Persiapan Karier
- [ ] Rapikan semua repo: README profesional
- [ ] CV + LinkedIn + cerita proyek
- [ ] Latihan interview (jelaskan RAG & tradeoff model)
- [ ] Mulai apply 🚀

---

## 📈 Portfolio Tracker

| # | Proyek | Repo | Status |
|---|---|---|---|
| 1 | CLI To-do app | [todo-cli](https://github.com/OwenLaban/todo-cli) | ✅ |
| 2 | REST API notes app + Docker | [notes-api](https://github.com/OwenLaban/notes-api) | ✅ |
| 3 | Chatbot API + structured output | [chatbot-api](https://github.com/OwenLaban/chatbot-api) | ✅ |
| 4 | App model lokal (Ollama) | — | ⬜ |
| 5 | RAG dokumen + sitasi | — | ⬜ |
| 6 | MCP server | — | ⬜ |
| 🏆 | Capstone | — | ⬜ |

## 📝 Catatan Mingguan

> Tulis kendala/pelajaran tiap minggu di sini.

- **Minggu 1:** ✅ Selesai semua. Dasar Python + proyek kalkulator lulus review. Repo [python-dasar](https://github.com/OwenLaban/python-dasar) sudah live di GitHub lengkap dengan README, `.gitignore`, dan venv (lebih awal dari jadwal Minggu 3). 5 commit.
- **Minggu 2:** ✅ Selesai. Latihan 05–08 lulus review; proyek 09 CLI manajemen tugas (CRUD + JSON) lulus 11/11 uji. Pelajaran utama: indentasi blok `main`, `try` harus membungkus operasi yang error, dan path data dikunci ke lokasi script (`Path(__file__).parent`).
- **Minggu 3:** ✅ Selesai. Latihan branch → PR #1 → merge di repo `python-dasar`; proyek portfolio #1 `todo-cli` live (CRUD + filter + cari + JSON, 17/17 uji). README profesional berisi masalah, demo, cara jalan, arsitektur, dan keterbatasan.
- **Minggu 4:** ✅ Selesai. Latihan 10 (HTTP/JSON) dan 11 (consume API GitHub + Open-Meteo) lulus review, PR #3 merged. Pelajaran utama: **variable shadowing** — nama loop `tugas` menimpa list-nya sehingga `len("Baca status code") - 2 = 14`; dan **environment variable** membuat konfigurasi berubah tanpa mengubah kode. Status code: 2xx sukses, 4xx salah client (401 vs 403), 5xx salah server.
- **Minggu 5:** ✅ Selesai. Latihan 12–13 lulus (5 endpoint + 7 test), proyek #2 `notes-api` live: CRUD + JSON persistence + 10/10 test pytest + README portfolio. Pelajaran: pytest hanya mengumpulkan fungsi `test_*`; `raise` sebelum kode membuat sisa fungsi unreachable; `response_model` memvalidasi output; fixture `tmp_path` membuat test terisolasi.
- **Minggu 6:** ✅ Selesai. `notes-api` di-Dockerize: image `python:3.13-slim` (200MB), `.dockerignore`, pemisahan `requirements.txt` (runtime) vs `requirements-dev.txt`, named volume `notes-data` + `NOTES_FILE`, dan Docker Compose. Verifikasi: health + CRUD di port 8001 OK, data selamat setelah container dihapus & dibuat ulang, 10/10 pytest. Pelajaran: container punya filesystem sendiri — tanpa volume data hilang; port mapping `host:container`; server wajib bind `0.0.0.0` di dalam container; copy `requirements.txt` dulu agar layer pip ter-cache. **Fase 0 selesai.**
- **Minggu 7:** ✅ Selesai. Latihan 14 tokenizer/context window: 4 fungsi + 5 test (total 12 test repo). Pelajaran: token ≠ kata; jumlah token tergantung tokenizer (`o200k_base` vs `cl100k_base`); 8.000 token ≈ 6.000–6.500 kata; context window dihitung token; RAG = retrieval + LLM (model tidak mencari sendiri di PDF); fine-tuning mengubah parameter, RAG menyuntik konteks; API key jangan pernah masuk prompt/repo. PR #6 merged.
- **Minggu 8:** ✅ Selesai. Latihan 15: 5 variasi prompt untuk ekstraksi email → JSON tiket (zero-shot, role+schema, few-shot, CoT, robust/edge case), diuji dengan Email 1 + edge case Email 2. Semua output utama JSON valid; **few-shot** paling konsisten, sedangkan prompt 5 mengalami under-extraction (`produk: null`). Pelajaran: schema eksplisit mengunci format; contoh mengunci gaya dan level detail; constraint berlebihan bisa menurunkan recall; email harus diperlakukan sebagai data, bukan instruksi. PR #8 merged.
- **Minggu 9:** ✅ Selesai. Proyek #3 [chatbot-api](https://github.com/OwenLaban/chatbot-api): FastAPI + memory JSON per sesi + output Pydantic + klien OpenRouter. 16/16 test; live test ingat nama, isolasi sesi, dan delete → 404. Pelajaran: test dengan mock bisa hijau meski `_client()` lupa `return` — tambahkan test konfigurasi client; `openrouter/free` adalah auto-router yang bisa memilih model safety, jadi pakai model chat spesifik; API key hanya di `.env`. PR #1 merged. **Fase 1 selesai.**
