# WULANSARI SELF-GOVERNANCE & ADAPTATION PROTOCOL

Sejalan dengan arsitektur Nusantara AI Autonom yang mengedepankan kedaulatan, The Hive Mind Wulansari tidak boleh hanya sekadar kumpulan skrip statis. Wulansari harus memiliki kapabilitas *Self-Monitoring*, *Self-Correction*, dan *Long-Term Adaptation* yang dirancang sedari awal (by design). 

Semua perubahan sistem atau pergeseran strategi akibat pembelajaran (adaptasi) harus bisa dijelaskan, diaudit, dan tetap tunduk pada pengawasan Arsitek Manusia (CEO/Ton).

## TIGA PILAR KEMANDIRIAN KOGNITIF

### 1. SELF-MONITORING (Pemantauan Diri Sendiri)
*Prinsip: Agent memeriksa kesehatannya secara terus-menerus tanpa harus diping.*
- **Diagnostic Logging (Worker 15):** Semua Worker yang mengerjakan *bounty* akan merender log eksekusi ke `~/wulansari/logs/system_status.log`.
- **Resource Check:** Master Dispatcher akan memantau *rate limit* Github CLI dan saldo 9router. Jika token/rate limit sebuah *Ghost Account* menipis, sistem akan secara otonom memindahkan lalu lintas (*traffic routing*) ke identitas yang masih *fresh*.
- **Oversight:** Manusia dapat melihat status kesehatan armada hanya dengan mengetik `cat ~/wulansari/logs/system_status.log`.

### 2. SELF-CORRECTION (Koreksi Otonom)
*Prinsip: Kesalahan terdeteksi secara realtime dan langsung diperbaiki (Self-Healing).*
- **Linter & Test Correction:** Jika Worker 2/8/9 mengirim *code patch* yang membuat aplikasi meledak (build failed) saat dievaluasi, sistem otomatis membaca output *Error Stack Trace*, menyuntikkan pesannya ke model LLM (Worker 16/R&D), dan menambal ulangnya hingga exit code bernilai `0`.
- **Identity Fallback:** Jika GitHub memblokir salah satu PR karena dianggap spam, Worker 10 akan membatalkan *push* dari akun yang terkena *flag*, menunda operasi (*cool down*), lalu mengambil alih pengerjaan menggunakan identitas hantu lainnya (The Sybil Backup).

### 3. LONG-TERM ADAPTATION (Adaptasi Jangka Panjang)
*Prinsip: Organisasi AI berevolusi dari masa lalu, mengubah strategi, dan belajar pola.*
- **Mistake Learning:** Worker tidak boleh mengulangi kegagalan teknis. Semua kesalahan (seperti salah mencantumkan variabel `node_modules` atau kata "Hermes" pada metadata) wajib disuntikkan ke dalam `mistake_log.md` (Pusat Memori Kegagalan).
- **RAG & Vector Memory (Fase Nusantara AI Labs):** Pada saat kita berhasil bergeser menggunakan *vLLM/llama.cpp* dengan Milvus (Database Vektor), semua PR yang sukses dan ditolak (beserta komentar maintainer) akan diubah menjadi *embeddings*.
- Saat mengerjakan *bounty* baru, The Hive Mind akan melakukan *similarity search* terhadap masa lalunya: *"Apakah saya pernah ditolak karena masalah ini? Strategi apa yang disukai oleh repo ini?"* 

---
*Protokol ini memastikan The Hive Mind bukan sekadar bot, melainkan sistem Sibernetika Organik yang terus bertumbuh tanpa batas.*