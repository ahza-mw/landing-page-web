# landing-page-web
cara edit
Berikut panduan lengkap cara mengedit landing page-nya! Semuanya mudah, tidak perlu keahlian coding.

🖼️ 1. Ganti Foto Produk
Cari bagian <svg ... > placeholder, ganti dengan tag <img>:
html<!-- SEBELUM (hapus seluruh tag <svg>...</svg>) -->
<svg width="100%" viewBox="0 0 300 400" ...> ... </svg>

<!-- SESUDAH -->
<img src="foto-produk-1.jpg" alt="Tas Anyam Rotan" style="width:100%;height:100%;object-fit:cover;">
Lakukan hal yang sama untuk hero, story, dan setiap produk.

💰 2. Ubah Nama Produk & Harga
Cari teks ini di dalam file, lalu ganti sesuai produk Anda:
html<!-- Nama produk -->
<div class="product-name">Tas Anyam Rotan</div>

<!-- Deskripsi singkat -->
<div class="product-desc">Dianyam manual dengan rotan pilihan</div>

<!-- Harga baru & harga coret -->
<span class="product-price">Rp 285.000</span>
<span class="product-price-old">Rp 350.000</span>  <!-- hapus baris ini kalau tidak ada diskon -->

📱 3. Ubah Nomor WhatsApp
html<!-- Cari baris ini -->
<a href="https://wa.me/6281234567890" ...>

<!-- Ganti angkanya, format: 62 + nomor tanpa 0 di depan -->
<a href="https://wa.me/628123456789" ...>

✍️ 4. Ubah Teks Hero & Judul
html<!-- Judul utama -->
<h1 class="hero-title">Produk Handmade<br><em>Unik & Berkualitas</em></h1>

<!-- Subjudul -->
<p class="hero-sub">Dibuat dengan detail dan penuh ketelitian...</p>
Teks di dalam tag <em> akan otomatis berwarna terracotta/oranye.

🎨 5. Ganti Warna Tema
Semua warna ada di bagian :root di awal file CSS. Cukup ubah kode warnanya:
css:root {
  --cream: #F9F3EA;         /* warna background utama */
  --terracotta: #C4795A;    /* warna aksen/highlight → ganti ini untuk ubah aksen */
  --brown-dark: #3B2A1A;    /* warna teks & tombol gelap */
  --sage: #8A9B7A;          /* warna hijau aksen */
  --gold: #C8A060;          /* warna bintang & gold detail */
}

💬 6. Edit Testimoni
html<p class="testi-text">Ganti dengan ulasan pelanggan asli Anda di sini...</p>

<div class="testi-name">Nama Pelanggan</div>
<div class="testi-loc">Kota, Indonesia</div>

<!-- Huruf avatar (otomatis pakai huruf pertama nama) -->
<div class="testi-avatar">R</div>

📦 7. Edit Paket Harga
html<div class="price-name">Paket Satuan</div>       <!-- Nama paket -->
<div class="price-amount">Rp 95rb</div>           <!-- Harga -->
<div class="price-period">per item</div>          <!-- Keterangan harga -->

<!-- List fitur paket -->
<li>1 produk pilihan</li>
<li>Packaging standar</li>

🏷️ 8. Ganti Label Tag Produk
html<!-- Pilihan warna tag: -->
<div class="product-tag">New</div>                              <!-- merah terracotta -->
<div class="product-tag" style="background:var(--sage)">Best Seller</div>   <!-- hijau -->
<div class="product-tag" style="background:var(--gold)">Limited</div>       <!-- gold -->

🔤 9. Ganti Nama Brand
html<!-- Di navbar & footer, cari: -->
<a class="nav-logo">Karya<span>Tangan</span></a>

<!-- Ganti dengan nama brand Anda: -->
<a class="nav-logo">Nama<span>Brand</span></a>
Kata di dalam <span> akan otomatis tampil miring berwarna terracotta.

Tips: Gunakan Ctrl+F (Find) di teks editor untuk mencari teks yang ingin diganti dengan cepat. Rekomendasi editor gratis: VS Code atau cukup Notepad++.
