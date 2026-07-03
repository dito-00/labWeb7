<div align="center">

# 🌐 Sistem Portal Berita & RESTful API
**Integrasi CodeIgniter 4 dan Vue.js 3 (Single Page Application)**

Sebuah proyek evolusi web dari arsitektur monolitik tradisional menuju layanan berbasis API yang sepenuhnya dinamis dan reaktif. Proyek ini dikembangkan untuk memenuhi tugas Praktikum Pemrograman Web 2.

**💻 Dikembangkan Oleh:**
<br>
**Ryanda Juandito Jodi** (312410329) 
<br>
Kelas I241B • Pemrograman Web 2

---

</div>

## ⚡ Sorotan Fitur Utama

Proyek ini dibagi menjadi dua ekosistem utama yang saling berkomunikasi melalui protokol HTTP:

### 🛡️ Sistem Backend (CodeIgniter 4)
- **API Berbasis Resource:** Pengelolaan penuh (Create, Read, Update, Delete) untuk entitas artikel.
- **Relasi Cerdas:** Penggabungan tabel `artikel` dan `kategori` menggunakan *Query Builder* (JOIN).
- **Manajemen Berkas:** Fitur unggah gambar sampul artikel dinamis dengan validasi keamanan.
- **Skalabilitas Data:** Implementasi *Server-side Pagination* dan *Keyword Search*.
- **Keamanan Lapis Ganda:** *Session-based login* untuk *dashboard* monolitik, dan **Token-Based Authentication** khusus untuk memproteksi *endpoint* REST API.

### 🚀 Sistem Frontend (Vue.js 3)
- **Reaktivitas Instan:** Manipulasi data *real-time* via **Axios** tanpa perlu memuat ulang halaman (*Asynchronous CRUD*).
- **Navigasi Mulus:** Transisi antar halaman (Home, Artikel, About) yang super cepat berkat **Vue Router**.
- **Otorisasi Sisi Klien:** Implementasi **Route Guard** untuk mencegah akses ilegal ke halaman dasbor.
- **Interseptor Otomatis:** Penyematan *Bearer Token* secara otomatis pada *header* setiap *request* menggunakan Axios Interceptors.

---

## 💎 Tech Stack & Lingkungan Pengembangan

| Kategori | Teknologi / Pustaka |
| :--- | :--- |
| **Logika Backend** | PHP 8, CodeIgniter 4 |
| **Basis Data** | MySQL |
| **Antarmuka Frontend** | HTML5, CSS3, JavaScript (ES6), Vue.js 3 |
| **Manajemen State & Rute**| Vue Router 4 |
| **Komunikasi Jaringan** | Axios, jQuery AJAX, RESTful API (JSON) |
| **Alat Pengujian & IDE** | XAMPP, Visual Studio Code, Postman |

---

## 🛣️ Evolusi Proyek (Milestones)

> Perjalanan pengembangan aplikasi ini dibagi ke dalam 8 tahap praktikum utama:

1. **Fondasi Arsitektur:** Pembuatan struktur *Routing* MVC dan *Master Layout* (Header/Footer).
2. **Manajemen Database:** Integrasi ke MySQL dan aktivasi operasi dasar CRUD (*Create, Read, Update, Delete*).
3. **Komponen Modular:** Penerapan *View Cells* di CI4 untuk elemen UI yang bisa dipakai ulang (seperti *widget* daftar artikel terbaru).
4. **Sistem Autentikasi:** Pembuatan gerbang *Login*, enkripsi *password_hash*, dan proteksi rute dengan *Auth Filter*.
5. **Manipulasi Data Lanjutan:** Integrasi fitur *Pagination* (5 data/halaman), fitur pencarian, filter kategori, dan mekanisme unggah gambar.
6. **Transisi ke REST API:** Pergeseran dari *rendering* server ke pengiriman data mentah (JSON) via *ResourceController* dan AJAX.
7. **Pembangunan SPA (Vue.js):** Frontend direkonstruksi ulang menggunakan Vue.js dan Vue Router untuk pengalaman navigasi tanpa *loading*.
8. **Pengamanan API (Token Auth):** Finalisasi keamanan dengan menyimpan token di *Local Storage*, divalidasi oleh *Route Guard* (Frontend), dan diverifikasi oleh *API Auth Filter* CI4 (Backend).

---

## 📸 Dokumentasi Visual

<details>
<summary><b>1. Dasbor Admin (Arsitektur Monolitik)</b> <i>(Klik untuk melihat)</i></summary>
<br>

| Halaman Utama | Manajemen CRUD |
|---|---|
| <img width="800" src="https://github.com/user-attachments/assets/1f2ca80f-5c49-498f-b854-6fe0eb2985d2" alt="Home"> | <img width="800" src="https://github.com/user-attachments/assets/796303ae-42a7-4455-9213-9dc64870db52" alt="Admin Dashboard"> |

| Pencarian & Pagination | Filter Kategori |
|---|---|
| <img width="800" src="https://github.com/user-attachments/assets/8e557618-4f89-4d2a-b1df-fe189dade031" alt="Search"> | <img width="800" src="https://github.com/user-attachments/assets/aa15dc3c-a08c-4535-b08b-ed5fc4ed87f6" alt="Kategori"> |

</details>

<details>
<summary><b>2. Antarmuka SPA (Vue.js & Vue Router)</b> <i>(Klik untuk melihat)</i></summary>
<br>

<img width="800" src="https://github.com/user-attachments/assets/9bc9a972-ca00-49eb-ab48-dde6f9f52825" alt="Home Vue">
<br><br>
<img width="800" src="https://github.com/user-attachments/assets/577481fc-3027-4ecc-ad3b-73b5bf5f9279" alt="Artikel Vue">
<br><br>

</details>

<details>
<summary><b>3. Autentikasi, Interseptor Token & Postman</b> <i>(Klik untuk melihat)</i></summary>
<br>

| Autentikasi Pengguna | Jaringan & Interseptor Token |
|---|---|
| <img width="800" src="https://github.com/user-attachments/assets/7b115b59-4f04-4f42-9bd4-c628ca48d133" alt="Login"> | <img width="800" src="https://github.com/user-attachments/assets/e314c38b-6311-40e1-acbe-4e16617078b2" alt="Interceptors"> |

| Pengujian API (GET) | Pengujian API (POST) |
|---|---|
| <img width="800" src="https://github.com/user-attachments/assets/f1e89673-3250-4054-8513-3049e9f29543" alt="GET"> | <img width="800" src="https://github.com/user-attachments/assets/925940ce-271b-417d-a441-cfa1c6f14adc" alt="POST"> |

</details>
