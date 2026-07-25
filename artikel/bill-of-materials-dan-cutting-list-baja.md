---
article_id: BES-13-A02
title: "Membuat Bill of Materials dan Cutting List yang Bisa Diaudit"
slug: "bill-of-materials-dan-cutting-list-baja"
description: "Link item IDs, grade, section/plate, dimensions, quantity, theoretical mass, cut allowance, stock plan, revisions, and remnants"
status: draft
publication_date: "2026-05-04"
publication_date_basis: editorial_backfill
date_modified: null
parent_topic: BES-13
primary_intent: "Build auditable quantities"
reader_community: "Besi.co.id"
reader_address: "Sobat Besi.co.id"
final_route: "/artikel/bill-of-materials-dan-cutting-list-baja.html"
technical_review: required
sources:
  - "https://pesta.bsn.go.id/faq"
  - "https://pesta.bsn.go.id/produk/by_ics?ics_no=91.080.10&key="
  - "https://www.iso.org/standard/9985.html"
  - "https://www.iso.org/standard/72532.html"
  - "https://www.iso.org/standard/85464.html"
  - "https://worldsteel.org/wider-sustainability/circular-economy/"
---

# Membuat Bill of Materials dan Cutting List yang Bisa Diaudit

Halo, Sobat Besi.co.id! Bill of Materials (BOM) dan cutting list yang bisa diaudit bukan sekadar daftar panjang material. Keduanya harus membuat orang lain dapat menelusuri setiap baris: dari item pada gambar yang berlaku, ke spesifikasi dan panjang potongnya, lalu ke kebutuhan stok, sisa, serta perubahan yang pernah terjadi.

Jawaban praktisnya: beri identitas unik pada setiap item, simpan dasar ukur dan asumsi massa secara jelas, pisahkan kebutuhan desain dari rencana pemotongan, lalu kendalikan revisi. Bila satu sambungan itu putus, estimator, pembelian, gudang, dan fabrikator dapat memakai angka yang berbeda untuk benda yang sama. Hasil akhirnya mungkin tampak rapi, tetapi tidak dapat diperiksa ulang.

Isi BOM dapat berubah bila gambar revisi, spesifikasi kontrak, bentuk produk yang benar-benar dipesan, panjang stok pemasok, atau metode fabrikasi berubah. Karena itu daftar ini bukan pengganti persetujuan gambar, optimasi fabrikasi, atau keputusan engineer proyek; ia adalah jejak kuantitas yang harus diperbarui setelah dasar keputusan tersebut jelas.

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

![Ilustrasi besi baja 1](/wp-content/uploads/2024/01/besi-baja-1.jpg)

Kredit gambar: aset lokal proyek.

## Jawaban singkat dan salah paham utama

Kesalahan paling mahal adalah menganggap BOM sama dengan pesanan pembelian, atau cutting list sama dengan gambar kerja. BOM menjawab **apa dan berapa** yang diperlukan menurut basis dokumen tertentu. Cutting list menjawab **bagaimana ukuran bersih itu diterjemahkan menjadi potongan dari stok tertentu**. Pesanan baru boleh dibuat setelah spesifikasi, persetujuan, dan aturan pengadaan proyek dipastikan.

Audit tidak berarti setiap angka selalu benar untuk semua keadaan. Audit berarti pemeriksa dapat menjawab empat pertanyaan: dari dokumen mana angka ini datang, siapa yang menghitung, asumsi apa yang dipakai, dan revisi apa yang menggantikannya. Jika jawaban itu tidak tersedia, angka massa yang sangat presisi pun tidak cukup membantu.

## Definisi dan batas objek

BOM yang baik adalah daftar kebutuhan material terstruktur. Minimal, satu barisnya menghubungkan item ID, elemen atau zona, grade atau spesifikasi, bentuk produk, dimensi rujukan, jumlah, satuan, panjang atau luas bila relevan, serta massa teoretis. Tambahkan kolom status dan rujukan gambar agar baris itu tidak terlepas dari asalnya.

Cutting list adalah turunan operasionalnya. Ia memakai item ID yang sama, lalu mencatat ukuran potong, jumlah potong, allowance pemotongan, batang atau pelat stok asal, dan sisa yang dihasilkan. *Cut allowance* adalah tambahan atau pengurang yang diputuskan untuk proses potong; nilainya tidak boleh disalin otomatis dari proyek lain tanpa metode, mesin, dan toleransi yang disetujui.

Massa teoretis bukan berat timbang aktual maupun dasar tagihan dengan sendirinya. Untuk produk yang memakai tabel dimensi dan massa, nilai itu bergantung pada geometri, panjang, asumsi densitas, tabel rujukan, dan pembulatan yang dipakai. Penerimaan material dan penimbangan aktual adalah pemeriksaan terpisah. [ISO 4200](https://www.iso.org/standard/9985.html) menunjukkan contoh standar yang membahas dimensi dan massa pipa baja; penggunaannya tetap harus mengikuti edisi dan syarat pasok yang ditetapkan proyek.

Daftar ini juga tidak menyetujui gambar atau memilih pola pemotongan paling hemat. Keputusan desain, detail sambungan, urutan fabrikasi, dan optimasi pemotongan dapat mengubah kebutuhannya. Catat perubahan itu sebagai revisi, jangan menyembunyikannya dengan menimpa angka lama.

## Cara kerjanya

Mulailah dengan register dokumen: nomor gambar, revisi, tanggal penerimaan, dan status penggunaannya. Hanya gambar yang ditetapkan tim proyek sebagai basis take-off yang masuk ke BOM. Setelah itu, pecah setiap elemen menjadi item yang dapat dipesan atau dipotong tanpa mengubah identitasnya. Satu jenis profil pada beberapa lokasi boleh memiliki beberapa item ID bila panjang, grade, atau perlakuan akhirnya berbeda.

Kemudian lakukan urutan berikut.

1. Buat item ID yang tidak berubah saat data lain direvisi, misalnya `B-042`.
2. Rekam sumbernya: nomor gambar, detail, grid atau zona, dan revisi.
3. Isi spesifikasi yang benar-benar tertulis: bentuk produk, grade, ukuran, dan satuan. Jangan menerjemahkan nama dagang menjadi grade tanpa dokumen pemasok atau spesifikasi yang berlaku.
4. Hitung kuantitas desain dan massa teoretis dengan rumus, tabel, serta aturan pembulatan yang dicatat.
5. Salin hanya item yang siap diproses ke cutting list, lengkap dengan ukuran potong bersih dan allowance yang disetujui.
6. Hubungkan potongan ke stok rencana dan beri ID sisa untuk remnant yang masih mungkin dipakai kembali.
7. Terbitkan revisi beserta daftar perubahan: item baru, berubah, dibatalkan, atau dipindahkan.

Kawan Besi.co.id, pemisahan antara kebutuhan desain dan rencana stok penting karena satu panjang bersih dapat dibeli dalam beberapa panjang dagang, sedangkan satu batang stok dapat menghasilkan beberapa item. Kolom `stock plan` sebaiknya mencatat bahwa ia rencana, bukan bukti material sudah tersedia. Gudang atau pembelian perlu mengonfirmasi nomor lot, ukuran yang diterima, dan sisa aktual setelah proses berjalan.

Gunakan satu baris kontrol untuk setiap revisi: siapa yang menerbitkan, siapa yang memeriksa, tanggal, alasan perubahan, dan dampaknya pada jumlah. Tanpa kontrol ini, file spreadsheet yang dikirim ulang mudah menciptakan dua versi kebenaran.

## Faktor yang mengubah hasil

Pertama, bentuk produk menentukan data yang dicatat. Profil, pelat, pipa, batang, baut, lapisan, dan kawat las tidak dapat diperlakukan sebagai satu keluarga spesifikasi. Katalog publik BSN dapat membantu menemukan identitas serta ruang lingkup yang tampak, tetapi status pada katalog tidak menetapkan dengan sendirinya edisi yang mengikat, kewajiban regulasi, atau kesesuaian untuk seluruh proyek. [FAQ Pesta Online BSN](https://pesta.bsn.go.id/faq) dan [katalog struktur logam](https://pesta.bsn.go.id/produk/by_ics?ics_no=91.080.10&key=) perlu dilanjutkan dengan pemeriksaan dokumen lengkap, kontrak, amandemen, dan persetujuan yang berlaku.

Kedua, detail proses mengubah cutting list. Kerf, bevel, kampuh, lubang, tekukan, ujung yang perlu dirapikan, serta urutan pemotongan dapat memengaruhi allowance dan sisa. Jangan memasukkan angka allowance sebagai “standar perusahaan” bila belum ada metode kerja atau keputusan proyek yang dapat diperiksa.

Ketiga, identitas material tidak berhenti pada label fisik. Bila proyek mengajukan asal-usul, kandungan daur ulang, atau klaim keberlanjutan, catat karakteristik yang diklaim, batas sistem, pihak yang menyerahkan, dan rekaman transaksi. Kerangka [ISO 22095](https://www.iso.org/standard/72532.html) membedakan model segregasi fisik, mass balance, dan klaim administratif; masing-masing memerlukan jejak bukti yang berbeda. Itu bukan sertifikasi otomatis atas material atau persetujuan struktur.

Keempat, tingkat pemeriksaan harus mengikuti rencana inspeksi yang disetujui. Rencana yang dapat diaudit menyebut lot atau populasi, karakteristik yang diperiksa, metode, identitas sampel, kriteria keputusan, penanggung jawab, serta jalur ketidaksesuaian. Abstrak [ISO 2859-1](https://www.iso.org/standard/85464.html) tidak memberi alasan untuk memilih ukuran sampel atau aturan penerimaan sendiri.

## Contoh keputusan praktis

Bayangkan gambar revisi menambah dua potong pada elemen yang sebelumnya sudah direncanakan dari satu batang stok. Jangan langsung mengubah total pada sel lama. Buat revisi baru yang menyatakan item ID, jumlah sebelum dan sesudah, referensi gambar revisi, serta dampak pada batang stok dan remnant. Dengan begitu pembeli tahu apakah pesanan perlu berubah, dan fabrikator tahu versi daftar mana yang boleh dipakai.

| Keadaan | Catatan BOM | Catatan cutting list | Tindakan aman |
| --- | --- | --- | --- |
| Gambar belum berstatus basis produksi | Tandai sementara dan sumbernya | Jangan lepaskan untuk potong | Minta konfirmasi gambar yang berlaku |
| Panjang bersih sudah jelas, stok belum dipilih | Catat kebutuhan desain | Kosongkan atau tandai rencana | Tetapkan stok setelah data pemasok/produksi tersedia |
| Ada sisa yang ingin dipakai kembali | Catat ID sisa, ukuran terukur, lokasi, dan status | Hubungkan ke potongan baru hanya bila tervalidasi | Verifikasi identitas, kondisi, dan persetujuan penggunaan |
| Material diterima berbeda dari rencana | Jangan menyamakan dengan item awal | Tahan perubahan otomatis | Catat selisih dan ajukan peninjauan yang berwenang |

Teman Besi.co.id, contoh ini sengaja tidak memberi angka panjang, berat, atau allowance. Angka tersebut hanya sah bila berasal dari gambar, standar lengkap, syarat pembelian, dan metode yang memang disetujui untuk pekerjaan Anda.

## Kesalahan umum dan cara memeriksanya

Shortcut yang sering dipilih adalah membuat satu tabel “total kebutuhan” lalu menghapus kolom sumber dan revisi agar mudah dibaca. Ia gagal ketika ada pertanyaan sederhana: total itu berasal dari gambar mana, apakah potongan sudah memasukkan allowance, dan apakah sisa masih tersedia? Tabel ringkas boleh dibuat untuk rapat, tetapi tabel induknya harus tetap dapat ditelusuri.

Sebelum menerbitkan BOM atau cutting list, periksa hal berikut.

- Apakah setiap item memiliki ID, sumber gambar, dan revisi yang jelas?
- Apakah grade, bentuk produk, dimensi, jumlah, satuan, dan basis massa teoretis dibedakan dari hasil timbang aktual?
- Apakah allowance, stok rencana, dan remnant diberi status serta pemilik keputusan?
- Apakah perubahan memiliki tanggal, penerbit, pemeriksa, alasan, dan dampak kuantitas?
- Apakah material yang akan dipakai ulang mempunyai bukti asal, kondisi, geometri, dan persetujuan untuk penggunaan baru?

Menggunakan kembali elemen baja dapat mempertahankan nilai produk, tetapi bukan berarti elemen itu otomatis layak untuk fungsi baru. Riwayat paparan, perubahan, kondisi, bukti material atau kemampuan las, alasan pengujian, dan persetujuan desain dapat diperlukan; [worldsteel](https://worldsteel.org/wider-sustainability/circular-economy/) juga membedakan pemanfaatan kembali dari daur ulang yang tidak mempertahankan identitas komponen.

## Langkah berikutnya

BOM dan cutting list yang dapat diaudit menghubungkan kebutuhan desain, rencana potong, dan perubahan tanpa menyamakan ketiganya. Sobat Besi.co.id, mulai dari satu register dokumen dan satu format item ID, lalu minta pemeriksa proyek menegaskan gambar, spesifikasi, allowance, serta aturan penerimaan yang berlaku sebelum daftar dilepas ke pembelian atau fabrikasi. Aturan operasinya sederhana: bila asal angka atau status revisinya tidak dapat ditunjukkan, jangan perlakukan baris itu sebagai dasar pemesanan atau pemotongan.
