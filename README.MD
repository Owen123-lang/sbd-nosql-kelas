# Aplikasi Web Gacha FGO (Fate/Grand Order)

Aplikasi web gacha berbasis MERN stack (MongoDB, Express.js, React.js, Node.js) yang terinspirasi dari game Fate/Grand Order.

## Deskripsi

Aplikasi ini merupakan simulasi sistem gacha dengan tema Fate/Grand Order, dimana pengguna dapat melakukan:
- Registrasi dan login akun
- Melakukan gacha untuk mendapatkan karakter
- Melihat karakter yang telah didapatkan
- Menggunakan sistem pity untuk menjamin mendapatkan karakter rare

## Teknologi yang Digunakan

### Frontend
- React.js
- Tailwind CSS untuk styling
- Context API untuk state management
- Vite sebagai build tool

### Backend
- Node.js dengan Express.js
- MongoDB sebagai database
- Docker untuk containerization

## Fitur Utama

### 1. Sistem Autentikasi
- Registrasi akun baru
- Login dengan akun yang sudah terdaftar
- Proteksi route untuk pengguna yang belum login

### 2. Sistem Gacha
- Simulasi gacha dengan berbagai tingkat kelangkaan karakter
- Sistem pity yang menjamin karakter rare setelah sejumlah pull
- Visualisasi animasi saat melakukan gacha

### 3. Koleksi Karakter
- Tampilan kartu karakter yang telah didapatkan
- Informasi detail setiap karakter
- History gacha yang telah dilakukan

## Cara Menjalankan Aplikasi

### Prasyarat
- Node.js dan npm terinstall
- Docker dan Docker Compose terinstall
- MongoDB (jika ingin menjalankan tanpa Docker)

### Langkah-langkah Menjalankan dengan Docker

1. Clone repository ini
2. Buka terminal dan masuk ke direktori project
3. Jalankan perintah:
```bash
docker-compose up --build
```
4. Aplikasi dapat diakses di:
   - Frontend: http://localhost:5173
   - Backend: http://localhost:3000

### Langkah-langkah Menjalankan Tanpa Docker

1. Clone repository ini
2. Buka terminal dan masuk ke direktori project

3. Setup Backend:
```bash
cd Backend
npm install
npm run dev
```

4. Setup Frontend (buka terminal baru):
```bash
cd Frontend
npm install
npm run dev
```

5. Aplikasi dapat diakses di:
   - Frontend: http://localhost:5173
   - Backend: http://localhost:3000

## Struktur Project

### Frontend
- `/src/pages`: Halaman-halaman utama aplikasi
  - `Login.jsx`: Halaman login
  - `Register.jsx`: Halaman registrasi
  - `Gacha.jsx`: Halaman untuk melakukan gacha
  - `Card.jsx`: Halaman untuk melihat koleksi karakter
- `/src/context`: Context untuk state management
- `/src/assets`: Aset gambar dan media lainnya

### Backend
- `/controllers`: Logic untuk handling request
- `/models`: Schema database MongoDB
- `index.js`: Entry point aplikasi backend



