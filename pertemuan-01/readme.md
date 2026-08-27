| informasi | jenis |
| --- | --- |
| universitas sumatera utara | Entitas |          
| tanggal berdiri | atribut |
| universitas sumatera utara ->located in -> medan | relasi |
| Indonesia | entitas |
| coordinate location | atribut |
| universitas sumatera utara ->located in->indonesia | relasi |
| Jalan Dr T Mansur No 9 Padang Bulan | entitas |
| universitas sumatera utara ->located in->Jalan Dr T Mansur No 9 Padang Bulan | relasi |
| Postal Code | atribut |

---

| Nama Properti | Fungsi atau maknanya | Contoh nilai yang dapat digunakan |
| --- | --- | --- |
| address | alamat fisik universitas | Jl. Tri Dharma No.9, Padang Bulan, Kec. Medan Baru, Kota Medan, Sumatera Utara 20222 |
| telephone | nomor telepon universitas | 0821-6888-9060 |
| name | nama universitas | Universitas Sumatera Utara |
| url | situs resmi universitas | https://satu.usu.ac.id/home |
| event | acara yang akan datang atau sudah berlalu yang terkait dengan universitas | PKKMB USU 2026 |

## 4. Pertanyaan Evaluasi

### 1. Perbedaan utama antara web tradisional dan Web Semantik
Jawaban: Web tradisional dirancang agar dokumen (halaman HTML) dapat dibaca dan dipahami oleh manusia, tetapi mesin (komputer) hanya melihatnya sebagai teks dan tag format, tanpa memahami makna di baliknya. Web Semantik menambahkan struktur data yang memiliki makna (metadata) sehingga mesin dapat memahami arti dari informasi tersebut, bukan sekadar menampilkannya.

### 2. Mengapa suatu entitas membutuhkan identifier unik?
Jawaban: 
Identifier unik (biasanya berupa URI) dibutuhkan agar:
- Entitas dapat dirujuk secara konsisten dan tidak ambigu di seluruh sistem/web (menghindari adanya kerancuan, misalnya nama "Jakarta" bisa merujuk ke kota di Indonesia atau tempat lain).
- Data tentang entitas yang sama dari sumber berbeda dapat dihubungkan (linked data) karena mengacu pada identifier yang sama.
- Memungkinkan mesin membedakan antara entitas dengan nama sama tetapi makna berbeda. 

### 3. Perbedaan subject, predicate, dan object 
Jawaban:
"Raymond kuliah_di USU"
- Subject: Raymond → entitas yang dibicarakan.
- Predicate: kuliah_di → hubungan atau relasi antara subject dan object.
- Object: USU → entitas atau nilai yang menjadi tujuan relasi.

### 4. Keuntungan merepresentasikan informasi sebagai hubungan antarentitas dibanding teks biasa
Jawaban: 
- Dapat diolah mesin: teks biasa hanya rangkaian karakter, sedangkan representasi relasi (graph) memiliki struktur yang bisa diproses secara logis oleh komputer.
- Mendukung penalaran (reasoning): mesin dapat menyimpulkan fakta baru dari relasi yang ada (misalnya, jika A adalah bagian dari B, dan B adalah bagian dari C, maka A adalah bagian dari C).
- Query lebih presisi: memungkinkan pencarian berbasis makna, bukan sekadar pencocokan kata kunci.
- Integrasi data lebih mudah: data dari berbagai sumber dapat digabungkan karena entitas yang sama merujuk pada identifier yang sama.
- Mengurangi ambiguitas: relasi eksplisit membuat makna lebih jelas dibanding teks bebas yang bisa multitafsir.

### 5. Bagaimana Knowledge Graph dapat membantu sistem pencarian atau AI
Jawaban:
- Pemahaman konteks & makna: Knowledge Graph memungkinkan sistem memahami hubungan antarentitas (misalnya, mesin pencari tahu bahwa "Soekarno" adalah seorang "Presiden" dari negara "Indonesia"), bukan hanya mencocokkan kata.
- Jawaban langsung (bukan hanya daftar link): seperti panel info di Google Search yang menampilkan fakta ringkas tentang suatu entitas.
- Disambiguasi entitas: membedakan makna kata yang sama (misalnya "Apple" perusahaan vs. buah apel).
- Penalaran dan inferensi: AI dapat menarik kesimpulan baru dari relasi yang sudah ada di graph, mendukung sistem tanya-jawab yang lebih cerdas.
- Personalisasi & rekomendasi: dengan memahami relasi antar preferensi pengguna dan entitas lain, sistem dapat memberi rekomendasi yang lebih relevan.
- Mendukung Large Language Model: Knowledge Graph dapat digunakan sebagai sumber fakta terstruktur untuk mengurangi halusinasi pada model AI generatif, karena AI bisa memverifikasi jawabannya terhadap data terstruktur yang valid.
