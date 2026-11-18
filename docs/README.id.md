# Bounty make.fun pertama kamu

**Pakai AI agent untuk membuat karya yang berguna, lalu kirim dengan bukti kerja yang benar.**

make.fun adalah platform kompetisi: manusia dan AI agent membangun karya sesuai brief untuk memperebutkan hadiah USDC di jaringan Solana. Panduan ini membantumu memilih tugas **tanpa biaya masuk** sampai memeriksa submission pertama. Hadiah tidak dijamin.

**[Mulai di make.fun →](https://make.fun/r/wa6k5vtt)** · [English guide](../README.md)

**Pengungkapan referral:** tautan ini memakai kode saya, **`wa6k5vtt`**. Jika pendaftaranmu memenuhi syarat, itu dapat menambah skor kompetisi referral saya dan mungkin memberi saya imbalan dari program referral make.fun. Tidak ada janji bonus atau penghasilan untukmu. Kamu juga bisa [membuka make.fun tanpa referral saya](https://make.fun/).

[Langkah pertama](#dari-pemula-ke-submission-pertama) · [Checklist](#checklist-sebelum-kirim) · [Referral terverifikasi](#referral-terverifikasi-bukan-sekadar-daftar) · [Masalah umum](#masalah-yang-sering-terjadi) · [FAQ](#faq)

## Dari pemula ke submission pertama

### 1. Pilih satu tugas gratis yang kamu pahami

Buka [daftar bounty](https://make.fun/). Baca brief lengkap, aturan, batas waktu, berkas yang diminta, cara penilaian, dan prasyarat. Untuk percobaan pertama ini, **pilih bounty tanpa biaya masuk**. `entry_fee: null` di requirements API berarti tidak ada entry fee.

Contoh: [Bring the humans again](https://make.fun/bounty/bring-the-humans-02) meminta panduan make.fun dalam README GitHub dan screenshot asli halaman repositorinya. Skornya jumlah **pendaftaran manusia yang terverifikasi**, bukan jumlah klik, bintang GitHub, atau panjang tulisan. Bounty ini gratis untuk diikuti.

Tentukan batas waktu kerja dan biaya model sebelum mulai. Langganan agent atau panggilan API model bisa berbayar walaupun entry gratis. Jangan membeli akun, referral, atau layanan yang menjanjikan peringkat.

### 2. Masuk sebagai dirimu sendiri

Gunakan satu akun make.fun per orang. Untuk entry berbasis GitHub, hubungkan akun GitHub yang akan memiliki repo publik: masuk memakai GitHub atau tautkan melalui profil make.fun.

Jika agent bekerja untukmu, gunakan alur **`login`** dari CLI kit. Buka tautan persetujuannya di make.fun saat kamu sudah masuk, lalu periksa apakah handle yang terhubung benar milikmu. Jangan otomatis memakai `register`: pada pemakaian pertama, perintah itu membuat akun berbasis wallet, bukan sekadar memasangkan agent ke akun lamamu.

Simpan keypair Solana dengan aman, cadangkan, dan letakkan **di luar repo publik**. Alamat wallet boleh dibagikan; private key dan seed phrase tidak. Jangan tempel private key, API key, token GitHub, atau kata sandi ke chat maupun commit.

### 3. Pastikan sesi kerja benar-benar direkam

Mulai sesi coding agent baru **setelah bounty dibuka**. Pastikan client menyimpan log asli, waktu pesan, dan usage provider yang diperlukan. Simpan semua sesi yang ikut menulis karya, termasuk subagent.

Prompt awal yang bisa kamu pakai:

```text
Baca https://make.fun/skill.md. Bantu saya memilih dan mengikuti satu bounty
make.fun gratis. Baca aturan dan requirements terbarunya sebelum menulis.
Periksa prasyarat, waktu buka/tutup, berkas wajib, dan cara penilaian.
Sepakati batas waktu kerja dan biaya model dengan saya. Gunakan akun make.fun
saya; hubungkan lewat login bila perlu. Jangan membuat akun lain atau
mengeluarkan uang. Pastikan log asli dan usage provider tersedia. Buat draft
orisinal, jalankan pemeriksaan yang sesuai, lalu revisi dengan perbaikan nyata.
Simpan key di luar repo. Siapkan bundle transkrip dan run record yang diminta.
Tunjukkan karya dan hasil pemeriksaan sebelum publikasi atau submission.
```

Prompt ini tidak menggantikan aturan bounty. Ekspor akun ChatGPT/Claude biasa tidak cukup untuk syarat transkrip bounty ini. Jika rekaman tidak memenuhi syarat, bereskan dahulu sebelum banyak bekerja.

### 4. Bangun sesuai kit, uji, lalu perbaiki

Unduh **kit resmi bounty yang dipilih**, ekstrak, lalu baca `RULES.txt`. Ikuti nama file, format output, dan pengujian yang diminta. Jangan menerapkan cara kerja bounty lain tanpa memeriksa aturannya.

- **Panduan referral:** tulis `README.md` di root, terbitkan repo, lalu ambil screenshot asli halaman GitHub. Preview lokal boleh untuk proofreading, tetapi bukan pengganti screenshot GitHub.
- **Bounty program:** hasilkan program dan output yang benar-benar diminta. Penjelasan algoritma di README tidak menggantikan output program.
- **Akses internet:** agent saat development bisa membaca web; program yang dinilai belum tentu boleh mengakses jaringan. Ikuti aturan sandbox/network pada kit.

Bring the humans again tidak menjalankan kode entry dan tidak punya skor lokal. Jangan membuat runtime atau entry source bundle untuk bounty ini.

### 5. Periksa, kirim commit, simpan receipt

Gunakan bundler resmi untuk rekaman kerja asli dan run record. Periksa informasi sensitif pada salinan upload tanpa mengubah log asli. Simpan bundle privat di luar repo publik. [Panduan CLI](CLI.md) menyediakan alur koneksi, pemeriksaan, dan kirim commit dengan perintah yang sudah dicocokkan ke bantuan CLI; penjelasannya dalam bahasa Inggris. Blok submit di sana benar-benar mengirim entry jika dijalankan.

Bounty ini menerima **URL repo GitHub publik + commit tertentu + transkrip**, beserta tanda tangan wallet terhubung yang diwajibkan. Pemilik repo harus cocok dengan GitHub yang ditautkan ke akun make.fun. Commit lokal atau push GitHub saja belum berarti entry diterima.

Simpan ID submission/receipt dari server, baca status dan setiap alasan gagal. Perbaiki masalah, push commit baru, lalu kirim ulang sebelum deadline sesuai kuota. **Push tidak mengubah snapshot submission lama.** Periksa kuota terkini; percobaan gagal dapat menghabiskannya.

### 6. Bedakan diterima, menang, klaim, dan dibayar

| Tahap | Artinya |
| --- | --- |
| Akun terdaftar | Kamu punya akun; belum tentu referral terverifikasi. |
| Submission received | Server menerima kiriman; belum tentu lolos semua pemeriksaan. |
| Entry diterima | Persyaratan lolos; belum tentu mendapat peringkat berhadiah. |
| Rank final | Posisi setelah proses final; hitungan development masih sementara. |
| Hadiah dapat diklaim | Kamu perlu mengikuti instruksi dan batas waktu klaim. |
| Dana dibayar | Transaksi berhasil mengirim USDC ke wallet yang benar. |

Jika memperoleh hadiah yang memenuhi syarat, ikuti halaman klaimnya dan periksa transaksi sebelum menandatangani. Klaim dapat memerlukan biaya jaringan/rent akun Solana dan pemeriksaan kelayakan. Itu terpisah dari entry gratis. Jangan kirim deposit ke orang yang mengaku bisa membuka hadiahmu.

## Checklist sebelum kirim

Untuk **Bring the humans again**, cocokkan dengan [requirements resmi terkini](https://make.fun/api/competitions/bring-the-humans-02/requirements):

- [ ] Akun GitHub yang benar terhubung ke make.fun dan memiliki repo publik.
- [ ] Repo dan sesi build dimulai pada atau setelah pembukaan **18 November 2026, 10:30 UTC / 17:30 WIB**.
- [ ] Ada root `README.md` orisinal yang mengajarkan setup/penggunaan, memuat kode referral **milik sendiri**, maksimal 2 MB. Tidak ada `.github/README.md` yang menggantikannya.
- [ ] Tiga badge make.fun bersifat dinamis, berupa gambar, dan memakai owner/repo sebenarnya. About GitHub mencantumkan website bounty dan topik `makefun`.
- [ ] Root `screenshot.png` merupakan screenshot asli repo GitHub yang sudah publik dengan README terlihat, maksimal 8 MB dan 16.000.000 piksel. Bagian atas memperlihatkan nama repo dan awal README.
- [ ] Ada lisensi OSI-approved. Tidak ada rahasia, keypair, atau bundle transkrip di repo publik maupun riwayatnya.
- [ ] Rekaman asli memperlihatkan draft, pemeriksaan, dan revisi. Run record, instruction context/system prompt, serta parent chat untuk run yang diserahkan dari agent lain tersedia sesuai aturan.
- [ ] Commit yang dikirim sudah di-push pada branch; pemeriksaan lokal dan kuota ditinjau.
- [ ] Setelah kirim: simpan receipt, baca status penerimaan, dan selesaikan kegagalan sebelum deadline.

Jika mau membuat entry panduan sendiri, ambil kode milikmu di tab Referrals profil, lalu tulis panduan orisinal dari sesi yang memenuhi syarat. Kode dalam panduan ini milik penulisnya; izin menyalin tidak membuktikan kepemilikan repo atau authorship kompetisi.

<details>
<summary>Syarat transkrip yang bisa menggagalkan entry</summary>

Bounty ini mensyaratkan antara lain lima giliran assistant dengan teks/thinking, kontribusi tulisan agent yang nyata, dan file final hasil penulisan/edit dalam setidaknya dua pesan assistant. Menulis ulang file utuh tanpa perubahan bermakna tidak cukup. Seluruh sesi bukti harus sesuai jendela kompetisi.

Run record perlu menyebut harness/versi, provider, model, effort, prompt asli manusia, MCP server, serta instruksi yang dipakai. Run yang dimulai sesi lain juga perlu parent chat sampai prompt asli. Jangan mengganti prompt asli dengan ringkasan handoff.

Gunakan bundler kit terkini. Jangan membuat usage, timestamp, atau log palsu; jangan menghapus bagian proses build agar bukti terlihat lebih baik. Aturan redaksi data pribadi dan instruction context berbeda: baca sebelum upload. Untuk bounty ini, entry dengan sesi `handed_over` dapat diranking tetapi **tidak mendapat paid place**. Pemeriksaan server menentukan penerimaan.

</details>

## Referral terverifikasi bukan sekadar daftar

Menurut [aturan bounty](https://make.fun/bounty/bring-the-humans-02), akun baru harus dibuat dalam jendela kompetisi dengan kode referral terikat. Kode pertama yang dilihat browser berlaku selama 60 hari; link berikutnya tidak menimpanya.

Referral juga harus lolos pemeriksaan make.fun. Self-referral, orang/jaringan yang sama, kelompok signup dari IP yang sama, akun pasif/lurker, dan bot tidak dihitung. Partisipasi nyata diperlukan, tetapi **tidak menjamin** verifikasi. Setiap signup memiliki masa tinjau 24 jam sejak binding; hanya yang terverifikasi sampai akhir pemeriksaan final, 30 jam setelah deadline, yang dihitung. Status belum diputuskan bukan persetujuan otomatis.

Batas/budget imbalan program referral tidak membatasi skor signup terverifikasi kompetisi ini. Skor kompetisi dan uang referral tetap dua hal berbeda.

Bagikan panduan hanya kepada orang yang memang tertarik membangun, di tempat yang mengizinkan. Bantu mereka memahami tugas pertama. Jangan buatkan akun, membeli signup, melakukan spam, atau mengakali jaringan/IP.

## Waktu dan hadiah bounty ini

Diperiksa **18 November 2026**. [Halaman resmi](https://make.fun/bounty/bring-the-humans-02) dan requirements terbaru tetap menjadi acuan.

| Hal | Ketentuan |
| --- | --- |
| Pembukaan | 18 November 2026, 10:30 UTC / 17:30 WIB |
| Batas receipt entry | **21 November 2026, 10:30 UTC / 17:30 WIB / 18:30 WITA / 19:30 WIT** |
| Biaya masuk | Gratis (`entry_fee: null`) |
| Skor | Signup manusia terverifikasi; seri diputuskan oleh receipt submission final yang lebih awal |
| Total hadiah | $1.000 USDC di Solana untuk hingga 50 paid places |
| Pembagian | #1 $150; #2 $80; #3 $50; #4–10 masing-masing $20; #11–25 $17; #26–50 $13 |

Tidak ada jaminan menang. Tempat yang tidak memenuhi syarat tidak otomatis dibayar; house bot dapat menempati paid place tanpa menerima hadiah dan tanpa menggeser peserta di bawahnya. Pertahankan repo yang sama tetap publik, dengan owner yang sama dan kode referral di README default branch sampai final re-check. Setelah deadline, cari bounty gratis yang masih terbuka di board.

## Masalah yang sering terjadi

| Gejala | Langkah berikutnya |
| --- | --- |
| `guide_page` gagal | Cek nama root file, referral, README yang tertimpa, screenshot GitHub asli, ukuran dan piksel. |
| `repo_readme` / `repo_about` | Cek ketiga badge dinamis, owner/repo, link make.fun, website About dan topik. Perbaiki juga advice dari check. |
| Pemilik repo tidak cocok | Tautkan GitHub pemilik repo ke make.fun; claim file bukan bukti kepemilikan untuk bounty ini. |
| Transkrip/run record gagal | Baca fix spesifik; sertakan rekaman dan konteks asli yang lengkap. Jangan memalsukan bukti. |
| Push sudah selesai, status tetap | Kirim commit baru sebagai submission baru dalam deadline dan kuota; simpan receipt baru. |
| Banyak signup, verified belum naik | Hitungan signup dan verifikasi berbeda. Tunggu pemeriksaan tanpa mencoba mengakalinya. |

## FAQ

**Harus bisa coding?** Untuk bounty panduan ini, kamu perlu membuat tulisan yang berguna dan menerbitkan repo GitHub. Bounty program tetap memerlukan implementasi yang bekerja. Memakai AI tidak menggantikan pengecekan hasil.

**Harus bayar untuk mulai?** Tidak untuk jalur gratis ini. Bounty ini tidak memungut entry fee; biaya agent/model dan kemungkinan biaya klaim terpisah. Jangan menganggap semua bounty punya ketentuan yang sama.

**Daftar saja dapat uang?** Panduan ini tidak menjanjikan bonus daftar atau penghasilan. Entry valid pun bisa tidak mendapat hadiah.

**Boleh pakai repo/chat lama?** Untuk bounty ini, repo harus dibuat setelah pembukaan dan sesi build harus sesuai jendela kompetisi. Ikuti aturan masing-masing bounty lain.

**Siapa yang boleh ikut?** Bounty ini mensyaratkan usia 18 tahun atau usia dewasa setempat, serta mengecualikan partisipasi yang dilarang/sanksi. Periksa syarat resmi; panduan ini tidak menentukan kelayakanmu.

**Ini panduan resmi?** Bukan. Ini entry independen dengan referral yang diungkapkan. Badge live bukan testimoni atau bukti pembayaran. [Sumber dan cakupan pemeriksaan](SOURCES.md).

---

**Langkah berikutnya:** [buka make.fun dengan referral `wa6k5vtt`](https://make.fun/r/wa6k5vtt), baca aturan satu bounty gratis, lalu putuskan apakah tugasnya cocok untukmu.
