# Your Style, Your Story — Aksesoris Premium

Website e-commerce sederhana (HTML + CSS + JavaScript murni) untuk toko aksesoris fashion. Proyek ini dibuat sebagai bagian dari tugas pengembangan website toko online, mencakup katalog produk, keranjang belanja, form pemesanan, dan simulasi pembayaran.

---

## 1. Ikhtisar Bisnis

### Nama Bisnis, Deskripsi, dan Proposisi Nilai
**Your Style, Your Story** adalah toko aksesoris premium yang menjual perhiasan dan aksesoris fashion seperti gelang, kalung, cincin, anting, jam tangan, dan gengge/anklet. Tagline toko adalah *"Your Story"* — merefleksikan filosofi bahwa setiap aksesoris yang dikenakan pelanggan adalah bagian dari cerita gaya hidup mereka sendiri.

**Proposisi nilai:** menyediakan aksesoris berkualitas dengan desain elegan dan harga terjangkau, disertai pengalaman belanja online yang mudah, aman, dan personal (transaksi bisa dikonfirmasi langsung lewat WhatsApp).

### Target Pasar & Segmentasi Pelanggan
- **Demografi:** Wanita muda hingga dewasa (usia ±15–35 tahun), khususnya pengguna aktif Instagram dan TikTok.
- **Psikografis:** Konsumen yang peduli penampilan, mengikuti tren fashion aksesoris, dan menyukai belanja online yang praktis.
- **Geografis:** Awalnya berfokus pada area Bandung, Jawa Barat, dengan potensi perluasan ke seluruh Indonesia melalui pengiriman online.

### Analisis Pasar Singkat & Pesaing
Industri aksesoris fashion di Indonesia tumbuh pesat seiring meningkatnya belanja online dan tren self-expression melalui gaya berpakaian. Kompetisi datang dari toko aksesoris lokal di marketplace (Shopee, Tokopedia) maupun toko serupa di Instagram/TikTok Shop. Keunggulan kompetitif "Your Style, Your Story" terletak pada branding personal, katalog visual yang rapi, serta kemudahan checkout langsung di website sendiri tanpa potongan biaya platform pihak ketiga.

### Strategi Manajemen Produk & Katalog
Produk dikelompokkan ke dalam 6 kategori utama:
| Kategori | Contoh Produk |
|---|---|
| Gelang | Chloe Chain Bracelet, Elsa Classic Bangle |
| Kalung | Luna Crescent Pendant |
| Cincin | Vania Solitaire Ring |
| Anting | Daisy Long Chain Earrings |
| Jam Tangan | Aurelius Executive Gold, Celestia Rose Gold Watch |
| Gengge / Anklet | Gema Summer Anklet |

Setiap produk memiliki nama yang menarik (branding storytelling), foto visual, kategori, dan label harga yang jelas—ditampilkan dalam bentuk kartu katalog yang bisa difilter berdasarkan kategori atau dicari lewat kolom pencarian.

### Model Bisnis & Aliran Pendapatan
Model bisnis bersifat **direct-to-consumer (D2C)** — penjualan dilakukan langsung ke konsumen tanpa perantara marketplace. Aliran pendapatan berasal dari penjualan produk aksesoris satuan maupun dalam jumlah (multi-item per pesanan), dengan pembayaran melalui transfer bank, e-wallet, QRIS, atau tunai (COD/di tempat).

### Strategi Harga, Promosi, dan Diskon
- Harga produk berkisar antara Rp110.000 – Rp425.000, disesuaikan dengan kategori dan bahan.
- Promosi utama dilakukan melalui Instagram dan TikTok (tautan kontak tersemat di halaman "Kontak Kami").
- Struktur website sudah disiapkan agar mudah menambahkan komponen diskon/voucher di masa depan (misalnya pada total keranjang) untuk mendukung strategi promosi musiman.

### Proses Checkout & Simulasi Payment Gateway
Alur pemesanan pada website:
1. Pelanggan memilih produk dari katalog → masuk ke **Keranjang**.
2. Pelanggan mengisi **Form Pemesanan** (nama, alamat, username Instagram, no. HP).
3. Pelanggan memilih salah satu metode pembayaran:
   - 💵 **Cash** (bayar di tempat)
   - 📱 **QRIS**
   - 🏦 **Transfer Bank (BNI)** — nomor rekening dummy ditampilkan otomatis
   - 💳 **E-Wallet (DANA)** — nomor tujuan dummy ditampilkan otomatis
4. Setelah memilih metode, muncul **modal pembayaran** berisi instruksi dan total tagihan.
5. Pelanggan diminta mengirim bukti transfer melalui WhatsApp untuk konfirmasi pesanan.

> Catatan: metode transfer bank & e-wallet pada proyek ini bersifat **simulasi/dummy** (tidak terhubung ke payment gateway sungguhan seperti Midtrans/Xendit/PayPal), sesuai kebutuhan tugas.

### Rencana SEO, Keamanan, dan Pemeliharaan
- **SEO:** penggunaan tag `<title>`, `<meta viewport>`, struktur heading (`h1`, `h2`) yang jelas, serta nama produk yang deskriptif untuk mendukung pencarian.
- **Keamanan:** input pelanggan (form pemesanan) divalidasi di sisi klien; ke depannya perlu ditambahkan validasi server-side dan enkripsi data saat terhubung ke backend/database sungguhan.
- **Pemeliharaan:** kode disusun modular (HTML/CSS/JS dalam satu file untuk versi awal) agar mudah dipecah menjadi folder terpisah (`css/`, `js/`, `images/`) saat proyek berkembang; produk dan gambar dapat diperbarui langsung melalui variabel data di JavaScript.

### Rencana Penggunaan Data Analitik untuk Pengambilan Keputusan
Rencana ke depan adalah mengintegrasikan tools analitik (misalnya Google Analytics) untuk melacak:
- Produk yang paling sering dilihat/dimasukkan ke keranjang.
- Metode pembayaran yang paling sering dipilih pelanggan.
- Sumber traffic (Instagram, TikTok, pencarian langsung).

Data ini akan digunakan untuk menentukan produk mana yang perlu di-restock, kategori mana yang perlu diperluas, serta metode pembayaran mana yang perlu diprioritaskan dalam UX checkout.

---

## 2. Fitur Utama Website
- Landing page dengan hero carousel produk unggulan
- Katalog produk dengan filter kategori & pencarian
- Keranjang belanja interaktif (tambah/kurangi/hapus item)
- Form pemesanan (nama, alamat, Instagram, no. HP)
- Simulasi 4 metode pembayaran (Cash, QRIS, BNI, DANA)
- Halaman kontak (WhatsApp, Email, Instagram, TikTok, alamat toko)
- Desain responsif untuk mobile dan desktop

## 3. Teknologi
- **HTML5** — struktur halaman
- **CSS3 murni** — styling (custom properties, flexbox, grid, media query)
- **JavaScript (vanilla)** — logika katalog, keranjang, dan modal pembayaran

## 4. Struktur Folder
```
.
├── index.html
├── README.md
├── css/        (opsional, jika dipisah dari index.html)
├── js/         (opsional, jika dipisah dari index.html)
└── images/     (opsional, jika gambar produk dipisah dari base64)
```

## 5. Cara Menjalankan
1. Clone atau download repository ini.
2. Buka file `index.html` langsung di browser, **atau**
3. Deploy melalui **GitHub Pages** untuk mengakses secara online.

## 6. Kontak
- WhatsApp: 0856-0394-6912
- Email: lindaiduy08@gmail.com
- Instagram: [@linda08.06](https://instagram.com/linda08.06)
- TikTok: [@ndaaaa0886](https://tiktok.com/@ndaaaa0886)
- Alamat: Jln. Cipedes Hegas No.50, Rt 03, Rw 03, Kontrakan Pak Dede, Pajajaran, Cicendo, Kota Bandung, Jawa Barat, Indonesia

---
© 2026 Your Style, Your Story — Aksesoris untuk setiap cerita Anda.
