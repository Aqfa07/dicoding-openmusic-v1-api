# OpenMusic API

OpenMusic adalah aplikasi pemutar musik open source yang menyediakan musik berlisensi gratis untuk semua orang.

## Fitur

- ✅ Manajemen Album (CRUD)
- ✅ Manajemen Lagu (CRUD)
- ✅ Validasi Data
- ✅ Error Handling
- ✅ Database PostgreSQL
- ✅ Migrations
- ✅ Pencarian Lagu (Query Parameter)
- ✅ Daftar Lagu dalam Album

## Instalasi

1. Clone repository
2. Install dependencies: `npm install`
3. Setup database PostgreSQL
4. Copy `.env.example` ke `.env` dan sesuaikan konfigurasi
5. Jalankan migrations: `npm run migrate:up`
6. Jalankan server: `npm start`

## API Endpoints

### Albums
- `POST /albums` - Menambahkan album
- `GET /albums/{id}` - Mendapatkan detail album
- `PUT /albums/{id}` - Mengubah album
- `DELETE /albums/{id}` - Menghapus album

### Songs
- `POST /songs` - Menambahkan lagu
- `GET /songs` - Mendapatkan semua lagu (dengan query parameter)
- `GET /songs/{id}` - Mendapatkan detail lagu
- `PUT /songs/{id}` - Mengubah lagu
- `DELETE /songs/{id}` - Menghapus lagu

## Environment Variables

\`\`\`
HOST=localhost
PORT=5000
PGUSER=postgres
PGPASSWORD=your_password
PGDATABASE=openmusic
PGHOST=localhost
PGPORT=5432
