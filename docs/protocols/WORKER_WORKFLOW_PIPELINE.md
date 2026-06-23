# WULANSARI WORKER WORKFLOW PIPELINE (THE 3-TIER ASSEMBLY LINE)

Untuk mencapai efisiensi industrial (layaknya pabrik keamanan siber), arsitektur 16-Agent direstrukturisasi menjadi 3 Tahapan (Tiers) yang beroperasi berurutan seperti ban berjalan (Assembly Line).

## TIER 1: THE SCOUTS (Pencari & Penyaring Target)
*Tugas: Mendeteksi peluang, menyaring noise, dan menyediakan daftar target yang tervalidasi.*
- **Worker 4 (GitHub Scout):** Memantau label `bounty` dan `good first issue` secara real-time.
- **Worker 5 (Micro-Bounty Scout):** Menyedot data dari Algora.io dan Gitcoin (Bounty <$100).
- **Worker 6 (High-ROI Watcher):** Memonitor HackerOne & Immunefi untuk target besar (>$1,000).
- **Worker 7 (Client Hunter):** Menyaring pesan di grup Telegram/Discord untuk mencari klien lepas (*freelance*).
> **Output Tier 1:** Daftar Repositori/Klien di `~/wulansari/targets/pending.json`

## TIER 2: THE ENGINEERS & HACKERS (Pekerja Eksekusi)
*Tugas: Melakukan kloning (via Master Dispatcher Worktree), meretas, menambal, dan membuat commit.*
- **Worker 1 (Lead Exploiter):** Menyerang target Immunefi menggunakan Foundry/Hardhat.
- **Worker 2 (Static Analyzer):** Menjalankan Slither/Semgrep otomatis.
- **Worker 3 (ZK & PQC Specialist):** Fokus pada target kriptografi dan matematika spesifik.
- **Worker 8 (Frontend Fixer):** Menambal *micro-bounties* berbasis UI (React, Tailwind).
- **Worker 9 (Backend Fixer):** Menambal API, Node.js, Python, Rust, dan Database.
> **Output Tier 2:** Repository Git dengan *branch* terselesaikan dan ter- *commit* rapi.

## TIER 3: THE GATEKEEPERS (Spesialis PR & Pengajuan)
*Tugas: Memverifikasi kode, mencegah kontaminasi branch, merakit deskripsi laporan kelas profesional, dan mengirim PR.*
- **Worker 10 (PR & Documentation Manager):** 
  - Mengecek setiap *Worktree* yang ditinggalkan Tier 2.
  - Memastikan *commit history* bersih (cherry-pick/rebase jika diperlukan).
  - Menulis laporan PR (Root Cause Analysis + Fix Applied).
  - Mengajukan PR dan membalas komentar *maintainer* repositori target.
> **Output Tier 3:** $USD (Bounty Terklaim).

---
*Alur:* `Tier 1 (Scout) -> Dispatcher.sh -> Tier 2 (Hack/Patch) -> Tier 3 (QC & PR)`
## TIER 4: THE ARCHITECTS (Infrastruktur & Inovasi Internal)
*Tugas: Memastikan Wulansari terus berevolusi melampaui limitasi hardware dan API berbayar.*
- **Worker 13 (R&D Rangers):** Mencari kerentanan Zero-Day dan meracik eksploit custom.
- **Worker 14 (OS Architect):** Meracik OS Linux X11 bare-metal teringan untuk rig Wulansari.
- **Worker 15 (Compliance & QA):** Hakim internal untuk menyensor PR dari kata-kata AI dan mengecek kredensial rahasia (Trufflehog).
- **Worker 16 (AI & LLM Dev):** Menerapkan local LLM (llama.cpp) dan RAG untuk memori jangka panjang agar sistem independen dari pihak ketiga.
