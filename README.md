# GS015 — Grand Senheng Kemaman

Google Review Helper untuk pelanggan GS015. Website statik satu fail (`index.html`), mesra telefon, tanpa pemasangan atau API key.

Link: https://guitarheero-sketch.github.io/GS015_review/

Link staf: tambah `?staff=9861` (atau `?staff=SH9861`) hujung URL. Kod staf akan dikunci dan masuk sebagai hashtag.

## Fungsi

- 6 kategori: Dapat S-Coin, Redeem S-Coin, Dapat PlusOne, Claim PlusOne, Tambah RW, Claim RW.
- Setiap ayat dibina rawak daripada 4 bahagian: pembuka + isi + komen servis + penutup. Ratusan ribu hingga jutaan kombinasi bagi setiap kategori, dipilih rawak setiap kali page dibuka atau "Ayat lain" ditekan.
- Butang "← Sebelum" untuk balik ke ayat tadi.
- Hujung review ada 2 hashtag: `#SHxxxx #GrandSenhengKemaman`.
- Kategori warranty perlu tick pengesahan sebelum copy.
- Copy & buka Google, Copy sahaja, atau Buka Google sahaja.
- Pelanggan pilih bintang sendiri ikut pengalaman sebenar.

## Peraturan dalam ayat

- **Dapat S-Coin:** harga, % cashback, jumlah S-Coin dan nilai RM (selepas tolak 5% maintenance fee). S-Coin sah setahun.
- **Redeem S-Coin:** tebus 100% guna S-Coin, RM1 = 100 S-Coin; ayat sebut jumlah S-Coin dan nilai barang.
- **Dapat PlusOne:** Senheng PlusOne® Membership (yuran dari RM12, sah setahun). Warranty kilang + 1 tahun. TV tak layak.
- **Claim PlusOne:** pilih "Repair, kos ditanggung" atau "Tak boleh repair, dapat baru".
- **Tambah RW:** small appliance bawah RM400. Ayat sebut harga RW, warranty 1 + 1 = 2 tahun, rosak tukar baru.
- **Claim RW:** rosak dalam 2 tahun, tukar baru on the spot.

## Mengubah ayat

Semua ayat ada dalam elemen `<script type="application/json" id="reviewData">` dalam `index.html` (`openers`, `service`, dan `cores` / `closers` bagi setiap kategori). Fail JSON lama dalam repo ni (`gs015-review-comments.json`, `scoin_comments*.json`) tak lagi digunakan oleh page.

Konfigurasi outlet: Place ID `ChIJsTTf4iuGyDERHjGUr39tto0`.
