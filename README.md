# Faucet Mavryk Network


## Fitur Utama

-   **Otomatisasi Penuh**: Jalankan sekali dan biarkan bot bekerja sesuai siklus yang Anda tentukan.
-   **Dukungan Multi-Akun**: Gunakan beberapa akun Telegram (file `.session`) untuk melakukan klaim.
-   **Dukungan Multi-Alamat**: Daftarkan semua alamat wallet Anda di `address.txt` dan bot akan memproses semuanya.
-   **Siklus Berulang**: Bot akan otomatis mengulang seluruh proses setiap `X` jam, sesuai konfigurasi di `config.json`.
-   **Antarmuka Interaktif**: Tampilan status *real-time* dalam bentuk tabel yang rapi dan menu yang mudah digunakan.
-   **Konfigurasi Mudah**: Pengaturan API, delay, dan jadwal perulangan dapat diubah dengan mudah melalui file `config.json`.
-   **Logging**: Semua aktivitas dicatat dalam file `laporan_faucet.csv` untuk kemudahan pelacakan.



## Prasyarat

-   Python 3.8 atau lebih baru.
-   API ID dan API Hash dari Telegram. Anda bisa mendapatkannya di [my.telegram.org](https://my.telegram.org).



## Instalasi & Konfigurasi

1.  **Clone Repositori**
    ```bash
    git clone 
    ```
2.  **Masuk ke Directory**
    ```
    cd mavrykfaucet
    ```
2.  **Install Dependensi**
    ```
    pip install telethon rich 
    ```

3.  **Isi Alamat Wallet**
    Buka file `address.txt` dan masukkan semua alamat wallet Anda. Setiap alamat harus berada di baris baru.
    ```
    0x...AlamatPertama...
    0x...AlamatKedua...
    0x...AlamatKetiga...
    ```

4.  **Setting Konfigurasi** :
    Isi **API ID** dan **API Hash** (WAJIB). Setting delay sesuka hati anda di `config.json`



## Cara Penggunaan

1.  **Jalankan Skrip**
    ```bash
    python bot.py
    ```

2.  **Buat Sesi Baru**
    -   Jika sudah ada langsung pilih opsi `1` atau `enter` untuk menjalankan bot
    -   Jika belum ada buat sesi, pilih opsi `2. Buat Sesi Baru`.
    -   Ikuti instruksi untuk menambahkan akun Telegram Anda (memasukkan nomor telepon, kode verifikasi, dan kata sandi 2FA jika ada).
    -   Ulangi langkah ini untuk semua akun Telegram yang ingin Anda gunakan. Sesi akan disimpan di dalam folder `sessions`.

4.  **Jalankan Proses Faucet**
    -   Setelah minimal satu sesi dibuat, pilih opsi `1. Jalankan Proses Faucet`.
    -   Bot akan mulai bekerja dan menampilkan prosesnya secara *real-time*.



## Disclaimer

Skrip ini dibuat untuk tujuan edukasi dan otomatisasi tugas pribadi. Penggunaan secara berlebihan atau tidak wajar dapat menyebabkan akun Telegram Anda dibatasi oleh pihak Telegram. Gunakan dengan bijak.
