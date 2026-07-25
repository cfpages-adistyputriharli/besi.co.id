---
article_id: BES-04-A03
title: "INP, UNP, dan CNP: Kanal yang Tidak Boleh Dipertukarkan dari Nama"
slug: "inp-unp-dan-cnp"
description: "Explain geometry, symmetry, lips, production route, axes, connection access, and torsional implications conceptually"
status: draft
publication_date: "2025-10-07"
publication_date_basis: editorial_backfill
date_modified: null
parent_topic: BES-04
primary_intent: "Compare channel profiles"
reader_community: "Besi.co.id"
reader_address: "Sobat Besi.co.id"
final_route: "/artikel/inp-unp-dan-cnp.html"
technical_review: required
sources:
  - "https://www.iso.org/standard/52949.html"
  - "https://www.iso.org/standard/73841.html"
  - "https://www.aisc.org/globalassets/aisc/manual/v15.0-shapes-database/naming-convention-for-structural-steel-products-for-use-in-electronic-data-interchange-edi.pdf"
  - "https://peraturan.bpk.go.id/Home/Details/161846/pp-no-16-tahun-2021"
  - "https://pesta.bsn.go.id/produk/detail/12882-sni17292020"
  - "https://pesta.bsn.go.id/produk/detail/12885-sni83692020"
---

# INP, UNP, dan CNP: Kanal yang Tidak Boleh Dipertukarkan dari Nama

Halo, Sobat Besi.co.id!

INP, UNP, dan CNP sama-sama kerap disebut “kanal”, tetapi sebutan itu bukan izin untuk saling menggantikan. Sebelum memilih atau menerima penggantian, baca penampang aktualnya, arah sumbu, ketebalan, cara dibuat, detail sambungan, serta data produk yang menyertainya. Nama dagang atau tinggi yang tampak mirip tidak membuktikan mutu, toleransi, kapasitas, maupun kesetaraan fungsi.

Jawaban singkatnya: INP, UNP, dan CNP harus diperlakukan sebagai keluarga profil yang berbeda sampai gambar, spesifikasi proyek, dan perancang yang berwenang menyatakan lain. Bentuk penampang mengubah letak material, akses baut atau las, dan kecenderungan elemen berputar atau melenting. Keputusan akhirnya dapat berubah oleh bentang, beban, pengekangan, sambungan, material, dan kondisi sementara saat pemasangan—semuanya perlu ditinjau pada proyek yang nyata.

![Ilustrasi INP 6](/wp-content/uploads/2024/01/INP-6.jpg)

_Aset lokal proyek._

<!-- BEGIN MANAGED IMAGE PLAN
## Image plan

- **Image ID:** `LOCAL-007`
- **Source type:** `local`
- **Placement:** after the opening has answered the main question, before the first detailed H2
- **Exact Markdown to insert:** `![Ilustrasi INP 6](/wp-content/uploads/2024/01/INP-6.jpg)`
- **Caption/credit:** Aset lokal proyek; jangan klaim sebagai dokumentasi proyek tertentu.
- **Selection basis:** filename/source metadata identifies `INP 6` as relevant content media; no pixels were inspected.
- **Hard boundary:** do not infer or describe unseen visual details, project ownership, location, people, brands, condition, performance, or outcome.
- **Substitution rule:** do not replace this image. If unavailable or provenance is incomplete, insert `[NEEDS IMAGE REVIEW: LOCAL-007]` and continue drafting the prose.
END MANAGED IMAGE PLAN -->

## Jawaban singkat dan salah paham utama

Kesalahan yang paling mahal biasanya muncul ketika pembelian atau detail gambar memakai kalimat, “ukurannya hampir sama, jadi pakai yang tersedia saja.” Hampir sama pada tinggi nominal tidak menjawab pertanyaan penting: apakah kedua sayap simetris, adakah bibir pengaku, di sisi mana bidang sambungan berada, dan bagaimana profil itu ditahan terhadap putar. Bahkan istilah bentuk produk sendiri perlu dipisahkan dari informasi mutu dan pengadaannya. [ISO 6929:2013](https://www.iso.org/standard/52949.html) membahas kosakata produk baja; kosakata tidak otomatis menetapkan grade, komposisi, toleransi, atau kelayakan untuk satu pekerjaan.

Karena itu, jangan mulai dari nama. Mulailah dari potongan penampang dan dokumen. Jika ada usulan substitusi, hentikan pelepasan material sampai tersedia gambar profil berdimensi, berat per meter yang dirujuk, standar/grade, sertifikat material bila dipersyaratkan, dan persetujuan pihak yang berwenang. Ini bukan berarti semua kanal pasti tidak boleh dipakai pada fungsi yang sama; artinya kesetaraan harus dibuktikan, bukan diasumsikan.

## Definisi dan batas objek

Dalam percakapan pasar, UNP lazim dipakai untuk profil kanal terbuka hasil canai dengan badan dan dua sayap. CNP lazim menunjuk kanal dari pelat tipis yang dibentuk dingin, sering dengan bibir pada tepi sayap. INP juga dipakai sebagai nama dagang/penamaan profil tertentu; bentuk aktualnya perlu dibaca dari tabel produk atau gambar pemasok, bukan ditebak dari singkatannya. Penamaan produk struktural yang baik memang perlu diurai menjadi geometri dan data pendukungnya, bukan hanya labelnya, sebagaimana terlihat pada [konvensi penamaan produk struktural AISC](https://www.aisc.org/globalassets/aisc/manual/v15.0-shapes-database/naming-convention-for-structural-steel-products-for-use-in-electronic-data-interchange-edi.pdf). Contoh tersebut bersifat ilustratif, bukan aturan pasokan Indonesia.

Yang dibahas di sini adalah cara membedakan bentuk dan konsekuensi detailnya secara konseptual. Artikel ini tidak menghitung ukuran kanal, memilih ketebalan, menetapkan jarak gording, atau menyetujui penggantian profil. Untuk pekerjaan struktur, hubungan antara aturan bangunan, desain, standar produk, fabrikasi, dan pemeriksaan tidak bisa digantikan oleh satu halaman produk atau satu tabel ukuran. Status [PP 16 Tahun 2021](https://peraturan.bpk.go.id/Home/Details/161846/pp-no-16-tahun-2021) pun bukan pengganti perhitungan dan persetujuan desain proyek.

## Cara kerjanya

Bayangkan penampang sebagai peta tempat baja ditempatkan. Pada kanal terbuka, badan menjadi jalur utama di tengah, sementara sayap menjulur ke satu arah. Jika kedua sayap dan badan tersusun simetris terhadap satu sumbu, perilakunya tetap harus dibaca terhadap dua sumbu utama penampang. Jika ada bibir pada ujung sayap, material tambahan itu dapat membantu menjaga bentuk elemen tipis secara lokal, tetapi juga mengubah detail lipatan, ruang baut, dan orientasi pemasangan.

Produksi turut penting. Profil canai panas dan profil bentuk dingin bukan sekadar dua rupa yang kebetulan menyerupai kanal. Jalur pembuatannya, ketebalan yang umum, detail tepi, serta standar produk yang relevan dapat berbeda. [ISO 630-1:2021](https://www.iso.org/standard/73841.html) sendiri diposisikan sebagai kondisi pengiriman umum untuk produk struktur canai panas; dokumen itu tidak boleh dipakai untuk menyamakan seluruh produk kanal, seluruh grade, atau seluruh produk bentuk dingin.

Saat detailer menempatkan kanal, orientasi bukan hiasan gambar. Membalik bukaan profil dapat memindahkan bidang yang mudah dijangkau untuk baut, pelat sambung, atau las. Membuat sepasang kanal juga tidak otomatis menyelesaikan persoalan: jarak antarprofil, pelat pengikat, pengaku, posisi sambungan, dan pengekangan menentukan apakah pasangan itu benar-benar bekerja seperti yang dimaksud. Kawan Besi.co.id, setiap perubahan orientasi perlu kembali ke gambar dan detail sambungan, bukan hanya ke foto stok material.

Kanal terbuka juga tidak memiliki simetri putar seperti penampang tertutup. Pada kondisi tertentu, gaya yang tidak melalui pusat geser, pengekangan yang kurang, atau sambungan yang eksentrik dapat memicu kecenderungan puntir. Ini adalah alasan untuk meminta pemeriksaan desain, bukan alasan untuk menyimpulkan bahwa satu profil selalu buruk atau selalu lebih kuat daripada yang lain. Data desain baja dan data desain bentuk dingin berada pada jalur standar yang berbeda, terlihat dari catatan [SNI 1729:2020](https://pesta.bsn.go.id/produk/detail/12882-sni17292020) dan [SNI 8369:2020](https://pesta.bsn.go.id/produk/detail/12885-sni83692020); gunakan naskah lengkap dan ketentuan proyek melalui perancang yang kompeten.

## Faktor yang mengubah hasil

Satu penampang tidak pernah berdiri sendiri. Sebelum menyebut dua kanal dapat dipertukarkan, cek setidaknya hal berikut:

- ukuran lengkap: tinggi, lebar sayap, tebal badan, tebal sayap, radius/lipatan, dan bibir bila ada;
- sumbu dan orientasi elemen terhadap beban serta pengekangannya;
- panjang tak tertahan, posisi tumpuan, sambungan, lubang, las, dan pelat tambahan;
- jenis produk, standar, grade, kondisi suplai, penandaan, dan sertifikat yang diminta;
- tahap pengangkutan dan ereksi, termasuk kondisi ketika pengekangan akhir belum terpasang.

Daftar itu sengaja tidak berisi angka desain. Angka yang aman pada satu proyek dapat keliru pada proyek lain karena bentang, beban, kombinasi pembebanan, lingkungan, dan detailnya berubah. Teman Besi.co.id, bila informasi tersebut belum ada, jangan membeli atau memasang profil sebagai pengganti sebelum data penampang, spesifikasi material, detail sambungan, dan perhitungan proyek ditinjau.

## Contoh keputusan praktis

Berikut bukan tabel kapasitas, melainkan cara menyaring keputusan agar tidak berhenti di nama profil.

| Situasi | Pertanyaan yang harus dijawab | Tindakan aman |
|---|---|---|
| Pemasok menawarkan profil lain dengan tinggi serupa | Apakah bentuk, tebal, massa, grade, dan toleransinya setara menurut dokumen? | Minta datasheet, gambar berdimensi, dan persetujuan tertulis perancang. |
| Kanal akan dibaut ke pelat | Di sisi mana baut dapat dipasang dan apakah bibir/radius mengganggu pelat atau alat? | Buat detail sambungan sesuai profil aktual; jangan menyalin detail dari profil lain. |
| Kanal dipakai sebagai elemen tipis berulang | Bagaimana pengekangan, jarak pengaku, dan kondisi saat pemasangan? | Tinjau dengan metode dan standar yang relevan untuk sistem tersebut. |
| Kanal dipasang berpasangan | Bagaimana pengikat, jarak, dan jalur gaya bekerja? | Jangan menyamakannya dengan satu profil lain tanpa desain dan detail yang disetujui. |

Jika kebutuhan berikutnya hanya memahami ketersediaan kanal terbuka, halaman [profil UNP](/unp) dapat menjadi titik awal untuk mengenali produk yang ditawarkan. Namun halaman produk bukan surat persetujuan substitusi. Sobat Besi.co.id tetap perlu menyandingkan penawaran dengan dokumen proyek yang sedang dikerjakan.

## Kesalahan umum dan cara memeriksanya

Shortcut yang realistis adalah memilih berdasarkan tinggi nominal dan harga per batang. Cara itu gagal karena dua profil yang sama-sama “100” misalnya dapat memiliki lebar, tebal, bibir, massa, toleransi, dan jalur pembentukan yang berbeda. Akibatnya, sambungan yang semula muat bisa tidak dapat dirakit, atau elemen yang diasumsikan tertahan bisa bekerja dengan kondisi yang lain.

Kesalahan kedua adalah memakai satu sertifikat atau satu label untuk menutup seluruh pertanyaan. Sertifikat perlu diperiksa keterkaitannya dengan produk yang diterima; label perlu dibaca bersama standar, grade, kondisi suplai, ukuran, dan jumlahnya. Kesalahan ketiga adalah menganggap perancang hanya diperlukan setelah ada masalah. Justru perubahan material, orientasi, lubang, atau sambungan perlu dinaikkan sebelum fabrikasi dan pemasangan.

Gunakan pemeriksaan singkat ini: cocokkan tanda pada material dengan pesanan; ukur dimensi yang relevan; bandingkan dengan gambar/detail; pastikan tidak ada bibir atau radius yang terlewat; lalu ajukan penyimpangan tertulis kepada perancang atau pengawas yang ditetapkan proyek. Jangan mengisi kekosongan data dengan label INP, UNP, atau CNP saja.

## Langkah berikutnya sebelum memilih kanal

INP, UNP, dan CNP tidak boleh dipertukarkan dari nama karena penampang, proses pembentukan, akses sambungan, dan respons terhadap orientasi dapat berbeda. Ambil gambar profil aktual serta spesifikasi pengadaan terlebih dahulu, lalu cocokkan dengan gambar kerja dan detail sambungan. Untuk keputusan ukuran, kapasitas, atau substitusi, minta tinjauan perancang yang kompeten dengan data proyek lengkap.

Aturan operasinya sederhana: bila bukti kesetaraan belum tertulis, perlakukan profil pengganti sebagai perubahan desain—bukan sebagai penggantian barang biasa.
