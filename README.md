
# README: CRUD API Guna Prefix Juga Helper Kat Laravel

Dokumen Ni Menerangkan Langkah-langkah Cam Mana Nak Buat Fitur CRUD Tuk Tabel Categories Kat Laravel Guna Bearer Token Juga Helper Tuk Response JSON Dia

## **Struktur Folder Dengan File Penting Sekali**

```
├── app
│   ├── Http
│   │   └── Controllers
│   │       └── Api
│   │           └── CategoryController.php
│   ├── Helpers
│   │   └── ResponseHelper.php
│   ├── Models
│       └── Category.php
├── routes
│   └── api.php
└── composer.json
```

---

## **Langkah-Langkah Implementasi CRUD Guna Prefix Juga Helper**

### **1. Model: `Category.php`**
Pastikaan Sudah Buat Model Di `app/Models/Category.php.`

### **2. Controller: `CategoryController.php`**
Buat File Controller Di `app/Http/Controllers/Api/CategoryController.php`.

### **3. Helper: `ResponseHelper.php`**
Buat File Helper Di `app/Helpers/ResponseHelper.php`.

### **4. Route: `api.php`**
Tambahkan Route Untuk Kategori Di `routes/api.php`.

### **5. Composer Autoload**
Daftarkan Helper Di `composer.json` Bagian `autoload`.

Jalankan Perintah Berikut Untuk Memuat Ulang Autoload:

```bash
composer dump-autoload
```

---

## **Testing Dengan Insomnia**
- Contoh Endpoint:
   - `GET /api/categories` // Buat Mendapatkan Semua Kategori.
   - `POST /api/categories` // Untuk Membuat Kategori Baru.
   - `PUT /api/categories/{id}` // Untuk Memperbarui Kategori.
   - `DELETE /api/categories/{id}` // Untuk Menghapus Kategori.

---

## **Kesimpulan**
Dengan Menggunakan Helper `ResponseHelper`, Code Controller Jadi Lebih Bersih Dan Konsisten Dalam Format Response JSON. Sedang Middleware Bearer Token Memastikan Keamanan Endpoint API.

```css
Disusun oleh [Abuu Ubaadah a.k.a Muhammad Yaziid Ash-Shabriyy]
```
