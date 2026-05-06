# Generator Modul Ajar Pro

**Generator Modul Ajar Pro** adalah aplikasi berbasis Python dan Streamlit yang dirancang untuk membantu guru menyusun Modul Ajar Kurikulum Merdeka secara otomatis. Dengan memanfaatkan teknologi RAG (Retrieval-Augmented Generation) dan Gemini 2.5 Flash, aplikasi ini mampu membedah dokumen Capaian Pembelajaran (CP) yang kompleks dan mengubahnya menjadi draf modul yang taktis dan siap cetak.

---

## 🚀 Fitur Utama

### RAG-Powered Extraction
Mengekstrak konteks materi langsung dari file PDF Capaian Pembelajaran (CP) untuk akurasi konten yang tinggi.

### AI Smart Reasoning
Menggunakan model Gemini 2.5 Flash dengan konfigurasi deterministik (Temperature 0.0) untuk menghasilkan tujuan, langkah, dan asesmen yang logis.

### Format Dokumen Resmi
Menghasilkan file Microsoft Word (.docx) dengan standar administrasi sekolah, termasuk:

- Identitas lengkap (Nama Sekolah, Fase, Mapel, Alokasi Waktu)
- Format teks Justify (Rata Kanan-Kiri) otomatis untuk isi materi agar terlihat profesional
- Blok Tanda Tangan Presisi yang simetris antara Kepala Sekolah dan Guru

### JSON-Based Processing
Memastikan data yang dihasilkan AI tetap terstruktur dan stabil sebelum dimasukkan ke dalam dokumen.

---

## 🛠️ Teknologi yang Digunakan

- **Bahasa Pemrograman:** Python 3.x  
- **Framework UI:** Streamlit  
- **AI Engine:** Google Generative AI (Gemini 2.5 Flash)  
- **Dokumentasi:** python-docx untuk automated word generation  
- **PDF Parser:** PyPDF2 untuk ekstraksi data CP  

---

## 📦 Instalasi

### 1. Clone repositori ini
```bash
git clone https://github.com/username/generator-modul-ajar.git
cd generator-modul-ajar
```

## Instal dependensi
```bash
pip install streamlit google-generativeai python-docx PyPDF2
```

## Jalankan aplikasi
```
streamlit run app.py
```

## 💡 Cara Penggunaan

1. Dapatkan API Key Gemini secara gratis melalui Google AI Studio.  
2. Masukkan API Key pada kolom yang tersedia di sidebar aplikasi.  
3. Unggah file PDF Capaian Pembelajaran (CP) yang ingin dibedah.  
4. Lengkapi Identitas Sekolah & Guru (termasuk Nama dan NIP untuk tanda tangan).  
5. Isi Detail Modul (Mata Pelajaran, Fase, dan Topik Materi).  
6. Klik tombol **Generate Modul Ajar Resmi**.  
7. Unduh file `.docx` yang dihasilkan dan modul siap untuk digunakan atau diedit lebih lanjut.  

## 📝 Catatan Penting

### AI sebagai Copilot
Aplikasi ini dirancang untuk meringankan beban administratif guru sebesar 80–90%. Guru tetap disarankan untuk memeriksa kembali konten modul agar sesuai dengan sarana dan prasarana di sekolah masing-masing.

### Privasi API Key
Aplikasi menggunakan mode BYOK (Bring Your Own Key), sehingga API Key Anda aman dan tidak disimpan di server aplikasi.

## 👨‍💻 Developer
**Sinopa**  
**Fokus:** Data Analytics & Automation Engineering

## 📌 Penjelasan for developer

- **Justify & Presisi:** Gue masukin poin ini karena ini "jualan" utama lo di sisi kualitas dokumen.  
- **BYOK:** Ini penting buat ngejelasin ke user kalau API Key mereka aman.  
- **Role AI:** Gue pertegas bahwa ini alat bantu (Copilot), biar nggak ada salah paham kalau hasilnya 100% mutlak tanpa perlu dicek lagi.  
