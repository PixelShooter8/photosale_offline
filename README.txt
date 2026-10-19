PHOTOSALE OFFLINE — PAKET ANDROID
=================================

Fail:
- index.html: aplikasi pengiraan
- manifest.webmanifest: metadata pemasangan
- sw.js: cache offline/service worker
- icon-192.png dan icon-512.png: ikon aplikasi

PENTING: Pakej ZIP ini belum dipasang pada telefon dan belum diterbitkan di alamat HTTPS. PWA offline memerlukan satu persediaan awal melalui HTTPS.

Kaedah penggunaan:
1. Simpan ZIP ini dan ekstrak semua fail.
2. Untuk pemasangan seperti aplikasi Android, muat naik kandungan folder ini ke hosting statik yang menyokong HTTPS (contohnya GitHub Pages atau hosting web anda).
3. Buka URL HTTPS itu menggunakan Chrome pada Android semasa ada internet.
4. Pilih menu Chrome (⋮) > Install app / Add to Home screen, jika pilihan itu muncul.
5. Buka aplikasi sekurang-kurangnya sekali ketika online. Selepas fail aplikasi dicache, aplikasi boleh dibuka offline.
6. Import laporan XLSX/CSV. Semua pengiraan dilakukan dalam pelayar; data jualan disimpan setempat pada telefon.
7. Selepas setiap event, tekan “Sandaran JSON” dan simpan fail sandaran ke lokasi yang selamat.

Formula:
- Untuk setiap Order ID, Gross Profit (order), Photohawk Fee (order), Transaction Fee (order) dan Shipping Fee (order) diambil sekali.
- Nilai order dan yuran diagihkan sama rata kepada bilangan baris gambar dalam order tersebut.
- Bersih diagih = kasar diagih - yuran PhotoHawk diagih - yuran transaksi diagih - penghantaran diagih.
- Anggaran bayaran jurufoto = bahagian bersih diagih × peratus agihan jurufoto.
- Penanda nama fail yang tidak dikenali dikecualikan daripada jumlah bayaran sehingga diperbetulkan.
- Semak hasil dengan penyata rasmi PhotoHawk sebelum membuat pembayaran.

Privasi dan batasan:
- Data diproses dan disimpan dalam storan pelayar pada peranti ini; ia tidak disegerakkan ke telefon lain.
- Jangan padam data pelayar tanpa membuat sandaran.
- Aplikasi ini tidak mengesahkan pembayaran bank secara automatik.
- PWA service worker berfungsi melalui HTTPS atau localhost, bukan sekadar membuka index.html dari file://.
- Pembacaan XLSX menggunakan parser ringan terbina dalam; fail XLS lama perlu disimpan semula sebagai XLSX atau CSV.
