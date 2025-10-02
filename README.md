# Callback — Halaman Callback

Sebuah halaman callback / webhook demo siap pakai, dibuat untuk memudahkan pengembang men-debug dan menguji endpoint callback. Cocok untuk integrasi cepat ke sistem internal, webhook third-party, atau serverless functions.

## Fitur Utama

- Form pengiriman callback (POST/PUT) dengan preview payload.
- Simulasi lokal (tidak mengirim ke server) untuk memeriksa payload.
- Preview JSON otomatis dan sanitasi input dasar.
- Menyimpan riwayat 20 callback terakhir di `localStorage`.
- Animasi halus menggunakan GSAP + CSS.
- Header X-Signature sederhana (opsional) untuk simulasi verifikasi.
- UI responsif, aksesibilitas dasar, dan mudah dimodifikasi.

## Cara Pakai

1. Simpan file `index.html` dan buka di browser.
2. Masukkan `Callback Endpoint (URL)` yang ingin diuji.
3. Edit payload (JSON) atau gunakan simulasi.
4. Klik **Kirim Callback** untuk mengirim. Lihat status dan riwayat.

## Deployment

File ini bersifat statis sehingga dapat dihosting di:
- GitHub Pages
- Netlify
- Vercel (static site)
- Atau server static lain

## Integrasi Server

Website ini hanya contoh client-side. Untuk penerimaan callback yang aman pada server produksi:
- Gunakan HTTPS
- Verifikasi signature HMAC di server
- Batasi rate requests dan detect replay attacks
- Log request dengan aman (tanpa menyimpan data sensitif secara plain)

## Kustomisasi & Pengembangan

- Tambahkan pilihan auth (Basic / Bearer) di UI
- Simpan history di server untuk analitik
- Tambahkan WebSocket untuk menampilkan status real-time dari server

## Lisensi

Callback — Lisensi: **Free Use License v1.0** (lihat `LICENSE`)

---

Terima kasih! Jika ingin saya buatkan versi dengan backend sederhana (Express / Serverless) atau dengan branding Anda, katakan saja.
