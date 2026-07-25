---
article_id: BES-10-A05
title: "Distorsi, Residual Stress, dan Sequence Pengelasan"
slug: "distorsi-dan-sequence-pengelasan"
description: "Explain heat/shrinkage, restraint, joint sequence, balance, fit-up, preset/trial, measurement, and controlled correction concepts"
status: draft
publication_date: "2026-03-06"
publication_date_basis: editorial_backfill
date_modified: null
parent_topic: BES-10
primary_intent: "Plan distortion control"
reader_community: "Besi.co.id"
reader_address: "Teman Besi.co.id"
final_route: "/artikel/distorsi-dan-sequence-pengelasan.html"
technical_review: required
sources:
  - "https://www.iso.org/standard/81651.html"
  - "https://www.iso.org/standard/68893.html"
  - "https://www.iso.org/standard/83737.html"
  - "https://cm.aws.org/standards-and-publications/codes-and-standards/d1-1/"
  - "https://www.aws.org/about/get-involved/committees/d1-committee-on-structural-welding/"
  - "https://www.iso.org/standard/85705.html"
  - "https://www.iso.org/standard/75614.html"
  - "https://jdih.pu.go.id/detail-dokumen/PermenPUPR-nomor-10-tahun-2021-Pedoman-Sistem-Manajemen-Keselamatan-Konstruksi"
  - "https://jdih.kemnaker.go.id/peraturan/detail/1546"
  - "https://jdih.kemnaker.go.id/peraturan/detail/1668/peraturan-menteri-nomor-8-tahun-2020"
  - "https://jdih.kemnaker.go.id/peraturan/detail/1210/peraturan-menteri-nomor-9-tahun-2016"
  - "https://jdih.kemnaker.go.id/peraturan/detail/1430/peraturan-menteri-nomor-38-tahun-2016"
  - "https://www.cdc.gov/niosh/welding/about/index.html"
  - "https://www.osha.gov/welding-cutting-brazing/hazards-solutions"
  - "https://www.cdc.gov/niosh/engcontrols/ecd/detail44.html"
---

# Distorsi, Residual Stress, dan Sequence Pengelasan

Halo, Teman Besi.co.id! Frame yang sudah rapi saat *fit-up* dapat berubah melengkung, menyudut, atau tidak lagi siku setelah las mendingin. Jalan keluarnya bukan sekadar menambah clamp atau mengejar bagian yang tampak miring dengan panas. Distorsi perlu direncanakan dari sambungan, pengekangan, urutan kerja, dan cara ukur sebelum pengelasan dimulai.

Jawaban singkatnya: panas las membuat daerah sambungan memuai lalu menyusut saat dingin. Jika penyusutan itu tidak seimbang atau ditahan secara tidak tepat, komponen dapat bergeser dan tegangan sisa (*residual stress*) tertinggal. Sequence pengelasan yang disetujui membantu mengendalikan arah dan akumulasi penyusutan, tetapi bukan resep universal untuk setiap frame.

Pilihan sequence, *preset*, tack, parameter, maupun cara koreksi harus mengikuti prosedur fabrikasi yang disetujui dan kebutuhan proyek. Perubahan penting juga bergantung pada material, detail sambungan, kekangan, dan standar yang berlaku. Sistem mutu pengelasan menuntut persyaratan yang ditetapkan, koordinasi yang kompeten, serta pengendalian pelaksanaan dan rekamannya—bukan pemeriksaan akhir semata ([ISO 3834-2](https://www.iso.org/standard/81651.html), [ISO 14731](https://www.iso.org/standard/68893.html), [ISO 17662](https://www.iso.org/standard/83737.html)).

![Ilustrasi Besi WF 1](/wp-content/uploads/2024/01/Besi-WF-1.jpg)

_Kredit gambar: aset lokal proyek._

<!-- BEGIN MANAGED IMAGE PLAN
## Image plan

- **Image ID:** `LOCAL-003`
- **Source type:** `local`
- **Placement:** after the opening has answered the main question, before the first detailed H2
- **Exact Markdown to insert:** `![Ilustrasi Besi WF 1](/wp-content/uploads/2024/01/Besi-WF-1.jpg)`
- **Caption/credit:** Aset lokal proyek; jangan klaim sebagai dokumentasi proyek tertentu.
- **Selection basis:** filename/source metadata identifies `Besi WF 1` as relevant content media; no pixels were inspected.
- **Hard boundary:** do not infer or describe unseen visual details, project ownership, location, people, brands, condition, performance, or outcome.
- **Substitution rule:** do not replace this image. If unavailable or provenance is incomplete, insert `[NEEDS IMAGE REVIEW: LOCAL-003]` and continue drafting the prose.
END MANAGED IMAGE PLAN -->

## Jawaban singkat dan salah paham utama

Distorsi adalah perubahan bentuk atau posisi yang terlihat setelah siklus panas dan dingin. Tegangan sisa adalah tegangan yang dapat tetap berada di dalam komponen walaupun gaya luar sudah tidak bekerja. Keduanya terkait, tetapi tidak sama: sebuah bagian dapat tampak lurus namun masih menyimpan tegangan sisa; sebaliknya, perubahan bentuk yang terlihat tidak otomatis menjelaskan seluruh kondisi tegangan di dalamnya.

Salah paham yang mahal adalah menganggap frame akan “kembali sendiri” bila las didinginkan. Penyusutan yang terjadi pada satu sisi sambungan dapat menarik bagian itu lebih kuat daripada sisi lain. Karena itu, target praktisnya bukan menjanjikan nol distorsi, melainkan mengendalikan hasil terhadap toleransi, datum ukur, dan urutan yang sudah ditetapkan.

Untuk pekerjaan baja struktural, jangan menganggap satu kode asing otomatis berlaku untuk semua pekerjaan. AWS menjelaskan bahwa D1.1 menjadi mengikat ketika diadopsi oleh kontrak, spesifikasi proyek, atau persyaratan regulator, dan lingkupnya adalah baja struktural ([AWS D1.1/D1.1M](https://cm.aws.org/standards-and-publications/codes-and-standards/d1-1/), [AWS D1 Committee](https://www.aws.org/about/get-involved/committees/d1-committee-on-structural-welding/)).

## Definisi dan batas objek

Pada frame, “objek” pengendalian bukan hanya jalur las. Objeknya mencakup anggota yang akan disambung, posisi datum, gap dan keselarasan saat *fit-up*, tack weld, fixture atau clamp, urutan sambungan, serta titik ukur sebelum dan sesudah pekerjaan. *Fit-up* berarti penyiapan dan penyelarasan komponen sebelum pengelasan; dari sinilah arah penyusutan mulai dapat diperkirakan secara praktis.

*Preset* adalah pengaturan awal posisi atau geometri untuk mengantisipasi perubahan bentuk. *Trial* adalah percobaan terkendali untuk memeriksa apakah asumsi proses menghasilkan geometri yang diterima. Keduanya bukan izin untuk menebak: nilai preset, panjang tack, dan sequence harus berada dalam dokumen yang disetujui atau hasil trial yang ditinjau pihak berwenang.

Halaman ini tidak menetapkan urutan las, parameter panas, metode *straightening*, atau batas penerimaan. [NEEDS REVIEW G-07: konfirmasi standar aplikasi, spesifikasi proyek, material, detail sambungan, dan prosedur pengelasan yang disetujui sebelum sequence dipilih.] Bila pemeriksaan non-destruktif diperlukan, pemilihan metode, cakupan, teknik, kriteria penerimaan, serta kompetensi personelnya juga memerlukan rencana inspeksi yang berlaku ([ISO 17635](https://www.iso.org/standard/85705.html), [ISO 9712](https://www.iso.org/standard/75614.html)).

## Cara kerjanya

Bayangkan satu sambungan pada frame: panas terlokalisasi menaikkan suhu di sekitar las, daerah itu cenderung memuai, lalu menyusut ketika mendingin. Karena bagian sekitarnya lebih dingin dan konstruksi saling terhubung, gerak tersebut tidak bebas sepenuhnya. Perbedaan penyusutan antar sisi, antar sambungan, atau antar tahap pekerjaan dapat muncul sebagai perubahan sudut, lengkung, puntir, atau pergeseran relatif.

Sequence adalah tata urut yang mengatur kapan dan di mana sambungan dikerjakan agar efek tersebut tidak terkumpul sembarangan pada satu arah. Keseimbangan di sini bukan berarti semua sambungan harus selalu identik; artinya pengaruh panas, posisi kerja, kekangan, dan kebutuhan geometri dipertimbangkan sebagai satu sistem. Kawan Besi.co.id, mulai dari pertanyaan sederhana: “Jika sambungan ini menyusut, ke mana anggota akan tertarik, dan datum mana yang harus tetap terlindungi?”

Kekangan pun perlu dipahami dengan hati-hati. Fixture dan clamp dapat menjaga posisi saat pengerjaan, tetapi kekangan yang berlebihan dapat memindahkan masalah menjadi tegangan sisa atau menyulitkan pelepasan. Maka pengendalian yang dapat ditelusuri mencatat kondisi awal, metode penahanan, urutan yang dipakai, pemeriksaan antara, dan hasil ukur. Kalibrasi, verifikasi, dan validasi peralatan merupakan bagian dari rantai kendali mutu, bukan pekerjaan administrasi setelah komponen selesai ([ISO 17662](https://www.iso.org/standard/83737.html)).

## Faktor yang mengubah hasil

Hasil tidak dapat diprediksi dari panjang las saja. Detail sambungan dan geometri anggota menentukan kepekaan terhadap tarik atau puntir. Kondisi *fit-up*—misalnya keselarasan, gap, dan tumpuan—mengubah posisi awal yang akan dipertahankan atau terkoreksi saat siklus panas berlangsung. Urutan tack dan pekerjaan utama juga dapat mengubah jalur transfer gaya di dalam rakitan.

Kemudian ada variabel proses dan organisasi: prosedur yang disetujui, kompetensi pelaksana, kondisi material dan consumable, kondisi peralatan, serta disiplin pemeriksaan antara. ISO 3834-2 menempatkan pengendalian prosedur, personel, peralatan, pelaksanaan, inspeksi, ketidaksesuaian, dan rekaman sebagai unsur mutu pengelasan yang saling terkait ([ISO 3834-2](https://www.iso.org/standard/81651.html)). Tidak ada pemeriksaan akhir yang dapat mengembalikan semua variabel penting yang tidak pernah dicatat saat pekerjaan berlangsung.

Kondisi tempat kerja juga tidak boleh dipisahkan dari keputusan sequence. Pengelasan dapat melibatkan asap, bahaya kebakaran, listrik, gas, posisi kerja, dan pekerja di sekitarnya; penilaian risiko perlu melihat proses, material atau kontaminan, ventilasi, enclosure, serta keadaan darurat ([NIOSH](https://www.cdc.gov/niosh/welding/about/index.html), [OSHA](https://www.osha.gov/welding-cutting-brazing/hazards-solutions)). [NEEDS REVIEW G-12: pastikan penilaian risiko, metode kerja, izin, pengawasan, dan persyaratan K3 proyek/Indonesia diterapkan oleh pihak kompeten.] Rujukan SMKK dan peraturan K3 Indonesia mencakup konteks konstruksi, lingkungan kerja, peralatan angkat-angkut, kerja pada ketinggian, dan mesin produksi ([Permen PUPR 10/2021](https://jdih.pu.go.id/detail-dokumen/PermenPUPR-nomor-10-tahun-2021-Pedoman-Sistem-Manajemen-Keselamatan-Konstruksi), [Permenaker 5/2018](https://jdih.kemnaker.go.id/peraturan/detail/1546), [Permenaker 8/2020](https://jdih.kemnaker.go.id/peraturan/detail/1668/peraturan-menteri-nomor-8-tahun-2020), [Permenaker 9/2016](https://jdih.kemnaker.go.id/peraturan/detail/1210/peraturan-menteri-nomor-9-tahun-2016), [Permenaker 38/2016](https://jdih.kemnaker.go.id/peraturan/detail/1430/peraturan-menteri-nomor-38-tahun-2016)).

## Contoh keputusan praktis

Misalkan sebuah frame sedang dirakit di meja kerja dan satu sisi harus tetap menjadi datum pemasangan. Ini bukan instruksi pengelasan, melainkan cara menyusun keputusan sebelum mulai:

| Pertanyaan sebelum pekerjaan | Bukti atau tindakan yang dicari | Keputusan aman |
| --- | --- | --- |
| Geometri mana yang kritis? | Gambar, toleransi, datum, dan titik ukur yang disetujui | Tandai titik ukur awal; jangan hanya mengandalkan kesan visual. |
| Apa yang menahan komponen? | Rencana fixture/clamp dan akses kerja | Tinjau risiko kekangan serta cara pelepasannya bersama prosedur fabrikasi. |
| Bagaimana penyusutan akan dibagi? | Sequence, tack, dan trial yang disetujui | Jangan menyalin urutan dari frame lain yang detailnya berbeda. |
| Kapan hasil dinilai? | Titik pemeriksaan antara dan akhir | Hentikan eskalasi bila ukuran menyimpang dari kriteria yang ditetapkan. |
| Apakah perlu NDT? | Rencana inspeksi dan standar aplikasi | Jangan memilih metode atau menyatakan lulus tanpa dasar yang berlaku. |

Sobat Besi.co.id, bila sequence belum disetujui, tindakan paling hemat biasanya bukan “coba satu sambungan dulu” pada produk akhir. Pisahkan trial yang sah, tentukan apa yang diukur, siapa yang menilai, dan kondisi mana yang harus sama dengan produksi. Hasil trial hanya berguna jika kondisi dan rekamannya cukup untuk dibandingkan; ia bukan bukti otomatis bahwa setiap frame lain akan sama.

## Kesalahan umum dan cara memeriksanya

Kesalahan pertama adalah baru mengukur ketika semua las selesai. Ukur kondisi awal, lalu gunakan titik pemeriksaan antara sesuai rencana agar perubahan dapat diketahui saat masih mungkin dihentikan dan ditinjau. Kesalahan kedua adalah menyamakan clamp dengan solusi: clamp memberi posisi, tetapi tidak menggantikan analisis penyusutan, prosedur, atau persetujuan sequence.

Kesalahan ketiga adalah menyebut hasil “aman” hanya karena tampak rapi. Rekaman inspeksi yang defensibel perlu mengidentifikasi objek atau joint, metode dan teknik, prosedur, personel, peralatan atau kalibrasi, cakupan, temuan, kriteria, hasil, dan disposisi ([ISO 17635](https://www.iso.org/standard/85705.html), [ISO 9712](https://www.iso.org/standard/75614.html)). [NEEDS REVIEW G-08: gunakan rencana NDT dan kriteria penerimaan yang disetujui; halaman ini tidak memilih metode, cakupan, atau acceptance level.]

Kesalahan keempat adalah membetulkan distorsi dengan pemanasan tanpa otorisasi. Controlled correction harus memiliki metode yang ditinjau dan batas yang jelas, karena tindakan koreksi dapat mengubah kondisi komponen dan mutu sambungan. Bila penyimpangan ditemukan, tahan pekerjaan, lindungi identitas komponen dan rekaman ukur, lalu minta keputusan melalui prosedur ketidaksesuaian yang berlaku. Teman Besi.co.id, itu jauh lebih dapat dipertanggungjawabkan daripada menyembunyikan hasil dengan koreksi spontan.

## Mengapa shortcut “las saja dulu, luruskan nanti” gagal

Shortcut ini terasa cepat karena menggeser keputusan sampai setelah bentuk berubah. Namun setelah beberapa sambungan selesai, penyebab perubahan bentuk bisa sudah bercampur: *fit-up* awal, urutan, kekangan, kondisi proses, dan koreksi sebelumnya. Pemeriksaan akhir tidak dapat membangun kembali bukti kendali yang hilang selama pelaksanaan; inilah alasan koordinasi pengelasan dan rekaman proses diperlukan ([ISO 14731](https://www.iso.org/standard/68893.html), [ISO 3834-2](https://www.iso.org/standard/81651.html)).

Alternatif yang lebih andal adalah mengunci keputusan sebelum panas pertama: cek gambar dan toleransi, tetapkan datum serta metode ukur, tinjau fit-up dan fixture, gunakan sequence yang sudah disetujui, dan tentukan titik hold untuk evaluasi. Jika kondisi aktual melampaui asumsi prosedur, jangan membuat resep baru di lantai produksi—eskalasi kepada penanggung jawab teknis.

## Langkah berikutnya sebelum frame dilas

Distorsi dikendalikan dengan mengelola penyusutan dan bukti proses, sedangkan tegangan sisa dihadapi dengan desain, prosedur, dan pengendalian yang tepat—bukan dengan asumsi bahwa bentuk yang terlihat lurus pasti sudah selesai. Sequence yang baik adalah sequence yang cocok untuk detail dan persetujuan pekerjaan tersebut.

Sebelum frame dilas, kumpulkan gambar dan toleransi, dokumen prosedur yang disetujui, rencana fixture/sequence, titik ukur, serta titik hold inspeksi. Pastikan pula rencana K3 menilai ventilasi dan pengendalian paparan; evaluasi NIOSH atas *local exhaust ventilation* menunjukkan bahwa efektivitas kontrol teknik perlu dinilai pada kondisi kerja yang nyata, bukan diasumsikan dari keberadaannya saja ([NIOSH engineering control](https://www.cdc.gov/niosh/engcontrols/ecd/detail44.html)).

Kawan Besi.co.id, aturan operasionalnya sederhana: bila sequence, kriteria ukur, atau metode koreksi belum tertulis dan disetujui, berhenti pada tahap perencanaan dan minta review teknis—jangan menjadikannya eksperimen pada frame produksi.
