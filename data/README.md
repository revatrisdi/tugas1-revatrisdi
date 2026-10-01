# Data Tugas 1

## Dataset yang Dipilih

Isi informasi berikut sebelum Milestone 1.

| Item | Isi |
|---|---|
| Nama dataset | `indonesian_news_dataset` (`data.csv`) |
| Sumber | [Kaggle - Indonesian News Dataset (iqbalmaulana)](https://www.kaggle.com/datasets/iqbalmaulana/indonesian-news-dataset) |
| Lisensi/ketentuan pakai | Open Source / Public Domain |
| Ukuran | 737.92 MB (Memenuhi syarat > 500 MB) |
| Periode data | Arsip Berita Daring Indonesia (Tempo, CNN Indonesia, CNBC Indonesia, Okezone, Suara, Kumparan, JawaPos) |
| Unit analisis | Artikel berita daring dari 7 media terkemuka di Indonesia |

## Struktur Kolom Dataset

Dataset `data.csv` memiliki total **11 kolom** dengan rincian sebagai berikut:

| No. | Nama Kolom | Deskripsi / Keterangan |
|:---|:---|:---|
| 1 | `id` | ID unik untuk setiap artikel berita. |
| 2 | `source` | Nama atau identitas media sumber berita (Tempo, CNN Indonesia, dll.). |
| 3 | `title` | Judul dari artikel berita. |
| 4 | `image` | Tautan atau referensi gambar visual yang menyertai artikel. |
| 5 | `url` | Tautan asli menuju halaman web berita. |
| 6 | `content` | Isi teks lengkap atau tubuh utama dari artikel berita. |
| 7 | `date` | Tanggal publikasi artikel berita. |
| 8 | `embedding` | Representasi vektor *embedding* dari teks berita. |
| 9 | `created_at` | *Timestamp* waktu data dicatat ke dalam sistem. |
| 10| `updated_at` | *Timestamp* waktu data terakhir diperbarui. |
| 11| `summary` | Ringkasan singkat mengenai isi berita. |

## Tempat Mencari Dataset

Pilih dataset Indonesia yang legal digunakan, dapat didokumentasikan sumbernya, dan memenuhi batas ukuran tugas.

| Situs | Kegunaan |
|---|---|
| [Satu Data Indonesia](https://data.go.id/) | Portal data terbuka lintas instansi pemerintah Indonesia. |
| [Badan Pusat Statistik](https://www.bps.go.id/) | Statistik sosial, ekonomi, kependudukan, dan data wilayah. |
| [BMKG Data Online](https://dataonline.bmkg.go.id/) | Data cuaca, iklim, gempa bumi, dan observasi meteorologi. |
| [Hugging Face Datasets](https://huggingface.co/datasets) | Dataset publik yang dapat dicari berdasarkan topik, bahasa, ukuran, dll. |
| [Kaggle Datasets](https://www.kaggle.com/datasets) | Katalog dataset publik; periksa lisensi dan dokumentasi pembuatnya. |
| [Google Dataset Search](https://datasetsearch.research.google.com/) | Mesin pencari untuk menemukan dataset dari berbagai portal. |

## Cara Memperoleh Data

1. Buka halaman dataset di Kaggle melalui tautan [Indonesian News Dataset](https://www.kaggle.com/datasets/iqbalmaulana/indonesian-news-dataset).
2. Klik tombol **Download** untuk mengunduh arsip dataset.
3. Ekstrak file dan ambil file mentah **`data.csv`** (ukuran ~737.92 MB), lalu letakkan ke dalam folder `data/raw/` pada direktori proyek tanpa mengubah data aslinya.
4. Atur variabel path pada `notebooks/01_data_profiling.ipynb` agar mengarah ke file `data.csv` tersebut.

## Aturan Penyimpanan

- Jangan commit dataset mentah atau hasil olahan berukuran besar ke Git.
- File pada `data/raw/` adalah data asli dan tidak boleh diubah.
- Simpan hasil transformasi yang dapat direproduksi pada `data/processed/`.