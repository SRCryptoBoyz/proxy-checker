# Pemeriksa Jenis Proxy

## Deskripsi
Script ini memeriksa validitas proxy dengan mencoba untuk terhubung dan menentukan apakah setiap proxy termasuk jenis Datacenter atau Residential.

## Fitur
- **Memeriksa apakah proxy aktif atau tidak dan secara otomatis menyimpan ke `datacenter.txt` atau `residental.txt` tergantung jenis proxy.**

## Prasyarat
- [Python](https://www.python.org) (Versi 3.6 atau lebih tinggi)

## Instalasi

1. Clone repositori :
   ```bash
   git clone https://github.com/recitativonika/proxy-type-checker.git
   ```
2. Masuk ke direktori proyek:
   ```bash
   cd proxy-type-checker
   ```
3. Instal dependensi yang diperlukan:
   ```bash
   pip install -r requirements.txt
   ```

## Cara Penggunaan

1. masukan daftar proxy lu di file `proxy.txt` sebelum jalanin bot nya, Contoh format:
   ```
   ip:port
   username:password@ip:port
   http://ip:port
   http://username:password@ip:port
   socks5://ip:port
   socks5://username:password@ip:port
   ```

2. Jalankan script:
   ```bash
   python main.py
   ```

3. Script akan memeriksa proxy yg valid/aktif atau tidak dan menyimpan daftar proxy ke dalam file `residental.txt` atau `datacenter.txt` tergantung pada jenis proxy nya.
