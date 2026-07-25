---
article_id: BES-03-A05
title: "Section Properties: Area, Inersia, Modulus, dan Radius Gyration"
slug: "memahami-section-properties-baja"
description: "Explain what area, centroid, moments of inertia, section modulus, torsion-related data, and radius of gyration represent"
status: draft
publication_date: "2025-09-23"
publication_date_basis: editorial_backfill
date_modified: null
parent_topic: BES-03
primary_intent: "Understand section-table fields"
reader_community: "Besi.co.id"
reader_address: "Kawan Besi.co.id"
final_route: "/artikel/memahami-section-properties-baja.html"
technical_review: required
sources:
  - "https://www.iso.org/standard/78322.html"
  - "https://www.iso.org/standard/72529.html"
  - "https://www.iso.org/standard/9985.html"
  - "https://www.asme.org/codes-standards/find-codes-standards/welded-and-seamless-wrought-steel-pipe"
---

# Section Properties: Area, Inersia, Modulus, dan Radius Gyration

Halo, Kawan Besi.co.id! Saat membuka tabel profil baja, angka `A`, `Ix`, `Iy`, `Sx`, `Sy`, dan `r` mudah terlihat seperti daftar spesifikasi yang bisa langsung dipilih. Padahal tiap angka menjawab pertanyaan yang berbeda: berapa banyak material pada penampang, di mana pusatnya, seberapa jauh material tersebar terhadap sumbu, dan seberapa efisien bentuk itu terhadap jenis pembebanan tertentu.

Jawaban singkatnya: *area* dipakai untuk membaca luas penampang; titik berat (*centroid*) menjadi acuan posisi geometri; momen inersia menunjukkan sebaran area terhadap suatu sumbu; modulus penampang menghubungkan geometri dengan tegangan lentur secara konseptual; sedangkan radius gyration merangkum sebaran area dalam satu panjang karakteristik. Data torsi, bila tersedia, berkaitan dengan respons penampang terhadap puntir. Semua itu adalah data geometri penampang, bukan putusan bahwa batang tertentu aman, tersedia, atau sudah memenuhi desain proyek.

Angka tabel hanya layak dipakai bila profil, dimensi aktual, satuan, sumbu, dan edisi tabelnya cocok dengan dokumen pekerjaan. Untuk memutus kapasitas, sambungan, stabilitas batang, atau penerimaan material, diperlukan data proyek dan pemeriksaan oleh pihak kompeten. **[NEEDS TECHNICAL REVIEW: verifikasi profil, beban, kondisi tumpuan, material, dan kriteria desain sebelum section properties dipakai sebagai dasar keputusan struktur.]**

![Ilustrasi besi baja 1](/wp-content/uploads/2024/01/besi-baja-1.jpg)

*Aset lokal proyek; bukan dokumentasi proyek tertentu.*

<!-- BEGIN MANAGED IMAGE PLAN
## Image plan

- **Image ID:** `LOCAL-001`
- **Source type:** `local`
- **Placement:** after the opening has answered the main question, before the first detailed H2
- **Exact Markdown to insert:** `![Ilustrasi besi baja 1](/wp-content/uploads/2024/01/besi-baja-1.jpg)`
- **Caption/credit:** Aset lokal proyek; bukan dokumentasi proyek tertentu.
- **Selection basis:** filename/source metadata identifies `besi baja 1` as relevant content media; no pixels were inspected.
- **Hard boundary:** do not infer or describe unseen visual details, project ownership, location, people, brands, condition, performance, or outcome.
- **Substitution rule:** do not replace this image. If unavailable or provenance is incomplete, insert `[NEEDS IMAGE REVIEW: LOCAL-001]` and continue drafting the prose.
END MANAGED IMAGE PLAN -->

## Jawaban singkat dan salah paham utama

Salah paham yang paling mahal adalah menganggap profil dengan `Ix` lebih besar selalu lebih baik. Lebih besar terhadap sumbu mana? Untuk penampang yang sama, `Ix` dan `Iy` dapat sangat berbeda. Arah profil saat dipasang, arah lentur, panjang batang, pengaku, sambungan, serta beban yang benar-benar bekerja menentukan apakah angka itu relevan.

Demikian juga, luas yang besar tidak otomatis berarti profil cocok untuk semua fungsi. Luas memberi tahu jumlah penampang geometris; ia bukan pengganti pemeriksaan lentur, tekan, tarik, geser, tekuk, atau torsi. Gunakan tabel sebagai bahasa untuk membandingkan bentuk pada tahap pemahaman dan penyiapan data, bukan sebagai stempel kelayakan.

## Definisi dan batas objek

Section properties adalah sifat yang dihitung dari bentuk dan ukuran penampang melintang. Bayangkan Anda memotong batang tepat tegak lurus arah panjangnya: bentuk hasil potongan itulah yang dibaca tabel. Nilainya berubah bila tebal, diameter, lebar sayap, orientasi, lubang, atau detail bentuk berubah.

Berikut arti kolom yang umum ditemui.

| Kolom | Arti praktis | Pertanyaan yang dijawab |
| --- | --- | --- |
| `A` (area) | Luas penampang | Seberapa besar area geometris yang tersedia? |
| Centroid | Titik pusat geometri area | Dari mana jarak terhadap sumbu diukur? |
| `Ix`, `Iy` | Momen inersia area terhadap sumbu x atau y | Seberapa tersebar area terhadap sumbu tersebut? |
| `Sx`, `Sy` | Modulus penampang elastis terhadap sumbu | Bagaimana geometri penampang dikaitkan dengan lentur terhadap sumbu itu? |
| `rx`, `ry` | Radius gyration terhadap sumbu | Seberapa menyebar area bila diringkas sebagai panjang karakteristik? |
| Data torsi | Parameter puntir yang didefinisikan tabel | Bagaimana bentuk itu dicatat untuk evaluasi puntir? |

Istilah “momen inersia” di sini berarti *second moment of area*, bukan massa benda yang berputar. `Ix` dan `Iy` selalu perlu dibaca bersama gambar sumbu dari sumber tabel. Kawan Besi.co.id, jangan menebak sumbu dari hurufnya saja: produsen, perangkat lunak, atau tabel dapat memakai konvensi gambar yang berbeda.

Batas pentingnya jelas: artikel ini menjelaskan cara membaca kolom tabel, bukan menghitung kapasitas struktur. Nilai pada tabel tidak menggantikan gambar kerja, spesifikasi material, maupun verifikasi engineer yang bertanggung jawab.

## Cara kerjanya

Area adalah titik awal. Jika area dibagi-bagi menjadi elemen kecil, centroid adalah lokasi rata-rata geometris dari seluruh elemen itu. Setelah sumbu melalui centroid dipilih, setiap elemen area memiliki jarak terhadap sumbu. Momen inersia menjumlahkan area-area kecil dengan pengaruh jarak kuadratnya. Karena jarak dikuadratkan, material yang ditempatkan lebih jauh dari sumbu memberi perubahan besar pada `I`.

Itulah sebabnya dua penampang dengan luas yang mirip dapat memiliki nilai inersia yang jauh berbeda. Bentuk I, misalnya, menempatkan sebagian area jauh dari sumbu utamanya; tabung atau kotak memiliki distribusi lain; batang bulat penuh berbeda lagi. Penjelasan ini bukan alasan untuk memilih bentuk tanpa perhitungan, tetapi membantu memahami mengapa bentuk, bukan sekadar berat, masuk ke diskusi desain.

Modulus penampang elastis biasanya berasal dari hubungan `S = I/c`, dengan `c` sebagai jarak dari sumbu netral ke serat terluar yang ditinjau. Ini membuat `Sx` dan `Sy` tetap bergantung pada sumbu dan arah lentur. Radius gyration mengikuti hubungan `r = √(I/A)`; ia berguna sebagai ringkasan hubungan antara area dan sebarannya, sehingga tidak boleh dilepaskan dari sumbu `x` atau `y` yang menyertainya.

Untuk pipa, jangan menyamakan nama nominal dengan geometri yang dipakai tabel. Standar dimensi tabung baja dan standar pipa mencakup sistem penamaan/dimensi masing-masing; pemilihan harus kembali ke dokumen produk yang berlaku, bukan menyulap satu label menjadi ukuran aktual. Lihat ruang lingkup [ISO 4200](https://www.iso.org/standard/9985.html) dan [ASME B36.10](https://www.asme.org/codes-standards/find-codes-standards/welded-and-seamless-wrought-steel-pipe) sebelum menyamakan tabel pipa yang berbeda.

## Faktor yang mengubah hasil

Pertama, cek identitas profil. Nama dagang, seri, atau ukuran nominal belum tentu cukup untuk membuktikan dimensi penampang yang dipakai dalam perhitungan tabel. Kedua, cek satuan: luas dapat dicetak dalam mm² atau cm², sementara `I` membawa satuan panjang pangkat empat dan `S` panjang pangkat tiga. Salah konversi kecil dapat membesar dampaknya pada pembacaan.

Ketiga, cek kondisi geometri. Tabel umumnya berangkat dari bentuk ideal dan aturan pembulatan tertentu. Pemotongan, lubang, pelat tambahan, korosi, deformasi, atau konfigurasi rakitan dapat membuat penampang aktual berbeda dari baris tabel. Teman Besi.co.id, ketika perbedaan itu memengaruhi keputusan, jangan “mengoreksi dengan kira-kira”; hentikan keputusan dan cocokkan dengan gambar serta prosedur yang disetujui.

Keempat, pisahkan data geometri dari bukti mutu material. Metode uji tarik dan aturan pengambilan contoh menjelaskan bagaimana hasil uji dikaitkan dengan spesimen dan identitasnya; metode itu sendiri bukan bukti bahwa seluruh stok atau elemen terpasang memenuhi syarat. Rujuk [ISO 6892-1](https://www.iso.org/standard/78322.html) dan [ISO 377](https://www.iso.org/standard/72529.html) untuk ruang lingkup pengujian dan sampel baja. **[NEEDS EVIDENCE REVIEW: sertifikat material, identitas heat/produk, metode, dan catatan penerimaan yang berlaku sebelum nilai material dipakai untuk keputusan proyek.]**

## Contoh keputusan praktis

Misalkan Anda menerima dua kandidat profil dari tabel pemasok untuk sebuah anggota lurus. Langkah aman bukan memilih yang beratnya paling rendah atau `Ix`-nya paling tinggi secara otomatis. Gunakan urutan berikut sebagai pembicaraan awal dengan perencana atau pemeriksa teknis.

1. Tetapkan fungsi anggota dan arah gaya yang sedang ditinjau.
2. Pastikan orientasi profil dan sumbu tabel yang bersesuaian.
3. Catat `A`, `Ix`/`Iy`, `Sx`/`Sy`, `rx`/`ry`, serta parameter torsi yang memang diminta oleh metode desain.
4. Cocokkan dimensi dan satuannya dengan gambar, spesifikasi, dan data produk yang disetujui.
5. Serahkan data itu untuk pemeriksaan kapasitas dan stabilitas; jangan membuat keputusan pemasangan dari tabel saja.

Contoh lain adalah pipa yang tampak memiliki diameter nominal sama. Nilai area dan inersianya dapat berbeda bila ketebalan dinding berbeda. Karena itu, pertanyaan yang lebih berguna bukan “diameternya sama, kan?”, melainkan “tabel mana yang dipakai, berapa geometri rujukannya, dan apakah produk yang diterima sesuai?” Sobat Besi.co.id, jawaban itu juga membantu memisahkan berat teoretis dari hasil timbang aktual; keduanya merupakan pemeriksaan yang berbeda.

## Kesalahan umum dan cara memeriksanya

Shortcut yang sering muncul adalah menyalin satu baris tabel ke spreadsheet lalu menganggap seluruh pekerjaan selesai. Cara itu gagal bila sumber tabel memakai satuan, sumbu, atau bentuk produk yang tidak sama dengan kebutuhan proyek. Ia juga gagal bila profil aktual telah diberi lubang atau dirakit dengan elemen lain.

Ubah shortcut itu menjadi pemeriksaan singkat berikut.

- Apakah judul kolom dan diagram sumbu berasal dari tabel yang sama?
- Apakah ukuran, tebal, dan bentuk produk yang diterima cocok dengan baris tabel?
- Apakah satuan `A`, `I`, `S`, dan `r` sudah konsisten dengan lembar kerja?
- Apakah properti yang dipakai adalah untuk arah pembebanan yang sedang ditinjau?
- Apakah ada perubahan geometri yang harus ditinjau ulang oleh pihak kompeten?
- Apakah dokumen mutu dan identitas produk tersedia bila keputusan bergantung pada mutu material?

Jangan pula menganggap data torsi selalu dapat dipertukarkan. Parameter puntir untuk penampang terbuka, tertutup, atau rakitan dapat mempunyai definisi dan batas penggunaan yang berbeda menurut metode yang dipakai. Bila desain memerlukan evaluasi torsi atau kombinasi perilaku yang lebih kompleks, **[NEEDS TECHNICAL REVIEW: gunakan metode desain dan data penampang yang disetujui untuk bentuk serta kondisi tumpuan aktual.]**

## Langkah berikutnya

Section properties adalah peta geometri: `A` membaca luas, centroid menetapkan acuan, `I` membaca sebaran area, `S` merangkum geometri untuk pembacaan lentur, dan `r` merangkum sebaran area terhadap sumbu. Data itu membuat percakapan teknis lebih rapi, tetapi tidak sendirian menjawab apakah sebuah elemen aman atau dapat diterima.

Langkah berikutnya adalah ambil satu baris tabel profil yang akan dipakai, simpan diagram sumbunya, lalu cocokkan ukuran dan satuannya dengan gambar serta dokumen produk. Kawan Besi.co.id, bila hasilnya akan memengaruhi pemilihan, fabrikasi, atau pemasangan, minta pihak kompeten meninjau data dan asumsi desainnya. Aturan operasinya: baca section properties sebagai data geometri yang dapat ditelusuri, bukan sebagai persetujuan struktur.
