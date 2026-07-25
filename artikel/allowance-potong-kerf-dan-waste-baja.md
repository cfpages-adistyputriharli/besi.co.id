---
article_id: BES-03-A06
title: "Allowance Potong, Kerf, Remnant, dan Waste dalam Takeoff Baja"
slug: "allowance-potong-kerf-dan-waste-baja"
description: "Account for stock length, kerf, end trim, nesting, trial pieces, damage, remnants, and traceability without hiding assumptions"
status: draft
publication_date: "2025-09-28"
publication_date_basis: editorial_backfill
date_modified: null
parent_topic: BES-03
primary_intent: "Plan material takeoff"
reader_community: "Besi.co.id"
reader_address: "Teman Besi.co.id"
final_route: "/artikel/allowance-potong-kerf-dan-waste-baja.html"
technical_review: required
sources:
  - "https://www.iso.org/standard/72529.html"
  - "https://www.iso.org/standard/9985.html"
  - "https://www.iso.org/standard/60321.html"
  - "https://www.iso.org/standard/86032.html"
  - "https://www.iso.org/standard/85464.html"
---

# Allowance Potong, Kerf, Remnant, dan Waste dalam Takeoff Baja

Halo, Teman Besi.co.id! Takeoff baja yang hanya menjumlahkan panjang atau berat item gambar sering terlihat rapi, tetapi belum tentu cukup untuk dipesan atau dipotong. Material datang dalam panjang stok tertentu; tiap potongan dapat memakan kerf; ujung mungkin perlu dirapikan; dan sisa yang masih layak pakai belum tentu cocok untuk kebutuhan berikutnya. Bila semua itu disembunyikan dalam satu angka “waste”, estimator kehilangan jejak alasan selisihnya.

Jawaban singkatnya: pisahkan kebutuhan bersih dari allowance potong, lalu catat kerf, end trim, trial piece, kerusakan, dan remnant sebagai komponen dengan asumsi yang jelas. Hasil takeoff harus menunjukkan kebutuhan bersih, pola pemakaian stok, serta sisa yang dapat atau tidak dapat dipakai kembali—bukan sekadar menaikkan kuantitas tanpa dasar. Angkanya dapat berubah setelah panjang stok pemasok, gambar yang disetujui, metode pemotongan, dan aturan pengendalian sisa proyek tersedia.

![Ilustrasi besi baja 1](/wp-content/uploads/2024/01/besi-baja-1.jpg)

*Aset lokal proyek; bukan dokumentasi proyek tertentu.*

<!-- BEGIN MANAGED IMAGE PLAN
## Image plan

- **Image ID:** `LOCAL-001`
- **Source type:** `local`
- **Placement:** after the opening has answered the main question, before the first detailed H2
- **Exact Markdown to insert:** `![Ilustrasi besi baja 1](/wp-content/uploads/2024/01/besi-baja-1.jpg)`
- **Caption/credit:** Aset lokal proyek; jangan klaim sebagai dokumentasi proyek tertentu.
- **Selection basis:** filename/source metadata identifies `besi baja 1` as relevant content media; no pixels were inspected.
- **Hard boundary:** do not infer or describe unseen visual details, project ownership, location, people, brands, condition, performance, or outcome.
- **Substitution rule:** do not replace this image. If unavailable or provenance is incomplete, insert `[NEEDS IMAGE REVIEW: LOCAL-001]` and continue drafting the prose.
END MANAGED IMAGE PLAN -->

## Jawaban singkat dan salah paham utama

Allowance bukan izin untuk menebak. Ia adalah catatan kebutuhan tambahan yang muncul karena cara material dibeli, dipotong, diinspeksi, dan disimpan. Kerf adalah bagian material yang hilang pada garis potong. End trim adalah bagian ujung yang sengaja tidak dipakai agar ujung atau panjang hasil memenuhi kebutuhan pekerjaan. Remnant adalah sisa yang masih diidentifikasi dan berpeluang dipakai; waste adalah sisa yang memang tidak dapat dipakai untuk kebutuhan yang direncanakan atau tidak layak ditelusuri.

Kesalahan paling mahal adalah menganggap semua sisa sama. Sisa pendek dari profil tertentu mungkin secara fisik masih ada, tetapi tidak otomatis menjadi remnant bernilai bila tidak memiliki tanda identitas, tidak memenuhi panjang minimum berikutnya, atau tidak ada kebutuhan yang cocok. Sebaliknya, menjumlahkan semua sisa sebagai waste sejak awal dapat membuat pembelian berlebih. Jadi pertanyaan pertama bukan “berapa persen waste?”, melainkan “stok mana dipakai untuk item mana, dan sisa apa yang masih terkendali?”

## Definisi dan batas objek

Dalam artikel ini, **kebutuhan bersih** adalah panjang, luas, atau jumlah komponen menurut gambar yang telah menjadi dasar takeoff. **Allowance potong** adalah tambahan yang direncanakan agar kebutuhan bersih dapat diwujudkan dari stok aktual. Tambahan itu dapat memuat kerf, trim, potongan percobaan, bagian rusak yang teridentifikasi, atau ketidakcocokan susunan potong. **Nesting** berarti menyusun beberapa kebutuhan pada satu batang, pelat, atau profil agar pemakaian stok lebih terarah.

Batas pentingnya: artikel ini tidak menetapkan parameter mesin, lebar kerf tertentu, kelas toleransi, atau persentase waste universal. Standar pemotongan termal dan toleransi konstruksi las menautkan hasil pada proses, material, ketebalan, persyaratan gambar, cara ukur, serta fungsi lanjutan; standar umum tidak otomatis berlaku untuk setiap jenis potong atau rakitan. [ISO 9013](https://www.iso.org/standard/60321.html) dan [ISO 13920](https://www.iso.org/standard/86032.html) dapat menjadi rujukan identitas dan ruang lingkup, tetapi nilai penerimaan proyek tetap memerlukan dokumen lengkap dan persetujuan yang berlaku.

Untuk pipa dan profil yang dihitung menurut massa teoretis, jangan samakan label nominal dengan hasil timbang atau penerimaan barang. Massa teoretis bergantung pada geometri, panjang, asumsi densitas, aturan pembulatan, dan tabel produk yang dipakai; pemeriksaan penerimaan dan penimbangan aktual adalah kegiatan terpisah. [ISO 4200](https://www.iso.org/standard/9985.html) mendeskripsikan dimensi dan massa pipa baja, bukan dasar untuk menebak kuantitas tagihan atau kapasitas layanan.

## Cara kerjanya

Mulailah dari daftar potong yang dapat diaudit: identitas item, material atau grade menurut dokumen, ukuran, panjang bersih, jumlah, revisi gambar, dan kebutuhan penandaan. Kelompokkan item yang benar-benar boleh berbagi stok. Setelah itu, masukkan panjang stok yang tercantum pada penawaran atau dokumen penerimaan, bukan panjang yang diingat dari proyek lain.

Susun calon pola potong per batang atau pelat. Untuk setiap pola, tuliskan jumlah potongan bersih, jumlah garis potong, allowance ujung bila disyaratkan, dan sisa akhir. Kerf dicatat per kejadian potong sesuai metode kerja yang disetujui, bukan ditempel sebagai angka persen pada seluruh berat. Bila ada kebutuhan trial piece atau area yang harus disisihkan karena penandaan, pisahkan pula sebagai baris allowance. Dengan begitu, perubahan metode atau gambar hanya mengubah komponen yang terkait.

Lalu beri status pada sisa: **remnant terkendali**, **sisa menunggu keputusan**, atau **waste terencana**. Remnant yang ingin dihitung sebagai kredit persediaan memerlukan lokasi, dimensi aktual, identitas material/heat bila relevan, kondisi, dan aturan siapa yang boleh melepasnya untuk pekerjaan lain. Kawan Besi.co.id, jangan mengurangi pembelian dari remnant yang hanya tercatat “ada sisa” tanpa verifikasi fisik dan penelusuran.

Identitas itu juga penting saat hasil potong akan dikaitkan dengan mutu material. Pengambilan sampel dan benda uji baja harus tetap terkait dengan sumber spesimen dan identitas produk; satu nilai atau nama sifat tidak dengan sendirinya membuktikan kesesuaian seluruh stok. [ISO 377](https://www.iso.org/standard/72529.html) membahas pengambilan dan penyiapan sampel serta benda uji untuk penentuan sifat mekanik baja. Dalam takeoff, prinsip praktisnya adalah: jangan sampai optimasi susunan potong memutus catatan material yang diperlukan oleh spesifikasi proyek.

## Faktor yang mengubah hasil

Hasil takeoff dapat berubah oleh lima kelompok informasi berikut.

| Faktor | Pertanyaan yang perlu dijawab | Dampak pada takeoff |
| --- | --- | --- |
| Stok pemasok | Panjang, lebar, bentuk, dan basis suplai apa yang benar-benar ditawarkan? | Menentukan pola potong yang mungkin dan sisa akhir. |
| Gambar serta revisi | Item mana sudah disetujui dan mana masih berubah? | Menahan pembelian atau pemotongan item yang berisiko menjadi salah. |
| Metode dan fungsi hasil | Bagaimana potong, persiapan tepi, dan pemeriksaannya ditetapkan? | Mengubah kerf, trim, serta kebutuhan penyisihan. |
| Pengendalian remnant | Apakah sisa diberi label, diukur, disimpan, dan boleh dialokasikan ulang? | Menentukan apakah sisa boleh menjadi kredit atau harus diperlakukan konservatif. |
| Pemeriksaan dan bukti | Catatan lot, identitas, kriteria, dan keputusan siapa yang berlaku? | Mencegah kuantitas atau sisa dipakai tanpa dasar penerimaan. |

Tidak ada satu persentase yang aman untuk seluruh proyek. Pelat dengan susunan bentuk berbeda, batang dengan banyak panjang pendek, dan pipa yang membutuhkan orientasi atau penandaan berbeda memiliki sumber kehilangan yang tidak sama. Sobat Besi.co.id, bila informasi ini belum ada, lebih jujur membukukan allowance sebagai asumsi sementara daripada menyajikan angka akhir seolah sudah tervalidasi.

[NEEDS REVIEW: gambar potong yang disetujui, panjang stok pemasok, metode potong, persyaratan penandaan, dan aturan remnant proyek sebelum allowance dibekukan.]

## Contoh keputusan praktis

Misalkan daftar potong membutuhkan beberapa bagian dari satu jenis batang. Estimator tidak perlu langsung memilih angka waste. Ia dapat membuat dua skenario: skenario A memakai panjang stok yang dikonfirmasi pemasok, sedangkan skenario B menunggu alternatif panjang stok. Pada masing-masing skenario, daftar potong memuat panjang bersih item, jumlah garis potong, trim yang diwajibkan, dan sisa per batang. Bagian yang tampak dapat digunakan ulang hanya dicatat sebagai remnant bila memenuhi aturan identifikasi dan kebutuhan minimum yang telah disetujui.

Contoh ini sengaja tidak memakai ukuran atau persen. Tanpa gambar, stok, prosedur, dan kebutuhan penerimaan yang disetujui, angka semacam itu hanya akan memberi kesan presisi palsu. Jika proyek menggunakan keputusan sampling untuk penerimaan, rencana tersebut harus mendefinisikan populasi atau lot, karakteristik yang diperiksa, metode, pemilihan sampel, kriteria keputusan, penanggung jawab, catatan, dan jalur ketidaksesuaian. [ISO 2859-1](https://www.iso.org/standard/85464.html) adalah standar pengambilan sampel atribut lot demi lot; pemilihan ukuran sampel atau aturan penerimaan proyek tetap harus berasal dari dokumen lengkap dan ITP yang disetujui.

Keputusan praktisnya sederhana: pesanan boleh memakai kebutuhan bersih ditambah allowance yang tertulis, tetapi kredit remnant hanya boleh mengurangi kebutuhan bila sisa tersebut nyata, terukur, teridentifikasi, dan tersedia pada saat dipakai. Bila salah satu syarat belum ada, tandai sebagai risiko pengadaan, bukan penghematan yang sudah pasti.

## Kesalahan umum dan cara memeriksanya

Beberapa shortcut terlihat cepat, tetapi biasanya memindahkan masalah ke gudang atau lantai fabrikasi.

- **Menambah satu persen tetap untuk semua item.** Periksa apakah angka itu memisahkan kerf, trim, sisa susunan, dan potongan percobaan. Jika tidak, perubahan satu faktor tidak dapat ditelusuri.
- **Menganggap sisa fisik pasti mengurangi pembelian.** Periksa ukuran aktual, identitas, kondisi, lokasi, dan kebutuhan yang kompatibel sebelum memberi kredit remnant.
- **Menggabungkan material yang namanya mirip.** Periksa referensi gambar, identitas produk/heat bila dipersyaratkan, serta aturan substitusi proyek sebelum satu stok dipakai untuk item lain.
- **Mengunci pesanan saat gambar masih bergerak.** Periksa revisi, tanggal persetujuan, dan item yang menjadi pemicu perubahan pola potong.
- **Memakai hasil potong sebagai bukti mutu seluruh material.** Pisahkan catatan fabrikasi dari dasar penerimaan material dan dari pengujian yang memang disyaratkan.

Shortcut yang paling sering menggoda adalah “tambahkan saja waste agar aman.” Cara itu gagal ketika pembeli, gudang, dan pelaksana tidak tahu cadangan tersebut untuk apa. Alternatif yang lebih andal ialah membuat register allowance: setiap baris menyebut sumber tambahan, dasar asumsi, penanggung jawab konfirmasi, dan kondisi kapan angka harus diperbarui. Teman Besi.co.id, register seperti ini membuat diskusi perubahan lebih cepat daripada mempertahankan angka cadangan yang tidak dapat dijelaskan.

## Aturan kerja sebelum material dipesan

Allowance potong yang baik bukan angka besar atau kecil; ia adalah keputusan yang dapat ditelusuri dari kebutuhan bersih sampai sisa akhir. Pisahkan kerf, trim, trial piece, kerusakan yang diketahui, remnant, dan waste agar pembelian tidak menyembunyikan asumsi. Jangan menggunakan tabel massa atau standar proses sebagai pengganti gambar, kondisi suplai, dan persetujuan proyek.

Sebelum menerbitkan permintaan pembelian, minta daftar potong ber-revisi, panjang stok yang ditawarkan, pola pemakaian stok, register allowance, serta daftar remnant yang telah diverifikasi. Setelah itu, lakukan tinjauan teknis terhadap persyaratan gambar, prosedur, penerimaan, dan traceability yang berlaku. Aturan operasinya: **jika sumber allowance tidak dapat disebutkan dan diverifikasi, jangan menganggapnya sebagai kuantitas final.**
