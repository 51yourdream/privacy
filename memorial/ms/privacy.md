# Dasar Privasi Virtual Memorial Space

**Tarikh Berkuat Kuasa: 1 November 2026**

## 1. Pengenalan

Virtual Memorial Space ("Aplikasi", "kami") ialah aplikasi iOS untuk mencipta ruang kenangan peribadi, melakukan ritual mengenang dan menulis surat. Dasar Privasi ini menerangkan maklumat yang dikendalikan oleh Aplikasi, di mana maklumat itu disimpan dan pilihan yang anda ada.

Aplikasi tidak memerlukan akaun. Kandungan kenangan anda kekal pada peranti anda. Pelayan kami hanya digunakan untuk Token Kenangan, iaitu token pilihan dalam Aplikasi yang digunakan untuk gaya persembahan yang lebih istimewa.

Dengan menggunakan Aplikasi, anda mengakui bahawa anda telah membaca dan memahami Dasar Privasi ini.

## 2. Maklumat yang Tidak Kami Kumpul

Aplikasi tidak mengumpul atau meminta:

- Nama, alamat e-mel, nombor telefon atau sebarang akaun log masuk anda
- Nama, foto, tarikh, penerangan, surat atau mesej dalam ruang kenangan anda
- Akses kepada keseluruhan pustaka foto, kamera, mikrofon, kenalan atau lokasi
- Butiran kad pembayaran anda
- Pengecam pengiklanan (IDFA). Aplikasi tidak menjejak anda merentas aplikasi atau laman web syarikat lain dan tidak memaparkan permintaan Ketelusan Penjejakan Aplikasi (ATT).
- Data analitik atau peristiwa penggunaan. Aplikasi tidak mengandungi SDK analitik dan tiada iklan.

## 3. Kandungan Kenangan yang Disimpan pada Peranti Anda Sahaja

Perkara berikut disimpan dalam storan peribadi Aplikasi pada iPhone atau iPad anda:

- Ruang kenangan: nama, jenis (contohnya orang tersayang, pasangan, rakan atau haiwan peliharaan), penerangan, tarikh lahir, tarikh peringatan, tema dan tetapan peringatan
- Foto yang anda tambahkan pada ruang kenangan
- Rekod ritual: lilin, bunga atau persembahan kertas yang digunakan, bilangan token yang dibelanjakan, masa dan mesej yang anda tambahkan
- Surat yang anda tulis, termasuk draf
- Keutamaan: bahasa, kesan dikurangkan, sama ada persembahan kertas tradisional dipaparkan, sama ada pengenalan telah selesai, penanda penyegerakan pembelian yang belum selesai dan pembilang yang mengehadkan permintaan penilaian
- Baki token terakhir yang diterima daripada pelayan kami, digunakan hanya untuk paparan luar talian

Kandungan ini tidak dimuat naik ke pelayan kami, tidak digunakan untuk pengiklanan dan tidak digunakan untuk sebarang ciri atau latihan kecerdasan buatan (AI). Jika Sandaran iCloud dihidupkan, iOS mungkin memasukkan data ini dalam sandaran peranti yang dikendalikan oleh Apple di bawah Apple ID anda. Aplikasi tidak mempunyai penyegerakan awan sendiri.

**Foto.** Anda memilih foto melalui pemilih foto sistem. Aplikasi hanya menerima foto yang anda pilih dan tidak mengakses keseluruhan pustaka foto anda. Salinan termampat bagi setiap foto yang dipilih disimpan dalam storan Aplikasi.

## 4. Token Kenangan dan Pelayan Kami

Token Kenangan ialah pembelian dalam aplikasi jenis boleh guna habis. Supaya baki anda kekal selepas Aplikasi dipasang semula, baki disimpan pada pelayan kami ("appapi") yang berjalan di Vercel dan menyimpan data dalam Vercel KV (Upstash Redis).

Pelayan hanya menyimpan:

- ID pengguna yang dijana secara rawak, tidak dikaitkan dengan nama, alamat e-mel atau Apple ID anda
- Ringkasan (hash) token akses yang dikeluarkan untuk ID pengguna tersebut. Token itu sendiri tidak disimpan pada pelayan.
- Baki token anda
- Rekod pembelian: ID produk, ID transaksi Apple, bilangan token dan masa
- Rekod perbelanjaan: ID persembahan (contohnya jenis lilin), bilangan token, kunci permintaan untuk mengelakkan potongan berganda, baki selepasnya dan masa
- Lejar kredit, perbelanjaan dan bayaran balik beserta jumlah serta ID transaksi atau ID perbelanjaan yang berkaitan

Setiap permintaan ke pelayan juga membawa versi Aplikasi dan pengecam peranti (identifierForVendor iOS), yang digunakan untuk mengesahkan tandatangan permintaan. Seperti mana-mana perkhidmatan web, penyedia pengehosan kami mungkin memproses alamat IP anda dalam log permintaan biasa untuk menyediakan dan melindungi perkhidmatan.

Pelayan tidak menyimpan nama, alamat e-mel anda atau apa-apa tentang orang atau haiwan peliharaan yang anda kenang: tiada nama, foto, surat atau mesej kenangan.

ID pengguna dan token disimpan dalam Rantai Kunci iOS pada peranti anda. Ia mungkin disegerakkan melalui Rantai Kunci iCloud supaya baki anda tersedia selepas Aplikasi dipasang semula atau pada peranti lain yang log masuk dengan Apple ID yang sama.

## 5. Pembelian

- **Apple (App Store)** memproses semua pembayaran melalui Apple ID anda. Kami tidak pernah menerima butiran kad pembayaran anda. Dasar privasi Apple: https://www.apple.com/legal/privacy/
- **RevenueCat** mengesahkan transaksi. RevenueCat menerima ID pengguna rawak di atas, maklumat transaksi (seperti ID produk, ID transaksi Apple dan masa pembelian) serta maklumat teknikal asas seperti versi Aplikasi, versi sistem pengendalian dan negara App Store. Pelayan kami meminta RevenueCat mengesahkan pembelian, dan RevenueCat memaklumkan pelayan kami tentang pembelian dan bayaran balik, supaya token dikreditkan sekali sahaja dan ditarik balik selepas bayaran balik. Dasar privasi RevenueCat: https://www.revenuecat.com/privacy

Token Kenangan tidak mempunyai nilai kewangan sebenar. Bayaran balik dikendalikan oleh Apple mengikut peraturannya. Terma penggunaan ialah perjanjian lesen standard Apple: https://www.apple.com/legal/internet-services/itunes/dev/stdeula/

## 6. Pemberitahuan (Pilihan)

Jika anda menghidupkan peringatan tarikh peringatan bagi sesuatu ruang kenangan, Aplikasi akan meminta kebenaran pemberitahuan dan menjadualkan pemberitahuan setempat pada peranti anda. Peringatan tidak melalui pelayan kami. Anda boleh mematikannya dalam Aplikasi atau dalam Tetapan iOS.

## 7. Cara Kami Menggunakan Maklumat

Kami menggunakan maklumat di atas hanya untuk:

- Memaparkan dan menyimpan ruang kenangan, ritual dan surat anda pada peranti anda
- Mencipta dompet token anda, mengkreditkan token yang dibeli sekali bagi setiap transaksi, menolak token apabila anda memilih persembahan premium dan menarik balik token selepas bayaran balik
- Mengesahkan permintaan serta mencegah penipuan atau kredit berganda
- Membalas permintaan sokongan anda

Kami tidak menjual atau menyewakan maklumat peribadi, tidak menggunakannya untuk pengiklanan dan tidak membina profil pengiklanan.

## 8. Perkongsian Maklumat

Kami hanya berkongsi maklumat dengan penyedia perkhidmatan yang diperlukan untuk menjalankan Aplikasi (Apple, RevenueCat serta Vercel / Upstash untuk pengehosan dan storan), atau apabila dikehendaki oleh undang-undang atau proses undang-undang yang sah.

## 9. Memadam Data Anda

Dalam Tetapan Aplikasi:

- **Padam Semua Data (Delete All Data)** memadam semua kandungan kenangan pada peranti ini: ruang kenangan, foto, rekod ritual, surat dan mesej.
- **Padam Data Token (Delete Token Data)** memadam dompet anda pada pelayan kami: rekod ID pengguna, hash token, baki, rekod pembelian dan perbelanjaan serta lejar. Baki anda menjadi sifar dan tidak boleh dipulihkan. Untuk mengelakkan pembelian yang sama dikreditkan semula, kami hanya menyimpan ID transaksi Apple (bersama ID produknya) tanpa ID pengguna. Selepas itu, ID pengguna dan token turut dibuang daripada Rantai Kunci anda.

Memadam Aplikasi akan membuang kandungan setempatnya daripada peranti, tetapi **tidak** memadam dompet anda pada pelayan kami. Untuk memadamnya, gunakan "Padam Data Token" sebelum memadam Aplikasi, atau hubungi kami. Data setempat yang telah dipadam mungkin masih ada dalam sandaran iCloud peranti yang terdahulu sehingga Apple menggantikan atau memadamnya.

Anda juga boleh meminta kami memohon kepada RevenueCat untuk memadam rekod pembelian yang disimpannya.

## 10. Keselamatan dan Penyimpanan

Sambungan ke pelayan kami, Apple dan RevenueCat menggunakan HTTPS yang disulitkan. Permintaan ditandatangani, pelayan hanya menyimpan hash token anda dan identiti anda disimpan dalam Rantai Kunci iOS. Tiada kaedah storan atau penghantaran yang selamat sepenuhnya.

- Kandungan setempat kekal sehingga anda memadamnya atau memadam Aplikasi.
- Data dompet pada pelayan kekal sehingga anda menggunakan "Padam Data Token" atau meminta kami memadamnya.
- ID transaksi Apple tanpa ID pengguna disimpan untuk mengelakkan kredit berganda.
- Apple dan RevenueCat menyimpan rekod pembelian mengikut dasar dan kewajipan undang-undang mereka sendiri.

## 11. Privasi Kanak-kanak

Virtual Memorial Space tidak ditujukan kepada kanak-kanak. Kami tidak dengan sengaja mengumpul maklumat peribadi daripada kanak-kanak di bawah umur 13 tahun (atau di bawah umur minimum yang ditetapkan di negara anda). Jika anda percaya seorang kanak-kanak telah memberikan maklumat peribadi kepada kami, hubungi kami dan kami akan memadamnya.

## 12. Pemprosesan Antarabangsa

Penyedia pengehosan dan storan kami serta RevenueCat mungkin memproses data di Amerika Syarikat atau negara lain selain negara anda. Kami bergantung pada perlindungan penyedia ini untuk pemprosesan tersebut.

## 13. Hak Anda

Bergantung pada tempat tinggal anda, anda mungkin berhak untuk mengakses, membetulkan, memadam atau mengehadkan pemprosesan maklumat peribadi anda. Kebanyakan data berada pada peranti anda dan di bawah kawalan anda. Untuk data pada pelayan kami, gunakan "Padam Data Token" atau hubungi kami. Kami mungkin meminta maklumat yang membantu kami mencari rekod berkaitan.

## 14. Perubahan pada Dasar Ini

Kami mungkin mengemas kini Dasar Privasi ini. Tarikh di bahagian atas akan berubah apabila kami berbuat demikian. Jika Aplikasi mula mengumpul jenis data baharu, kami akan mengemas kini dasar ini terlebih dahulu.

## 15. Hubungi Kami

Jika anda mempunyai soalan tentang Dasar Privasi ini, hubungi:

- E-mel: lpjustdoit@163.com

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
