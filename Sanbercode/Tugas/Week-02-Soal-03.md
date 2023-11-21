# Tutorial SQL Injection dengan SQLMap dan DIOS

## 1. Pendahuluan

SQL Injection adalah teknik serangan di mana penyerang menyisipkan atau memanipulasi pernyataan SQL yang dieksekusi oleh aplikasi, dengan tujuan untuk mendapatkan akses atau informasi yang tidak sah dari basis data. Dalam tutorial ini, kita akan menggunakan alat SQLMap dan DIOS untuk melakukan SQL Injection.

## 2. SQLMap

### a. Instalasi SQLMap

- Install SQLMap melalui terminal dengan perintah:
```bash
pip install sqlmap
```

### b. Pemindaian SQL Injection
- Lakukan pemindaian SQL Injection pada URL target dengan perintah:

```bash
sqlmap -u "http://example.com/vulnerable_page.php?parameter=value"
```

- SQLMap akan mendeteksi dan mengeksploitasi kerentanan SQL Injection secara otomatis.


## 3. DIOS (Damn Insecure and Open Source)

### a. Instalasi DIOS

- Clone repositori DIOS dari GitHub:
```bash
  git clone https://github.com/stamparm/DIOS.git
```

### b. Eksploitasi SQL Injection dengan DIOS

- Navigasi ke direktori DIOS:
```bash
cd DIOS
```

- Jalankan DIOS dengan perintah:
```bash
python dios.py -u "http://example.com/vulnerable_page.php?parameter=value"
```

- DIOS akan melakukan serangan SQL Injection dan menampilkan hasilnya.

## 4. Kesimpulan
Dengan menggunakan SQLMap dan DIOS, Anda dapat dengan mudah mengidentifikasi dan mengeksploitasi kerentanan SQL Injection pada aplikasi web. Namun, ingatlah bahwa melakukan uji penetrasi pada sistem atau situs web tanpa izin dapat melanggar hukum. Selalu dapatkan izin tertulis sebelum melakukan uji penetrasi.