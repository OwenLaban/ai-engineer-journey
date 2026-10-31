# 🤖 Rencana Jadi AI Engineer — 24 Minggu

> Based on: [roadmap.sh/ai-engineer](https://roadmap.sh/ai-engineer) (2026)
> Profil: Mulai dari nol → Career switch → 20+ jam/minggu

---

## 🎯 Target Akhir

Kamu siap apply sebagai **Junior AI Engineer / AI Application Engineer** jika bisa:

- ✅ Membangun API Python yang rapi + Docker
- ✅ Membuat aplikasi LLM: prompt engineering, structured output, function calling
- ✅ Membangun RAG lengkap: chunking → embedding → vector DB → retrieval → generation + sitasi
- ✅ Membuat agent dengan tools + MCP server/client sederhana
- ✅ Evaluasi, regression testing, observability, mitigasi prompt injection
- ✅ Punya **4–6 repo portfolio** di GitHub + 1 capstone + README profesional

## 🗺️ Struktur 24 Minggu

| Fase | Minggu | Fokus roadmap.sh | Proyek Wajib |
|---|---|---|---|
| 0. Fondasi Software | 1–6 | Prasyarat backend | CLI Python + REST API + Docker |
| 1. Inti LLM | 7–9 | Intro, Cara Kerja LLM, Prompt Engineering | Prompt Lab + Chatbot API |
| 2. Model & Konteks | 10–12 | Type of Models, Hugging Face, Ollama, Context Engineering | Laporan perbandingan model |
| 3. RAG | 13–16 | Embeddings, Vector DB, RAG | RAG dokumen sendiri + sitasi |
| 4. Agent + MCP + Safety | 17–20 | AI Agents, MCP, AI Safety/Ethics | Agent multi-tool + MCP server |
| 5. Eval + Deploy + Karier | 21–24 | Observability, Evaluations, Multimodal | Capstone + deploy + CV |

---

## 📦 Fase 0 — Fondasi Software (Minggu 1–6)

> ⚠️ Fase paling penting. Jangan dipercepat. Semua fase selanjutnya berdiri di sini.

### Minggu 1 — Setup + Python Dasar
- Install Python 3.12+, VS Code, Git
- Python dasar: variabel, tipe data, list/dict, loop, fungsi
- Virtual environment + pip
- **Latihan:** program kalkulator + konverter suhu (fungsi terpisah)

### Minggu 2 — Python Lanjutan
- Error handling (try/except), file I/O, modul
- OOP dasar: class, method, inheritance
- f-string, list comprehension, typing hints dasar
- **Latihan:** program manajemen tugas sederhana (CLI)

### Minggu 3 — Terminal, Git, GitHub
- Terminal: navigasi, command dasar
- Git: init, add, commit, branch, merge, log
- GitHub: push, pull, clone, pull request
- Menulis README.md yang rapi
- **Proyek #1:** CLI Python (To-do app) → push ke GitHub dengan README bagus

### Minggu 4 — Web: JSON, HTTP, REST API
- Konsep HTTP: method, status code, header, body
- JSON: parsing, serialisasi
- Cara kerja REST API + autentikasi API key
- Environment variable (.env) — jangan hardcode secret
- **Latihan:** script yang consume public API (mis. cuaca) via `requests`

### Minggu 5 — FastAPI + Testing
- FastAPI: endpoint, path/query parameter, Pydantic validation
- pytest dasar: test endpoint
- **Proyek #2:** REST API "notes app" (CRUD lengkap + validasi + 3 test)

### Minggu 6 — Docker + Penutup Fondasi
- Docker: image vs container, Dockerfile, docker compose
- Menjalankan API di dalam container
- **Lulus Fase 0 jika:** Proyek #2 berjalan lokal + di Docker + test hijau + README jelas

---

## 🧠 Fase 1 — Inti LLM (Minggu 7–9)

### Minggu 7 — Introduction + Cara Kerja LLM
- Introduction: apa itu AI Engineer, roles & responsibilities, AI Engineer vs ML Engineer, impact on product development
- Common terminology: AI vs AGI, LLM, embeddings, fine-tuning, inference, RAG, context window
- Cara kerja LLM: token, context, parameter sampling: temperature, top-k, top-p, repetition penalty
- Tokenizer: coba main-main di playground tokenizer
- Kebiasaan aman: **jangan pernah tempel API key/secret ke prompt**
- Sumber: blog "visual intro to LLMs", seri YouTube 3Blue1Brown

### Minggu 8 — Prompt Engineering
- Prompt anatomy: system prompt, role & behavior, context, constraints, output format
- Teknik: zero-shot, few-shot, CoT, ReAct, function calling, streaming, prompt caching
- Iterasi prompt: baseline → ubah → bandingkan hasil
- **Latihan:** 5 variasi prompt untuk 1 tugas, bandingkan kualitasnya

### Minggu 9 — Proyek #3: Chatbot API + Structured Output
- Chatbot dengan memory percakapan sederhana
- Structured output: JSON schema terkontrol via Pydantic
- **Lulus Fase 1 jika:** chatbot API output JSON valid + punya evaluasi manual sederhana + README

---

## 🔌 Fase 2 — Model & Konteks (Minggu 10–12)

### Minggu 10 — Ekosistem Model
- Jenis model: pre-trained, closed vs open-source, self-hosted
- Kriteria memilih: kualitas, latensi, biaya, privasi, dukungan bahasa Indonesia
- Model utama: Claude, GPT, Gemini, Llama, DeepSeek, Qwen, Gemma, Mistral

### Minggu 11 — Hugging Face + Model Lokal
- Hugging Face: Hub, tasks, model card, inference
- Install **Ollama** → jalankan model lokal (mis. Llama 3.2, Qwen)
- Coba OpenRouter untuk akses banyak model via 1 API
- **Latihan:** tugas yang sama dijalankan di 3 model berbeda, bandingkan

### Minggu 12 — Context Engineering + Proyek #4
- Context engineering: sumber konteks, memory, compaction, long-context
- Context failure modes: kenapa LLM "lupa" dan salah
- **Proyek #4:** aplikasi dengan model lokal (Ollama) — mis. summarizer dokumen
- **Lulus Fase 2 jika:** laporan tradeoff 2–3 model untuk 1 tugas nyata (biaya, kecepatan, kualitas)

---

## 🗄️ Fase 3 — RAG (Minggu 13–16)

> Fase paling sering ditanya di interview AI Engineer.

### Minggu 13 — Embeddings
- Konsep embedding: teks → vektor, semantic similarity
- Use case: semantic search, klasifikasi, rekomendasi, deteksi anomali
- Embedding model: OpenAI vs Sentence Transformers (open-source)
- **Latihan:** semantic search sederhana di 20 kalimat

### Minggu 14 — Vector Database
- Pilih **satu dulu**: Chroma (paling gampang) atau Qdrant
- Konsep: indexing, similarity search, metadata filter
- **Latihan:** simpan 100 dokumen kecil, query semantik

### Minggu 15 — Pipeline RAG
- Pipeline lengkap: chunking → embedding → indexing → retrieval → generation
- Chunking strategy: size, overlap, impact pada kualitas
- Framework: SDK langsung dulu, lalu coba LangChain atau LlamaIndex
- RAG vs fine-tuning: kapan pakai yang mana (konsep)

### Minggu 16 — Proyek #5: RAG Dokumen Sendiri
- **Proyek:** tanya-jawab atas dokumen pilihanmu (mis. buku/PDF/spesifikasi)
- Wajib ada: **sitasi sumber** per jawaban + laporan evaluasi sederhana
- **Lulus Fase 3 jika:** RAG menjawab akurat dari dokumen + sitasi + README

---

## 🤝 Fase 4 — Agent + MCP + Safety (Minggu 17–20)

### Minggu 17 — AI Agents
- Konsep agent: LLM + tools + loop keputusan
- Tools & function calling, ReAct prompting
- Multi-agent: kapan perlu, kapan overkill
- **Latihan:** agent 1 tool (kalkulator/cari-cuaca) dari nol tanpa framework

### Minggu 18 — Agent dengan Framework
- Framework: Claude Agent SDK atau OpenAI Agent SDK (pilih satu)
- Agent 2–3 tools: baca file, search web, database sederhana

### Minggu 19 — MCP (Model Context Protocol)
- Komponen: host, client, server, transport, data layer
- **Proyek #6:** MCP server sederhana (mis. expose API cuaca/notes sebagai tools)
- Connect MCP server ke Claude Code/desktop

### Minggu 20 — AI Safety & Ethics
- Ancaman: prompt injection, data leak, bias
- Mitigasi: sanitasi input, batasan output, adversarial testing, content moderation
- **Lulus Fase 4 jika:** agent multi-tool + MCP server + lolos 5 skenario prompt injection

---

## 📊 Fase 5 — Eval + Deploy + Karier (Minggu 21–24)

### Minggu 21 — LLM Evaluation & Observability
- Eval: deterministik, model-based, human eval, metrik
- Tools: DeepEval / RAGAS + tracing (Langfuse / LangSmith / Helicone)
- Regression testing untuk prompt/RAG/agent

### Minggu 22 — Multimodal Dasar + Dev Tools
- Image understanding, audio (Whisper), Text-to-Speech — secukupnya
- AI-assisted coding tools: Claude Code, Cursor — pakai untuk mempercepat proyek

### Minggu 23 — Capstone
- **Capstone:** gabungan semua skill — RAG + agent + MCP + evaluasi + observability
- Contoh: "Asisten dokumen internal" dengan agent yang bisa cari dokumen, jawab dengan sitasi, evaluasi diri
- Deploy: Docker + API publik + monitoring biaya/latensi

### Minggu 24 — Persiapan Karier
- Rapikan semua repo GitHub: README profesional (masalah, arsitektur, cara jalanin, keterbatasan, hasil eval)
- CV + LinkedIn: cerita proyek, bukan sekadar daftar skill
- Latihan interview: jelaskan RAG pipeline & tradeoff model dengan kata-katamu sendiri
- Apply: Junior AI Engineer, AI Application Engineer, LLM Engineer (entry)

---

## 📏 Aturan Main

1. **Alokasi 20 jam/minggu:** 8 jam bangun → 6 jam teori → 4 jam dokumentasi → 2 jam review
2. **Satu stack saja:** Python + FastAPI + 1 vector DB (Chroma) + 1 framework RAG/agent
3. **Tiap proyek wajib README:** masalah, arsitektur, cara menjalankan, keterbatasan, hasil evaluasi
4. **Anti tutorial-hell:** setiap minggu harus ada commit. Kalau tidak commit = tidak belajar
5. **Hemat biaya:** model lokal (Ollama) + kuota gratis dulu; eksperimen berbayar dibatasi ~Rp200rb/bulan
6. **Jangan loncat fase:** agents/RAG tanpa fondasi Python = frustrasi

## 📚 Sumber Belajar Utama (gratis dulu)

- [roadmap.sh/ai-engineer](https://roadmap.sh/ai-engineer) — peta jalan (ini)
- [Python for Everybody](https://www.py4e.com/) atau kursus Python CS50P — Fase 0
- [FastAPI docs](https://fastapi.tiangolo.com/) — resmi & bagus
- [Prompt Engineering Guide](https://www.promptingguide.ai/) — Fase 1
- [Hugging Face Learn](https://huggingface.co/learn) + [Ollama docs](https://ollama.com/) — Fase 2
- [LangChain docs](https://python.langchain.com/) / [LlamaIndex docs](https://docs.llamaindex.ai/) — Fase 3
- [Anthropic MCP docs](https://modelcontextprotocol.io/) — Fase 4
- [DeepEval](https://deepeval.com/) / [RAGAS](https://docs.ragas.io/) — Fase 5

## ⚠️ Risiko Utama

Roadmap.sh itu luas — jangan tenggelam. Untuk career switch dari nol, risiko terbesar:

1. **Loncat ke agents/RAG sebelum Python kuat** → semua jadi copy-paste buta
2. **Tutorial hell** → nonton banyak, build nol
3. **Ganti-ganti framework** → waktu habis, portfolio kosong

Antidote: patuhi struktur fase + aturan main di atas. Progres dicek di `checklist-progres.md`.
