# 🎧 OpenMusic API V1

**OpenMusic** adalah aplikasi pemutar musik open source yang menyediakan musik berlisensi gratis untuk semua orang.  
Dirancang untuk praktik backend development menggunakan **Node.js**, **Hapi.js**, dan **PostgreSQL**.

---

## ✨ Fitur Utama

- ✅ **Manajemen Album** (CRUD)
- ✅ **Manajemen Lagu** (CRUD)
- ✅ **Validasi Data** dengan Joi
- ✅ **Error Handling** yang konsisten
- ✅ **Database PostgreSQL** dengan migrasi skema
- ✅ **Pencarian Lagu** dengan query parameter
- ✅ **Daftar Lagu dalam Album**

---

## ⚙️ Instalasi

1. **Clone repository**
2. Install dependensi:
    ```bash
    npm install
    ```
3. Siapkan database PostgreSQL
4. Salin `.env.example` ke `.env`, lalu sesuaikan konfigurasi
5. Jalankan migrasi database:
    ```bash
    npm run migrate:up
    ```
6. Jalankan server:
    ```bash
    npm start
    ```

---

## 📡 API Endpoints

### 🎼 Albums
- `POST /albums` - Tambah album baru
- `GET /albums/{id}` - Lihat detail album + lagu-lagu di dalamnya
- `PUT /albums/{id}` - Edit album
- `DELETE /albums/{id}` - Hapus album

### 🎵 Songs
- `POST /songs` - Tambah lagu baru
- `GET /songs` - Lihat semua lagu (`?title=` dan `?performer=` untuk filter)
- `GET /songs/{id}` - Lihat detail lagu
- `PUT /songs/{id}` - Edit lagu
- `DELETE /songs/{id}` - Hapus lagu

---

## 🔐 Environment Variables

```
HOST=localhost
PORT=5000
PGUSER=postgres
PGPASSWORD=your_password
PGDATABASE=openmusic
PGHOST=localhost
PGPORT=5432
```

---

## 📄 Lisensi

Dibuat sebagai bagian dari **belajar back-end development** di platform **Dicoding Indonesia**.
