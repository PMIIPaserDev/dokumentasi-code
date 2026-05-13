# 📘 Panduan Singkat Git (Versi Ringkas Pro Git)

Panduan ini berisi perintah-perintah esensial Git untuk membantu kamu memulai proyek dengan cepat di Linux maupun Windows.

---

## 1. Instalasi Git

### 🐧 Di Linux (Debian/Ubuntu)
Buka terminal dan ketik perintah berikut:
```bash
sudo apt update
sudo apt install git -y
```
###🪟 Di Windows
Unduh installer dari git-scm.com.
Jalankan .exe dan ikuti petunjuk instalasi.
Buka CMD atau PowerShell untuk mulai menggunakan Git.
Verifikasi instalasi (berlaku untuk semua OS):

```bash
git --version
```
2. Pengaturan Awal (First-Time Setup)
Identitas ini penting karena setiap commit di Git akan menggunakan informasi ini.
```bash
git config --global user.name "Nama Lengkap Anda"
git config --global user.email "emailanda@example.com"
 ``` 
3. Dasar-Dasar Git yang Sering Dipakai
Memulai Repositori
Membuat repo baru di folder saat ini:

```bash
git init
```
Menyalin repo yang sudah ada dari internet:

```bash
git clone [https://github.com/username/nama-repo.git](https://github.com/username/nama-repo.git)
```
Siklus Perubahan File
Cek status file:

```bash
git status
```
Menambah file ke Staging Area (siap simpan):

Bash
git add nama_file.html  # Satu file
git add .               # Semua file
Menyimpan perubahan secara permanen (Commit):

Bash
git commit -m "Catatan: Deskripsi perubahan Anda"
4. Bekerja dengan GitHub (Remote)
Menghubungkan folder lokal ke GitHub:

Bash
git remote add origin [https://github.com/username/nama-repo.git](https://github.com/username/nama-repo.git)
Mengirim kode ke GitHub:

Bash
git push -u origin main
Mengambil kode terbaru dari GitHub:

Bash
git pull origin main
5. Percabangan (Branching)
Branch digunakan agar kamu bisa bereksperimen tanpa merusak kode utama.

Buat branch baru: git checkout -b nama-fitur

Pindah ke branch lain: git checkout main

Menggabungkan fitur ke main:

Bash
git checkout main
git merge nama-fitur
6. Referensi Dokumentasi
Untuk pemahaman lebih dalam, kamu bisa merujuk ke:

Buku Resmi (Pro Git): git-scm.com/book/id/v2 (Tersedia dalam Bahasa Indonesia).

Bantuan Cepat: Ketik git help <perintah> di terminal kamu.
