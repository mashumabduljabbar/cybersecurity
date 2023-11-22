### Checklist Android Pentest

#### 1. **Rekognisi:**
   - [ ] Identifikasi aplikasi target beserta versinya.
   - [ ] Kumpulkan informasi tentang infrastruktur target.
   - [ ] Enumerasi layanan yang berjalan pada target.

#### 2. **Analisis Statis:**
   - [ ] Dekompilasi APK menggunakan alat seperti JADX atau JADX-GUI.
   - [ ] Tinjau kode sumber untuk potensi kerentanan.
   - [ ] Identifikasi kredensial tertanam atau informasi sensitif.
   - [ ] Periksa penyimpanan data yang tidak aman.

#### 3. **Analisis Dinamis:**
   - [ ] Siapkan lingkungan pengujian dengan emulator atau perangkat fisik.
   - [ ] Gunakan alat seperti Frida atau Xposed untuk manipulasi waktu eksekusi.
   - [ ] Intersep dan analisis lalu lintas jaringan untuk potensi masalah keamanan.
   - [ ] Uji kerentanan waktu eksekusi seperti injeksi kode atau manipulasi waktu eksekusi.

#### 4. **Uji Otentikasi dan Otorisasi:**
   - [ ] Uji mekanisme otentikasi yang lemah atau tidak aman.
   - [ ] Verifikasi manajemen sesi untuk penggunaan token yang benar.
   - [ ] Periksa apakah mekanisme otorisasi kuat dan menerapkan kontrol akses yang benar.

#### 5. **Uji Penyimpanan Data:**
   - [ ] Periksa bagaimana data sensitif disimpan di perangkat.
   - [ ] Periksa enkripsi data sensitif.
   - [ ] Uji praktik penyimpanan data yang tidak aman.

#### 6. **Uji Komunikasi Jaringan:**
   - [ ] Verifikasi penggunaan protokol komunikasi yang aman (misalnya, HTTPS).
   - [ ] Periksa kerentanan SSL/TLS.
   - [ ] Uji transmisi data yang tidak aman.

#### 7. **Kualitas Kode dan Praktik Kode Aman:**
   - [ ] Evaluasi kualitas kode secara keseluruhan.
   - [ ] Cari konfigurasi keamanan yang tidak benar.
   - [ ] Periksa penanganan kesalahan yang benar untuk mencegah kebocoran informasi.

#### 8. **Rekayasa Balik:**
   - [ ] Gunakan alat seperti JADX atau APKTool untuk rekayasa balik.
   - [ ] Analisis perilaku aplikasi untuk mengidentifikasi kelemahan keamanan.
   - [ ] Cari kode tersembunyi atau terobosan.

#### 9. **OWASP Top 10:**
   - [ ] Verifikasi aplikasi terhadap OWASP Top 10 Mobile Risks terbaru.
   - [ ] Prioritaskan dan tangani kerentanan yang diidentifikasi.

#### 10. **Pelaporan:**
   - [ ] Dokumentasikan semua temuan, termasuk langkah-langkah yang detail untuk mereproduksi.
   - [ ] Berikan rekomendasi untuk perbaikan.
   - [ ] Pastikan laporan jelas, ringkas, dan dapat diimplementasikan.

#### 11. **Tindakan Setelah Pengujian:**
   - [ ] Verifikasi bahwa masalah yang dilaporkan telah diperbaiki.
   - [ ] Lakukan pengujian ulang untuk mengonfirmasi efektivitas perbaikan.
   - [ ] Pertimbangkan memberikan pelatihan atau panduan kepada pengembang berdasarkan masalah yang diidentifikasi.
