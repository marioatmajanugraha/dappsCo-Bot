# dAppsCo-Bot 🦁

Script ini digunakan untuk mengotomatiskan farming ROAR di platform [dApps.co](https://dapps.co) dengan antarmuka tabel CLI yang elegan dan hitungan mundur waktu nyata.

---

## 📌 Fitur

- ✅ Auto farming dan klaim ROAR untuk semua akun menggunakan cookie dari `cookies.txt`
- ⏳ Hitungan mundur waktu nyata (`time_remaining`) diperbarui setiap detik dalam tabel CLI
- 📊 Tampilan tabel interaktif dengan `cli-table3` (Handle, Roar Holdings, Time Remaining, Status)
- 🔌 Dukungan proxy (`proxy.txt`) untuk koneksi aman dan menghindari rate limit
- 🎁 Menampilkan hasil klaim (jumlah ROAR) dan info akun (Roar Holdings) secara real-time
- ⚡ Manajemen multi-akun dengan penanganan error otomatis (cookie kadaluarsa, rate limit)
- 🎮 Pilihan mode proxy melalui prompt interaktif (y/n)

---

## 🚀 Cara Penggunaan

### 1. Clone repository ini

```sh
git clone https://github.com/marioatmajanugraha/dappsCo-Bot.git
cd dappsCo-Bot
```

### 2. Install Dependencies

```sh
npm install axios chalk@4 cfonts http-proxy-agent socks-proxy-agent readline-sync cli-table3
```

### 3. Siapkan file konfigurasi

#### a. Buat `cookies.txt`

Isi dengan cookie akun dApps.co, satu per baris. Bisa berupa raw string atau JSON:

Contoh raw string:

```txt
_ga=GA1.1.950983283...; privy-token=...
```

Contoh JSON:

```json
{"handle":"Contohxyz888","cookie":"_ga=GA1.1.950983283..."}
```

#### b. (Opsional) Buat `proxy.txt`

Jika ingin menggunakan proxy, isi dengan format seperti ini:

```txt
http://username:password@host:port
socks5://username:password@host:port
```

### 4. Jalankan Script

```sh
node index.obf.js
```

### 5. Ikuti Instruksi

- Pilih apakah ingin menggunakan proxy (y/n)
- Jika `cookies.txt` berisi raw string, masukkan handle akun (contoh: Balveerxyz888)
- Script akan berjalan otomatis, menampilkan tabel dengan hitungan mundur setiap detik

---

⚠️ **Disclaimer**

Gunakan script ini dengan bijak dan sesuai aturan dApps.co. Developer tidak bertanggung jawab atas penyalahgunaan atau banned akun.

---

## 🤝 Kontribusi

Jika ingin berkontribusi, silakan fork repo ini dan ajukan pull request! Kami terbuka untuk ide baru, seperti penambahan fitur atau optimalisasi.

---

## 📞 Kontak

Jika ada pertanyaan, hubungi: [@balveerxyz](https://t.me/balveerxyz)  
Join channel Telegram gratis: [t.me/airdroplocked](https://t.me/airdroplocked)
