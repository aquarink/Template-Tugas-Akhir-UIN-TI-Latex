# Template Tugas Akhir UIN TI LaTeX

Template ini dibuat untuk membantu mahasiswa **Program Studi Teknik Informatika UIN Syarif Hidayatullah Jakarta** dalam menulis skripsi menggunakan **LaTeX** secara lebih terstruktur, rapi, dan konsisten dengan format akademik.

Template ini juga dilengkapi dengan **panduan penulisan pada setiap bab** sehingga mahasiswa dapat memahami apa saja yang harus ditulis pada setiap bagian skripsi.

---

# Fitur Template

- Struktur skripsi lengkap (Bab 1 – Bab 6)
- Template daftar gambar dan daftar tabel otomatis
- Manajemen referensi menggunakan **BibTeX**
- Contoh penyematan **gambar dan tabel**
- Contoh **State of the Art (SOTA)**
- Contoh penggunaan **sitasi**
- Penomoran otomatis section, subsection, dan subsubsection

---

# Cara Menggunakan Template

Template ini direkomendasikan untuk digunakan melalui **Murfy.ai** agar proses kompilasi LaTeX lebih mudah.

---

## 1. Membuat Akun Murfy.ai

Buka halaman berikut:


https://app.murfy.ai


Kemudian lakukan pendaftaran akun.

Disarankan untuk **login menggunakan Google Account** agar proses pendaftaran lebih cepat.

---

## 2. Download Template dari GitHub

Masuk ke repository berikut:


https://github.com/aquarink/Template-Tugas-Akhir-UIN-TI-Latex


Klik tombol:


<> Code


Kemudian pilih:


Download ZIP


atau langsung download melalui link berikut:


https://github.com/aquarink/Template-Tugas-Akhir-UIN-TI-Latex/archive/refs/heads/main.zip


Setelah itu simpan file ZIP tersebut di komputer Anda.

---

## 3. Upload Template ke Murfy.ai

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


.
├── chapters

│ ├── bab1.tex

│ ├── bab2.tex

│ ├── bab3.tex

│ ├── bab4.tex

│ ├── bab5.tex

│ └── bab6.tex

│

├── config

│ └── metadata.tex

│

├── images

│ └── (tempat menyimpan gambar)

│

├── references.bib

│

└── main.tex


Penjelasan:

| Folder/File | Fungsi |
|---|---|
| `main.tex` | File utama dokumen |
| `chapters/` | Berisi setiap bab skripsi |
| `images/` | Tempat menyimpan gambar |
| `references.bib` | Database referensi BibTeX |
| `config/metadata.tex` | Mengatur judul skripsi, nama, NIM, dll |

---

# Cara Menambahkan Referensi (BibTeX)

1. Cari artikel yang ingin disitasi melalui **Google Scholar**

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

Paste kode tersebut ke file:

references.bib
Cara Menggunakan Sitasi

Untuk memanggil referensi pada dokumen gunakan:

\cite{pebrianto2025adaptive}

atau

\parencite{pebrianto2025adaptive}

Contoh hasil:

Pebrianto dan Suryani (2025)

atau

(Pebrianto dan Suryani, 2025)

Referensi yang digunakan akan otomatis muncul pada Daftar Pustaka.

Cara Menambahkan Gambar

Upload gambar ke folder:

images/

Gunakan script berikut pada dokumen:

\begin{figure}[H]
\centering
\includegraphics[width=0.8\textwidth]{images/nama_gambar.png}
\caption{Judul gambar}
\label{fig:nama-gambar}
\end{figure}

Panggil gambar dalam teks menggunakan:

\ref{fig:nama-gambar}
Cara Menambahkan Tabel

Gunakan contoh berikut:

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
Kontribusi

Jika ingin membantu pengembangan template ini, silakan:

Fork repository

Buat branch baru

Submit Pull Request

Lisensi

Template ini dibuat untuk keperluan akademik mahasiswa.