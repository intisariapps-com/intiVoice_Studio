# 🎙️ intiVoice AI Studio — Google Colab Turnkey Server

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/intisariapps-com/intiVoice_Studio/blob/main/intiVoice_Studio_Server.ipynb)
[![License: Apache 2.0](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![Python: 3.10+](https://img.shields.io/badge/python-3.10+-brightgreen.svg)](https://python.org)
[![Audio Quality: 48kHz](https://img.shields.io/badge/Audio-48kHz_Broadcast_Quality-purple.svg)](#)

> **Engine Backend GPU Serverless (Tesla T4) untuk Aplikasi [intiVoice Web Studio](https://intisariapps.com).**  
> Menghasilkan suara berkualitas siaran 48kHz, Voice Design berbasis teks, Dialog Dua Suara Alami, dan Voice Cloning 1:1 langsung dari Google Colab secara gratis dan instan.

---

## 🚀 Fitur Unggulan V1.6.3

* ⚡ **Turnkey 1-Click Server:** Cukup klik tombol **Open in Colab** dan pilih **Runtime ➔ Run all**, seluruh dependensi dan server API langsung online dalam hitungan detik.
* 🚀 **Zero Pop-Up Google Drive:** Berjalan instan dengan cache super-cepat NVMe SSD Colab tanpa pop-up dialog otorisasi izin Drive.
* 👥 **Dual-Speaker Dialogue Engine:** Sintesis percakapan naskah 2 pembicara berbeda dengan jeda nafas alami dan auto-export subtitle ganda.
* ⏱️ **Live Countdown Watchdog (3 Menit):** Widget hitung mundur realtime di layar Colab yang otomatis mematikan runtime saat menganggur untuk menghemat kuota GPU compute units.
* 🌐 **Otomasi Cloudflare Permanent Named Tunnel:** Menghasilkan URL publik domain tetap aman via Tunnel Token (TCP HTTP/2 Mode).
* 🎙️ **Ultimate Voice Cloning 1:1:** Mendukung kloning vokal tingkat tinggi via referensi audio WAV acuan untuk mereproduksi dinamika dan artikulasi asli pembicara.
* 🎬 **Dual Subtitle CapCut Generator:** Setiap kali sintesis selesai, sistem otomatis membuat berkas .SRT & .ASS Karaoke sinkron jeda nafas (Mobile Safe Zone 9:16).

---

## 📖 Cara Penggunaan

1. Klik tombol **Open in Colab** di atas atau buka berkas [`intiVoice_Studio_Server.ipynb`](./intiVoice_Studio_Server.ipynb).
2. Pastikan jenis runtime telah menggunakan GPU:
   * Buka menu **Runtime** ➔ **Change runtime type** ➔ Pilih **T4 GPU** ➔ Klik **Save**.
3. Jalankan seluruh sel:
   * Tekan menu **Runtime** ➔ **Run all** (atau shortcut `Ctrl+F9` di Windows / `Cmd+F9` di Mac).
4. (Opsional) Masukkan **Cloudflare Tunnel Token** jika ingin URL domain selalu tetap, atau biarkan kosong untuk Quick Tunnel acak.
5. Tunggu hingga terminal memunculkan banner sukses:
   ```text
   🎉 MESIN INTIVOICE AI SUDAH ONLINE DAN SIAP DIGUNAKAN!
   👉 SALIN URL INI KE WEB STUDIO:
      https://xxxxxxxx-xxxx.trycloudflare.com
   ```
6. Buka aplikasi **intiVoice Web Studio**, masuk ke **Tab Pengaturan Mesin**, tempel URL tersebut, lalu klik **Simpan & Uji Ping**.
7. Mulai generate suara atau kloning vokal dengan kualitas studio 48kHz!

---

## 🛠️ Persyaratan Sistem (Google Colab)

| Komponen | Spesifikasi |
|---|---|
| **GPU** | NVIDIA Tesla T4 (16GB VRAM) — Tersedia di Google Colab Free Tier |
| **Python** | Python 3.10 / 3.11 (Default Colab) |
| **Paket Inti** | PyTorch 2.5+, CUDA 12.0+, `uv`, FastAPI, Uvicorn, Cloudflared |
| **Penyimpanan** | Google Drive (~5GB untuk cache bobot model permanen) |

---

## 📄 Lisensi

Proyek ini dilisensikan di bawah [Apache License 2.0](LICENSE).
Dikembangkan untuk ekosistem produk digital suara cerdas **intisariapps.com**.
