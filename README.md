<div align="center">

# SI-PANDRI
### Sistem Pengelolaan Parfait Laundry

**Laundry Lebih Mudah, Lebih Teratur.**

Proyek UTS Dasar Pemrograman (DP2) · Tim SEPAKAT  
Program Studi Ilmu Komputer · Fasilkom-TI · Universitas Sumatera Utara

![Free Pascal](https://img.shields.io/badge/Free%20Pascal-3.2.2-blue)
![Platform](https://img.shields.io/badge/Platform-Windows-lightgrey)

</div>

## Tentang Proyek

**SI-PANDRI (Sistem Pengelolaan Parfait Laundry)** adalah aplikasi administrasi laundry berbasis terminal yang dibuat menggunakan Free Pascal. Aplikasi ini membantu admin dan pelanggan mengelola pesanan laundry, mulai dari registrasi akun, pemesanan, penimbangan, perhitungan biaya, pembaruan status cucian dan pembayaran, hingga pembuatan laporan transaksi.

Data aplikasi disimpan dalam file lokal `.dat`, sehingga data tetap tersedia ketika program dijalankan kembali.

## Anggota Kelompok

| No. | Nama | NIM | KOM | Laboratorium |
|---:|---|---|:---:|---|
| 1 | Syahril Maimubdy | 261401130 | A | LAB DP2 |
| 2 | Sabitha Sarah | 261401124 | A | LAB DP2 |
| 3 | Gilbert Kindly | 261401127 | A | LAB DP2 |

## Fitur Utama

### Menu Pelanggan
- Registrasi dan login akun pelanggan.
- Membuat pesanan laundry dengan pilihan layanan dan metode pembayaran.
- Melihat daftar pesanan serta mengecek status pesanan.
- Mengubah metode pembayaran sesuai ketentuan sistem.
- Menghubungi admin melalui tautan WhatsApp yang disiapkan program.

### Menu Admin
- Melihat dan mencari pesanan pelanggan.
- Memasukkan berat aktual laundry dan menghitung biaya otomatis berdasarkan berat serta tarif per kilogram.
- Mengatur tarif layanan dan informasi pembayaran.
- Memperbarui status pembayaran dan status cucian.
- Menyiapkan pesan tagihan atau pemberitahuan melalui WhatsApp.
- Melihat daftar pelanggan dan laporan transaksi.

### Contoh Perhitungan Biaya

| Layanan | Tarif per kg | Berat | Total |
|---|---:|---:|---:|
| Reguler | Rp6.000 | 3,5 kg | Rp21.000 |
| Express | Rp10.000 | 2,5 kg | Rp25.000 |

Total biaya dihitung menggunakan rumus:

`Total biaya = berat aktual × tarif per kilogram`

## Penerapan Materi Dasar Pemrograman

Program menerapkan materi yang dipersyaratkan dalam UTS Dasar Pemrograman DP2:

| Materi | Penerapan dalam Program |
|---|---|
| Input dan output | `write`, `writeln`, `read`, dan `readln` untuk interaksi dengan pengguna. |
| Variabel dan tipe data | Penggunaan `string`, `integer`, `real`, `boolean`, `char`, serta `record`. |
| Struktur pengkondisian | `if-then-else`, nested-if, dan `case-of` untuk validasi, pemilihan layanan, dan pengelolaan menu. |
| Perulangan | `repeat-until`, `while-do`, dan `for-to-do` untuk menu, validasi input, serta pemrosesan data. |
| Kontrol perulangan | `break` untuk menghentikan pencarian ketika data ditemukan. |
| Menu interaktif | Menu utama, admin, dan pelanggan yang berjalan menggunakan perulangan `repeat-until`. |
| Pengolahan file | File `.dat` digunakan untuk menyimpan data pelanggan, pesanan, dan pengaturan. |

## Struktur Repositori

```text
UTS_Daspro_Sepakat_A/
├── README.md
├── LICENSE
├── SI_PANDRI.pas
├── SI_PANDRI.exe
├── SI_PANDRI.o
├── Run-Terminal-SI-PANDRI.pdf
├── pandri_pelanggan.dat
├── pandri_pengaturan.dat
└── pandri_pesanan.dat
```

- `SI_PANDRI.pas` — source code utama program Pascal.
- `SI_PANDRI.exe` — program hasil kompilasi untuk Windows.
- `SI_PANDRI.o` — file objek hasil kompilasi.
- `Run-Terminal-SI-PANDRI.pdf` — dokumentasi berupa tangkapan layar hasil program.
- `pandri_*.dat` — file data pelanggan, pesanan, dan pengaturan.
- `README.md` — dokumentasi proyek.

## Cara Menjalankan

### Menjalankan program di Windows

1. Unduh atau klon repositori ini.
2. Buka folder repositori.
3. Jalankan `SI_PANDRI.exe`.

### Kompilasi dari source code

Pastikan Free Pascal Compiler (FPC) telah terpasang, kemudian jalankan perintah berikut dari folder repositori:

```bash
fpc SI_PANDRI.pas
```

Setelah kompilasi berhasil, jalankan `SI_PANDRI.exe` di Windows.

**Login admin demo:** `admin`  
**Password:** `admin123`

Gunakan akun tersebut untuk demonstrasi kelas. Informasi rekening yang tersedia di program merupakan contoh dan perlu diperiksa sebelum digunakan untuk demonstrasi pembayaran.

## Dokumentasi

Lihat [Run-Terminal-SI-PANDRI.pdf](Run-Terminal-SI-PANDRI.pdf) untuk dokumentasi tangkapan layar hasil program.

## Catatan

- Program dirancang untuk penggunaan lokal pada satu komputer.
- WhatsApp hanya dibuka melalui tautan yang disiapkan program; pesan tidak dikirim otomatis.
- Pembayaran tidak terhubung langsung ke bank. Admin perlu memverifikasi pembayaran secara manual.
- File `.dat` menyimpan data lokal aplikasi. Hindari menggunakan kata sandi pribadi untuk akun demo.

---

**Tim SEPAKAT** · UTS Dasar Pemrograman DP2  
Ilmu Komputer · Fasilkom-TI · Universitas Sumatera Utara
