# Pertemuan 2 - Format Dokumen XML

## 1. Profil XML
Struktur XML-nya seperti ini:

1. Deklarasi XML — `<?xml version="1.0" encoding="UTF-8"?>` di baris pertama, wajib ada dan menyatakan versi serta encoding dokumen.
2. Komentar — `<!-- Profil mahasiswa Web Semantik -->` sebagai keterangan, tidak memengaruhi data.
3. Root element — `<profilMahasiswa>`, satu-satunya elemen akar yang membungkus seluruh data (syarat XML well-formed, dimana hanya boleh ada satu root).
4. Element `<profil>`** — muncul berulang (5 kali), satu untuk tiap mahasiswa, dengan atribut `nim` berisi Nomor Induk Mahasiswa masing-masing.
5. Child elements di dalam setiap `<profil>`:
   - `<nama>` — nama lengkap mahasiswa
   - `<angkatan>` — tahun angkatan
   - `<programStudi>` — program studi
   - `<hobi>` — muncul dua kali per profil (elemen berulang, karena tiap orang punya 2 hobi)
   - `<deskripsi>` — deskripsi singkat, ditulis dalam blok teks

Semua tag dibuka-tutup dengan benar dan bersarang (nested) secara konsisten, sehingga dokumen memenuhi syarat **well-formed XML**.

## 2. Analisis Kesalahan XML

| No | Bagian yang Salah | Alasan | Perbaikan |
|---|---|---|---|
| 1 | `<nama>Budi Santoso</Nama>` | XML bersifat **case sensitive**, sehingga tag `<nama>` dan `</Nama>` dianggap berbeda. | `<nama>Budi Santoso</nama>` |
| 2 | `<angkatan>2024` | Tag `<angkatan>` tidak memiliki **tag penutup**. | `<angkatan>2024</angkatan>` |
| 3 | `<deskripsi>Saya suka AI & Web Semantik</deskripsi>` | Karakter `&` merupakan karakter khusus dalam XML. Harusnya menggunakan &amp; | `<deskripsi>Saya suka AI &amp; Web Semantik</deskripsi>` |

## 3. Analisis XML Schema
1. Root element: `buku`
2. Tipe data judul: `xs:string`
3. Tipe data tahun: `xs:gYear`
4. Tipe data harga: `xs:decimal`
5. Atribut ISBN: Wajib dituliskan karena menggunakan `use="required"`

## 4. Analisis Namespace
1. Mengapa kedua elemen title tidak sama? ...
2. Fungsi prefix: ...
3. Fungsi xmlns: ...
4. Apakah URI namespace harus dapat dibuka? ...

## 5. Pertanyaan Evaluasi
1. Perbedaan XML dan HTML: ...
2. Apa yang dimaksud well-formed? ...
3. Perbedaan well-formed dan valid: ...
4. Mengapa XSD lebih kuat dibanding DTD? ...
5. Mengapa namespace penting? ...
6. Apa kegunaan XPath? ...
