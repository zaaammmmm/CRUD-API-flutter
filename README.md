# CRUD API Flutter - Aplikasi Manajemen Mahasiswa

## 📱 Deskripsi Proyek
Aplikasi Flutter multi-platform untuk melakukan operasi **CRUD** (Create, Read, Update, Delete) pada data mahasiswa. Aplikasi ini terhubung dengan backend PHP API lokal untuk mengelola data mahasiswa (nama, NIM, prodi).

### Fitur Utama
- ✅ **Create**: Tambah data mahasiswa baru
- ✅ **Read**: Tampilkan daftar semua mahasiswa
- ✅ **Update**: Edit data mahasiswa
- ✅ **Delete**: Hapus data mahasiswa
- 📱 Support multi-platform: Android, iOS, Web, Desktop (Windows, macOS, Linux)
- 🔄 Real-time sync dengan backend API

## 🛠️ Tech Stack
- **Frontend**: Flutter (Dart)
- **HTTP Client**: `http: ^0.13.6`
- **Backend**: PHP API (`http://127.0.0.1/api_mahasiswa/index.php`)
- **Model**: `Mahasiswa` (id, nama, nim, prodi)

## 📋 Prasyarat
1. **Flutter SDK** ≥ 3.10.7 (lihat [flutter.dev](https://flutter.dev))
2. **Backend PHP API** berjalan di `http://127.0.0.1/api_mahasiswa/index.php`
3. **Dart SDK** (termasuk dalam Flutter)

## 🚀 Cara Menjalankan

### 1. Clone / Download Proyek
```bash
git clone <repo-url>
cd CRUD-API-flutter
```

### 2. Install Dependencies
```bash
flutter pub get
```

### 3. Jalankan Backend API
Pastikan server PHP Anda berjalan dengan endpoint:
```
http://127.0.0.1/api_mahasiswa/index.php
```
- Method: GET (read), POST (create), PUT (update), DELETE (delete)
- Format data: JSON

### 4. Jalankan Aplikasi
```bash
# Android / iOS / Desktop
flutter run

# Web
flutter run -d chrome
```

## 🏗️ Struktur Kode
```
lib/
├── main.dart              # Entry point & UI (HomePage)
├── mahasiswa.dart         # Model Mahasiswa
└── mahasiswa_service.dart # API Service (CRUD operations)
```

### Model Mahasiswa
```dart
class Mahasiswa {
  final int? id;
  final String nama;
  final String nim;
  final String prodi;
}
```

### API Endpoints
| Method | Endpoint | Deskripsi |
|--------|----------|-----------|
| GET | `http://127.0.0.1/api_mahasiswa/index.php` | Ambil semua data |
| POST | `http://127.0.0.1/api_mahasiswa/index.php` | Tambah data |
| PUT | `http://127.0.0.1/api_mahasiswa/index.php` | Update data |
| DELETE | `http://127.0.0.1/api_mahasiswa/index.php?id=X` | Hapus data |

## 📸 Screenshot
*(Aplikasi menampilkan form input dan list mahasiswa dengan tombol edit/delete)*

## 🔧 Kontribusi
1. Fork repository
2. Buat feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add some AmazingFeature'`)
4. Push ke branch (`git push origin feature/AmazingFeature`)
5. Open Pull Request

## 📄 Lisensi
Project ini dilisensikan di bawah [LICENSE](LICENSE).

## 🙏 Terima Kasih
Terima kasih telah menggunakan CRUD API Flutter!

---
**Made with ❤️ using Flutter**

