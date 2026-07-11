# Migunani - Volunteer Marketplace

Migunani adalah prototipe aplikasi *marketplace event volunteer* (relawan) yang menjembatani antara mahasiswa, relawan umum, dan *organizer* (penyelenggara acara). 

Proyek ini dibangun menggunakan arsitektur **Decoupled / Headless**, di mana Frontend dan Backend sepenuhnya terpisah dan saling berkomunikasi melalui RESTful API.

## 🚀 Tech Stack (Teknologi yang Digunakan)

### Frontend
- **Framework:** React.js
- **Build Tool:** Vite
- **Bahasa:** TypeScript
- **Styling:** Tailwind CSS

### Backend
- **Framework:** Laravel (PHP)
- **Database:** SQLite (Default untuk *development* lokal)
- **Autentikasi:** Laravel Sanctum

---

## 🛠️ Cara Menjalankan Proyek Secara Lokal

Pastikan Anda sudah menginstal **PHP (v8+)**, **Composer**, dan **Node.js** di komputer Anda.

### 1. Setup Backend (API Server)
Buka terminal baru dan jalankan perintah berikut secara berurutan:
```bash
cd backend
composer install
cp .env.example .env
php artisan key:generate
php artisan migrate
php artisan serve
```

### 2. Setup Frontend (UI Web)
Buka terminal baru yang lain, lalu jalankan perintah berikut:
```bash
cd frontend
npm install
npm run dev
```
Frontend akan berjalan di https://wishmeluckteam-app-volunteer.vercel.app/. 

Silakan buka tautan frontend tersebut di browser Anda untuk mulai menjelajahi aplikasi Migunani!
