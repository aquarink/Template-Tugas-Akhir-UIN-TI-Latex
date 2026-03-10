# Template Tugas Akhir UIN TI LaTeX

Template ini dibuat untuk membantu mahasiswa **Program Studi Teknik Informatika UIN Syarif Hidayatullah Jakarta** dalam menulis skripsi menggunakan **LaTeX** secara terstruktur, rapi, dan sesuai format akademik.

Template ini juga sudah dilengkapi dengan **panduan penulisan setiap bab**, contoh penggunaan **gambar**, **tabel**, serta **sitasi menggunakan BibTeX**.

Struktur dokumen yang dihasilkan mencakup halaman awal seperti **lembar persetujuan, abstrak, daftar isi, daftar gambar, dan daftar tabel** sebelum masuk ke bab utama skripsi. :contentReference[oaicite:0]{index=0}

---

# Panduan Lengkap Template

Panduan penggunaan template secara lebih lengkap dapat diunduh atau dibaca melalui file berikut:

📄 **Panduan Template Skripsi (PDF)**  
https://github.com/aquarink/Template-Tugas-Akhir-UIN-TI-Latex/blob/main/panduan.pdf

Dokumen panduan ini berisi penjelasan lengkap mengenai:

- Struktur dokumen skripsi
- Penjelasan isi setiap bab
- Cara menggunakan BibTeX untuk sitasi
- Cara menyematkan gambar dan tabel
- Contoh State of The Art (SOTA)
- Pedoman penulisan skripsi menggunakan template ini

---

# Fitur Template

- Struktur skripsi lengkap (Bab 1 – Bab 6)
- Penomoran otomatis section, subsection, dan subsubsection
- Manajemen referensi menggunakan **BibTeX**
- Contoh penyematan **gambar dan tabel**
- Contoh **State of the Art (SOTA)**
- Contoh penggunaan **sitasi**
- Template sudah dilengkapi **panduan penulisan skripsi**

---

# Cara Menggunakan Template

Template ini direkomendasikan untuk digunakan melalui **Murfy.ai** agar proses kompilasi LaTeX lebih mudah.

---

# 1. Membuat Akun Murfy.ai

Buka halaman berikut:

https://app.murfy.ai

Kemudian lakukan pendaftaran akun.

Disarankan untuk **login menggunakan Google Account** agar proses pendaftaran lebih cepat.

---

# 2. Download Template dari GitHub

Masuk ke repository berikut:

https://github.com/aquarink/Template-Tugas-Akhir-UIN-TI-Latex

Klik tombol:

```
<> Code
```

Kemudian pilih:

```
Download ZIP
```

Atau langsung download melalui link berikut:

https://github.com/aquarink/Template-Tugas-Akhir-UIN-TI-Latex/archive/refs/heads/main.zip

Setelah itu simpan file ZIP tersebut di komputer Anda.

---

# 3. Upload Template ke Murfy.ai

Masuk ke dashboard Murfy:

https://app.murfy.ai/dashboard

Kemudian lakukan langkah berikut:

1. Klik **Create Project**
2. Pilih **Upload Project**
3. Upload file **ZIP** yang telah didownload dari GitHub
4. Tunggu hingga proses upload selesai

Setelah project berhasil diupload, template sudah siap digunakan.

---

# Struktur Folder Template

Berikut struktur utama pada repository:

```
.
├── chapters
│   ├── bab1.tex
│   ├── bab2.tex
│   ├── bab3.tex
│   ├── bab4.tex
│   ├── bab5.tex
│   └── bab6.tex
│
├── config
│   └── metadata.tex
│
├── images
│
├── references.bib
│
└── main.tex
```

Penjelasan:

| File / Folder | Fungsi |
|---|---|
| main.tex | File utama dokumen |
| chapters/ | Berisi masing-masing bab skripsi |
| config/metadata.tex | Mengatur judul skripsi, nama, NIM, dll |
| images/ | Folder untuk menyimpan gambar |
| references.bib | Database referensi BibTeX |

---

# Cara Menambahkan Referensi (BibTeX)

1. Cari artikel yang ingin disitasi melalui **Google Scholar**

https://scholar.google.com

2. Klik tombol **Cite / Kutip**

3. Pilih format **BibTeX**

4. Copy kode BibTeX yang muncul

Contoh:

```bibtex
@article{pebrianto2025adaptive,
  title={Adaptive DDoS Attack Detection: Entropy-Based Model With Dynamic Threshold and Suspicious IP Reevaluation},
  author={Pebrianto, Juri and Suryani, Vera},
  journal={IEEE Access},
  year={2025},
  publisher={IEEE}
}
```

5. Paste kode tersebut ke file:

```
references.bib
```

---

# Cara Menggunakan Sitasi

Untuk memanggil referensi pada dokumen gunakan:

```
\cite{pebrianto2025adaptive}
```

atau

```
\parencite{pebrianto2025adaptive}
```

Contoh hasil:

```
Pebrianto dan Suryani (2025)
```

atau

```
(Pebrianto dan Suryani, 2025)
```

Referensi yang digunakan akan otomatis muncul pada **Daftar Pustaka**.

---

# Cara Menambahkan Gambar

1. Upload gambar ke folder:

```
images/
```

2. Gunakan script berikut pada dokumen:

```
\begin{figure}[H]
\centering
\includegraphics[width=0.8\textwidth]{images/nama_gambar.png}
\caption{Judul gambar}
\label{fig:nama-gambar}
\end{figure}
```

3. Panggil gambar dalam teks menggunakan:

```
\ref{fig:nama-gambar}
```

Contoh penggunaan dalam paragraf:

```
Seperti ditunjukkan pada Gambar \ref{fig:nama-gambar}, sistem yang dikembangkan
mampu melakukan proses klasifikasi secara otomatis.
```

---

# Cara Menambahkan Tabel

Gunakan contoh berikut:

```
\begin{table}[H]
\centering
\begin{tabular}{lccc}
\toprule
Metode & Accuracy & Precision & Recall \\
\midrule
Metode A & 0.85 & 0.83 & 0.82 \\
Metode B & 0.90 & 0.88 & 0.87 \\
Metode Usulan & 0.94 & 0.92 & 0.91 \\
\bottomrule
\end{tabular}
\caption{Hasil perbandingan metode}
\label{tab:hasil-metode}
\end{table}
```

Memanggil tabel dalam teks:

```
Hasil evaluasi metode dapat dilihat pada Tabel \ref{tab:hasil-metode}.
```

---

# Struktur Bab Skripsi

Template ini sudah menyediakan struktur bab sebagai berikut:

```
BAB 1  PENDAHULUAN
BAB 2  LANDASAN TEORI
BAB 3  METODOLOGI PENELITIAN
BAB 4  HASIL DAN PEMBAHASAN
BAB 5  KESIMPULAN DAN SARAN
BAB 6  PENUTUP
```

Setiap bab sudah dilengkapi dengan **contoh penulisan dan panduan isi** agar mahasiswa lebih mudah menulis skripsi.

---

# Kontribusi

Jika ingin membantu pengembangan template ini:

1. Fork repository
2. Buat branch baru
3. Submit Pull Request

---

# Author

Pebri 

Repository:

https://github.com/aquarink/Template-Tugas-Akhir-UIN-TI-Latex