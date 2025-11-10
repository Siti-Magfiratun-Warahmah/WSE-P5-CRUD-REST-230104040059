# Laporan Praktikum P5: Membangun RESTful CRUD

Repositori ini berisi hasil dari Praktikum ke-5 mata kuliah **Web Service Engineering**. Proyek ini berfokus pada implementasi API RESTful sederhana untuk operasi CRUD (Create, Read, Update, Delete) menggunakan Node.js dan Express.js.

## 👤 Identitas Mahasiswa

* **Nama** : SITI MAGFIRATUN WARAHMAH
* **NIM** : 230104040059
* **Kelas** : TI23B
* **Dosen** : Muhayat, M.IT

## 📝 Deskripsi Proyek

Proyek ini adalah sebuah server API sederhana yang dibuat dengan Express.js untuk mengelola data produk. API ini mengikuti prinsip RESTful dan menggunakan metode HTTP (GET, POST, PUT, DELETE) yang sesuai dengan operasinya.

Data produk untuk sementara disimpan dalam sebuah *array* di dalam file `src/data/products.data.js` (belum menggunakan database).

## 🛠️ Teknologi yang Digunakan

* Node.js (v18+)
* Express.js
* Nodemon (sebagai dev dependency)
* Postman / Thunder Client (untuk pengujian API)

## 🗺️ Tabel Endpoint API

Server berjalan pada `http://localhost:3000`. Berikut adalah daftar endpoint yang telah diimplementasikan:

| Method | Endpoint | Deskripsi | Status Sukses | Status Gagal/Error |
| :--- | :--- | :--- | :--- | :--- |
| **GET** | `/api/products` | Mengambil semua data produk. | `200 OK` | - |
| **GET** | `/api/products/:id` | Mengambil data produk spesifik berdasarkan ID. | `200 OK` | `404 Not Found` |
| **POST** | `/api/products` | Menambah data produk baru. | `201 Created` | - |
| **PUT** | `/api/products/:id` | Memperbarui data produk berdasarkan ID. | `200 OK` | `404 Not Found` |
| **DELETE** | `/api/products/:id` | Menghapus data produk berdasarkan ID. | `200 OK` | `404 Not Found` |

## 🚀 Cara Menjalankan Proyek

1.  **Clone repositori ini:**
    ```bash
    git clone [URL_REPOSITORI_ANDA]
    cd praktikum5_restful_crud
    ```

2.  **Instal dependencies:**
    ```bash
    npm install express
    ```
    *Catatan: Instal juga `nodemon` sebagai dev dependency:*
    ```bash
    npm install nodemon --save-dev
    ```

3.  **Jalankan server (mode development):**
    ```bash
    npm run dev
    ```

4.  **Uji Endpoint:**
    Gunakan Postman atau Thunder Client untuk menguji endpoint yang ada di tabel di atas.
