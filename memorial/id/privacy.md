# Kebijakan Privasi Virtual Memorial Space

**Tanggal Berlaku: 1 November 2026**

## 1. Pendahuluan

Virtual Memorial Space ("Aplikasi", "kami") adalah aplikasi iOS untuk membuat ruang kenangan pribadi, melakukan ritual mengenang, dan menulis surat. Kebijakan Privasi ini menjelaskan informasi apa yang ditangani Aplikasi, di mana informasi itu disimpan, dan pilihan apa yang Anda miliki.

Aplikasi tidak memerlukan akun. Konten kenangan Anda tetap berada di perangkat Anda. Server kami hanya digunakan untuk Token Kenangan, token opsional di dalam Aplikasi yang dipakai untuk gaya persembahan yang lebih istimewa.

Dengan menggunakan Aplikasi, Anda menyatakan telah membaca dan memahami Kebijakan Privasi ini.

## 2. Informasi yang Tidak Kami Kumpulkan

Aplikasi tidak mengumpulkan atau meminta:

- Nama, alamat email, nomor telepon, atau akun login apa pun milik Anda
- Nama, foto, tanggal, deskripsi, surat, atau pesan dalam ruang kenangan Anda
- Akses ke seluruh pustaka foto, kamera, mikrofon, kontak, atau lokasi
- Detail kartu pembayaran Anda
- Pengenal iklan (IDFA). Aplikasi tidak melacak Anda di aplikasi atau situs web milik perusahaan lain dan tidak menampilkan permintaan Transparansi Pelacakan Aplikasi (ATT).
- Data analitik atau peristiwa penggunaan. Aplikasi tidak berisi SDK analitik dan tidak menampilkan iklan.

## 3. Konten Kenangan yang Hanya Disimpan di Perangkat Anda

Hal-hal berikut disimpan di penyimpanan pribadi Aplikasi pada iPhone atau iPad Anda:

- Ruang kenangan: nama, jenis (misalnya orang tercinta, pasangan, teman, atau hewan peliharaan), deskripsi, tanggal lahir, tanggal peringatan, tema, dan pengaturan pengingat
- Foto yang Anda tambahkan ke ruang kenangan
- Catatan ritual: lilin, bunga, atau persembahan kertas yang digunakan, jumlah token yang dipakai, waktu, dan pesan yang Anda tambahkan
- Surat yang Anda tulis, termasuk draf
- Preferensi: bahasa, efek yang dikurangi, apakah persembahan kertas tradisional ditampilkan, apakah pengenalan sudah selesai, penanda sinkronisasi pembelian yang tertunda, dan penghitung yang membatasi permintaan rating
- Saldo token terakhir yang diterima dari server kami, hanya digunakan untuk tampilan saat offline

Konten ini tidak diunggah ke server kami, tidak digunakan untuk iklan, dan tidak digunakan untuk fitur atau pelatihan kecerdasan buatan (AI) apa pun. Jika Cadangan iCloud aktif, iOS dapat menyertakan data ini dalam cadangan perangkat yang ditangani Apple di bawah Apple ID Anda. Aplikasi tidak memiliki sinkronisasi cloud sendiri.

**Foto.** Anda memilih foto melalui pemilih foto sistem. Aplikasi hanya menerima foto yang Anda pilih dan tidak mengakses seluruh pustaka foto Anda. Salinan terkompresi dari setiap foto yang dipilih disimpan di penyimpanan Aplikasi.

## 4. Token Kenangan dan Server Kami

Token Kenangan adalah pembelian dalam aplikasi yang bersifat habis pakai. Agar saldo tetap ada setelah Aplikasi diinstal ulang, saldo disimpan di server kami ("appapi") yang berjalan di Vercel dan menyimpan data di Vercel KV (Upstash Redis).

Server hanya menyimpan:

- ID pengguna yang dibuat secara acak, tidak terhubung dengan nama, alamat email, atau Apple ID Anda
- Ringkasan (hash) dari token akses yang diterbitkan untuk ID pengguna tersebut. Token itu sendiri tidak disimpan di server.
- Saldo token Anda
- Catatan pembelian: ID produk, ID transaksi Apple, jumlah token, dan waktu
- Catatan pemakaian: ID persembahan (misalnya jenis lilin), jumlah token, kunci permintaan untuk mencegah pemotongan ganda, saldo setelahnya, dan waktu
- Riwayat penambahan, pemakaian, dan pengembalian dana beserta jumlah dan ID transaksi atau ID pemakaian terkait

Setiap permintaan ke server juga menyertakan versi Aplikasi dan pengenal perangkat (identifierForVendor iOS), yang digunakan untuk memverifikasi tanda tangan permintaan. Seperti layanan web pada umumnya, penyedia hosting kami dapat memproses alamat IP Anda dalam log permintaan rutin untuk menyediakan dan melindungi layanan.

Server tidak menyimpan nama, alamat email Anda, atau apa pun tentang orang atau hewan peliharaan yang Anda kenang: tidak ada nama, foto, surat, atau pesan kenangan.

ID pengguna dan token disimpan di Rantai Kunci iOS pada perangkat Anda. Keduanya dapat disinkronkan melalui Rantai Kunci iCloud sehingga saldo tetap tersedia setelah Aplikasi diinstal ulang atau di perangkat lain yang masuk dengan Apple ID yang sama.

## 5. Pembelian

- **Apple (App Store)** memproses semua pembayaran melalui Apple ID Anda. Kami tidak pernah menerima detail kartu pembayaran Anda. Kebijakan privasi Apple: https://www.apple.com/legal/privacy/
- **RevenueCat** memvalidasi transaksi. RevenueCat menerima ID pengguna acak di atas, informasi transaksi (seperti ID produk, ID transaksi Apple, dan waktu pembelian), serta informasi teknis dasar seperti versi Aplikasi, versi sistem operasi, dan negara App Store. Server kami meminta RevenueCat untuk mengonfirmasi pembelian, dan RevenueCat memberi tahu server kami tentang pembelian dan pengembalian dana, sehingga token hanya ditambahkan satu kali dan ditarik kembali setelah pengembalian dana. Kebijakan privasi RevenueCat: https://www.revenuecat.com/privacy

Token Kenangan tidak memiliki nilai uang di dunia nyata. Pengembalian dana ditangani oleh Apple sesuai aturannya. Ketentuan penggunaan adalah perjanjian lisensi standar Apple: https://www.apple.com/legal/internet-services/itunes/dev/stdeula/

## 6. Notifikasi (Opsional)

Jika Anda mengaktifkan pengingat tanggal peringatan untuk sebuah ruang kenangan, Aplikasi meminta izin notifikasi dan menjadwalkan notifikasi lokal di perangkat Anda. Pengingat tidak melewati server kami. Anda dapat menonaktifkannya di Aplikasi atau di Pengaturan iOS.

## 7. Cara Kami Menggunakan Informasi

Kami menggunakan informasi di atas hanya untuk:

- Menampilkan dan menyimpan ruang kenangan, ritual, dan surat Anda di perangkat Anda
- Membuat dompet token Anda, menambahkan token yang dibeli satu kali per transaksi, memotong token saat Anda memilih persembahan premium, dan menarik kembali token setelah pengembalian dana
- Memverifikasi permintaan serta mencegah penipuan atau penambahan ganda
- Menanggapi permintaan dukungan Anda

Kami tidak menjual atau menyewakan informasi pribadi, tidak menggunakannya untuk iklan, dan tidak membuat profil iklan.

## 8. Berbagi Informasi

Kami hanya berbagi informasi dengan penyedia layanan yang diperlukan untuk menjalankan Aplikasi (Apple, RevenueCat, serta Vercel / Upstash untuk hosting dan penyimpanan), atau jika diwajibkan oleh hukum atau proses hukum yang sah.

## 9. Menghapus Data Anda

Di Pengaturan Aplikasi:

- **Hapus Semua Data (Delete All Data)** menghapus semua konten kenangan di perangkat ini: ruang kenangan, foto, catatan ritual, surat, dan pesan.
- **Hapus Data Token (Delete Token Data)** menghapus dompet Anda di server kami: catatan ID pengguna, hash token, saldo, catatan pembelian dan pemakaian, serta riwayat. Saldo Anda menjadi nol dan tidak dapat dipulihkan. Untuk mencegah pembelian yang sama ditambahkan lagi, kami hanya menyimpan ID transaksi Apple (beserta ID produknya) tanpa ID pengguna. Setelah itu, ID pengguna dan token juga dihapus dari Rantai Kunci Anda.

Menghapus Aplikasi akan menghapus konten lokalnya dari perangkat, tetapi **tidak** menghapus dompet Anda di server kami. Untuk menghapusnya, gunakan "Hapus Data Token" sebelum menghapus Aplikasi, atau hubungi kami. Data lokal yang telah dihapus mungkin masih ada di cadangan iCloud perangkat sebelumnya hingga Apple menggantikan atau menghapusnya.

Anda juga dapat meminta kami untuk mengajukan penghapusan catatan pembelian yang disimpan oleh RevenueCat.

## 10. Keamanan dan Penyimpanan

Koneksi ke server kami, Apple, dan RevenueCat menggunakan HTTPS terenkripsi. Permintaan ditandatangani, server hanya menyimpan hash token Anda, dan identitas Anda disimpan di Rantai Kunci iOS. Tidak ada metode penyimpanan atau transmisi yang sepenuhnya aman.

- Konten lokal disimpan sampai Anda menghapusnya atau menghapus Aplikasi.
- Data dompet di server disimpan sampai Anda menggunakan "Hapus Data Token" atau meminta kami menghapusnya.
- ID transaksi Apple tanpa ID pengguna disimpan untuk mencegah penambahan ganda.
- Apple dan RevenueCat menyimpan catatan pembelian sesuai kebijakan dan kewajiban hukum mereka sendiri.

## 11. Privasi Anak

Virtual Memorial Space tidak ditujukan untuk anak-anak. Kami tidak dengan sengaja mengumpulkan informasi pribadi dari anak di bawah 13 tahun (atau di bawah usia minimum yang berlaku di negara Anda). Jika Anda yakin seorang anak telah memberikan informasi pribadi kepada kami, hubungi kami dan kami akan menghapusnya.

## 12. Pemrosesan Internasional

Penyedia hosting dan penyimpanan kami serta RevenueCat dapat memproses data di Amerika Serikat atau negara lain selain negara Anda. Kami mengandalkan perlindungan dari penyedia tersebut untuk pemrosesan ini.

## 13. Hak Anda

Tergantung tempat tinggal Anda, Anda mungkin berhak mengakses, mengoreksi, menghapus, atau membatasi pemrosesan informasi pribadi Anda. Sebagian besar data ada di perangkat Anda dan berada dalam kendali Anda. Untuk data di server kami, gunakan "Hapus Data Token" atau hubungi kami. Kami mungkin meminta informasi yang membantu kami menemukan catatan terkait.

## 14. Perubahan Kebijakan Ini

Kami dapat memperbarui Kebijakan Privasi ini. Tanggal di bagian atas akan berubah saat kami melakukannya. Jika Aplikasi mulai mengumpulkan jenis data baru, kami akan memperbarui kebijakan ini terlebih dahulu.

## 15. Hubungi Kami

Jika Anda memiliki pertanyaan tentang Kebijakan Privasi ini, hubungi:

- Email: lpjustdoit@163.com

---

## Bahasa lain

- [English](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/en/privacy.md)
- [简体中文](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/zh/privacy.md)
- [繁體中文](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/zh-tw/privacy.md)
- [日本語](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ja/privacy.md)
- [한국어](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ko/privacy.md)
- [Deutsch](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/de/privacy.md)
- [Français](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/fr/privacy.md)
- [Español](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/es/privacy.md)
- [Italiano](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/it/privacy.md)
- [Português (Portugal)](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/pt-PT/privacy.md)
- [Português (Brasil)](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/pt-BR/privacy.md)
- [ไทย](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/th/privacy.md)
- [Tiếng Việt](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/vi/privacy.md)
- [Bahasa Indonesia](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/id/privacy.md)
- [Bahasa Melayu](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ms/privacy.md)
- [العربية](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ar/privacy.md)
