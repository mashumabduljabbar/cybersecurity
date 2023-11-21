# Laporan Keamanan - Uji Penetrasi Situs Web E-Commerce

## Injection Attacks (SQL Injection):
- **URL Pencarian Produk:** `https://www.satubaju.com/find-q-putih?key=product' OR '1'='1`
- **Temuan:** Situs rentan terhadap serangan SQL injection dengan menggunakan input tertentu.

## Cross-Site Scripting (XSS):
- **URL Kolom Komentar:** `https://www.satubaju.com/Kaos-Paris-Bonjour,14905?comment=<script>alert('XSS')</script>`
- **Temuan:** Situs  tidak rentan terhadap serangan XSS melalui kolom komentar.

## Insecure Direct Object References:
- **URL Akses Data Tidak Sah:** `https://www.satubaju.com/user/orders/9999`
- **Temuan:** Situs tidak dapat dimanipulasi untuk mengakses data yang tidak seharusnya dapat diakses.

## Insecure File Upload:
- **URL Unggah File Berbahaya:** `https://www.satubaju.com/upload?file=evilscript.php`
- **Temuan:** Situs tidak dapat menerima dan menjalankan file berbahaya, mengancam keamanan.

---

**Saran Perbaikan:**
1. Melakukan validasi input dengan lebih ketat untuk mencegah serangan SQL injection.
2. Membersihkan input pengguna sebelum menampilkannya untuk mencegah serangan XSS.
3. Memastikan bahwa akses langsung ke data atau file dibatasi dengan benar.
4. Mengimplementasikan validasi dan pembatasan yang ketat pada unggahan file.
