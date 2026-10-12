# Digibouquet

Web statis berbahasa Indonesia untuk mengirim bunga digital, catatan, dan lagu YouTube.

## Pengembangan lokal

Dari direktori repositori, jalankan:

```sh
python3 -m http.server 3000 --bind 0.0.0.0
```

Tidak memerlukan dependensi, database, atau API key. Buka halaman, isi hadiah, buat tautan, lalu buka tautan itu untuk melihat tampilan penerima. Isi hadiah dikodekan dalam URL fragment (bukan dienkripsi); jangan gunakan untuk pesan rahasia. Tautan bisa panjang untuk catatan yang panjang.

## Vercel

Push kode ke GitHub, impor repositori di Vercel, pilih framework **Other**, tanpa build command dan output directory `.`. Deploy dari root repositori. Tidak memerlukan environment variables. Buat tautan hadiah dari alamat deployment agar bisa diakses orang lain.

Pemutaran lagu menggunakan embed resmi YouTube. Halaman hadiah mencoba autoplay dengan suara saat dibuka; browser dapat memblokirnya sampai pengguna menekan tombol Putar lagi. Pemilik video dapat membatasi embed; tersedia tautan untuk membuka YouTube langsung. Font Google opsional; font sistem digunakan jika tidak tersedia. Bunga versi awal menggunakan emoji dan tampilannya mengikuti perangkat.
