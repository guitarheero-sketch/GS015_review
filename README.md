# GS015 — Grand Senheng Kemaman

Google Review Helper untuk pelanggan GS015. Website statik, mesra telefon, tanpa pemasangan atau API key.

## Publish di GitHub Pages

1. Extract ZIP ini.
2. Buat repository public, contohnya `gs015-review-helper`.
3. Upload `index.html`, `gs015-review-comments.json`, dan `.nojekyll` terus ke root repository (jangan letak dalam subfolder).
4. Dalam Settings > Pages, pilih deployment daripada branch `main`, folder `/ (root)`, kemudian Save.
5. Selepas deployment selesai, buka URL Pages yang GitHub paparkan.

Link staf boleh ditambah dengan `?staff=SH12345` pada hujung URL website. Gantikan dengan kod staf sebenar (SH + 3–8 digit).

## Fungsi

- 7 kategori, 50 komen setiap kategori: jumlah 350.
- Pilihan kumpulan Semua / Servis / S-Coin / Warranty.
- Ayat boleh dipilih, ditukar dan diedit sebelum disalin.
- Kiraan S-Coin dan penukaran RM kepada S-Coin.
- Pengesahan pengalaman warranty sebelum copy.
- Draf dan sejarah disimpan pada peranti pelanggan.
- Pilihan copy sahaja, buka Google sahaja, atau copy dan buka Google.
- Pelanggan semak dan hantar sendiri menggunakan akaun Google mereka.

## Konfigurasi outlet

Nama: Grand Senheng Kemaman
Kod: GS015
Place ID: ChIJsTTf4iuGyDERHjGUr39tto0
Hashtag: #GrandSenhengKemaman

## Mengubah komen

Fail `gs015-review-comments.json` menyimpan komen. Kekalkan struktur, 50 komen setiap kategori, placeholder dan hashtag yang diperlukan. Salinan backup JSON juga berada dalam elemen `fallbackData` dalam `index.html`. Kemas kini kedua-duanya dan revision bersama supaya backup sepadan.

Senario warranty berdasarkan konteks outlet yang diberikan. Pelanggan perlu memilih ayat yang sesuai dengan pembelian atau tuntutan sebenar mereka.

## Semakan

Syntax JavaScript dan ujian simulasi DOM lulus untuk kategori, pengiraan, salinan, draf, validasi staf, pengesahan warranty, pautan Google dan backup offline. Semak paparan pada telefon selepas publish.
