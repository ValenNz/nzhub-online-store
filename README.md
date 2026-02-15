# 🥝 The NZ Hub — E‑commerce (Laravel 10 + Blade)

Aplikasi e‑commerce sederhana berbasis **Laravel 10** dengan tampilan **Blade**. Proyek ini menampilkan konsep toko online yang menjual produk bertema Selandia Baru (NZ), dilengkapi fitur katalog, keranjang, checkout, dan panel admin.

> Cocok sebagai bahan pembelajaran Laravel full‑stack: routing, MVC, relasi database, autentikasi, dan manajemen transaksi.

---

## ✨ Fitur Utama

### Pengguna (Customer)

* 🔍 Melihat katalog produk & detail produk
* 🛒 Keranjang belanja (add / update / remove)
* 💳 Checkout & pilihan metode pembayaran
* 📦 Riwayat & pelacakan pesanan
* 👤 Registrasi & login akun

### Admin

* 📊 Dashboard statistik penjualan
* 📦 Manajemen produk (CRUD + gambar)
* 🗂️ Manajemen kategori
* 🧾 Manajemen pesanan & status order
* 👥 Manajemen user

---

## 🧱 Tech Stack

| Layer           | Teknologi                     |
| --------------- | ----------------------------- |
| Backend         | Laravel 10                    |
| Frontend        | Blade + Bootstrap / Tailwind  |
| Database        | MySQL / MariaDB               |
| Auth            | Laravel Auth                  |
| Package Manager | Composer & NPM                |
| Storage         | Laravel Storage (public disk) |

---

## 📂 Struktur Folder Penting

```
app/
 ├── Http/Controllers
 ├── Models
resources/
 ├── views
 ├── css
 ├── js
database/
 ├── migrations
 ├── seeders
routes/
 ├── web.php
public/
storage/
```

---

## ⚙️ Instalasi

### 1. Clone Repository

```bash
git clone https://github.com/username/repository-name.git
cd repository-name
```

### 2. Install Dependency

```bash
composer install
npm install
```

### 3. Setup Environment

```bash
cp .env.example .env
php artisan key:generate
```

### 4. Konfigurasi Database (.env)

```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=nzhub
DB_USERNAME=root
DB_PASSWORD=
```

### 5. Migrasi & Seeder

```bash
php artisan migrate --seed
```

### 6. Storage Link

```bash
php artisan storage:link
```

### 7. Jalankan Server

```bash
php artisan serve
npm run dev
```

Buka di browser:

```
http://127.0.0.1:8000
```

---

## 🔐 Akun Default (Seeder)

| Role  | Email                                       | Password |
| ----- | ------------------------------------------- | -------- |
| Admin | [admin@nzhub.test](mailto:admin@nzhub.test) | password |
| User  | [user@nzhub.test](mailto:user@nzhub.test)   | password |

---

## 💳 Alur Checkout (Flow)

1. User pilih produk
2. Tambah ke cart
3. Checkout
4. Pilih metode pembayaran
5. Admin verifikasi
6. Status → diproses → dikirim → selesai

---

## 🧪 Testing (Opsional)

```bash
php artisan test
```

---

## 🚀 Deployment (Shared Hosting / VPS)

Build assets:

```bash
npm run build
```

Cache config:

```bash
php artisan config:cache
php artisan route:cache
php artisan view:cache
```

Pastikan folder berikut writable:

```
storage/
bootstrap/cache
```

---

## 🛠️ Pengembangan Selanjutnya (Ideas)

* Integrasi payment gateway (Midtrans / Xendit)
* Wishlist
* Review & rating produk
* Coupon / voucher diskon
* REST API / mobile app support
* Role & permission (RBAC)

---

## 🤝 Kontribusi

Pull request sangat diterima. Untuk perubahan besar, silakan buka issue terlebih dahulu untuk diskusi.

---

## 📄 Lisensi

Open‑source untuk pembelajaran.
