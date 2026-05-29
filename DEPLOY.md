# Cara Deploy ERP Kost / Kontrakan

File sudah siap dipublikasikan sebagai situs statis. Jika kamu ingin membuat link yang bisa diakses publik, ikuti salah satu cara di bawah.

## 1. Deploy ke Netlify (paling cepat)

1. Buka https://app.netlify.com/
2. Daftar atau login.
3. Pilih "Add new site" > "Deploy manually".
4. Pilih file `index.html` atau drag-and-drop seluruh folder `programming for business`.
5. Tunggu hingga proses selesai.
6. Netlify akan memberikan URL publik seperti `https://nama-proyek.netlify.app`.

## 2. Deploy ke GitHub Pages

### Opsi A — Upload manual lewat GitHub web
1. Login ke GitHub.
2. Buat repository baru (misalnya `erp-kost-kontrakan`).
3. Di halaman repository, klik "Add file" > "Upload files".
4. Upload file `index.html`, `finalproject.html`, `README.md`, dan `DEPLOY.md`.
5. Klik "Commit changes".
6. Buka tab `Settings` repository > `Pages`.
7. Di bagian "Source", pilih branch `main` dan folder `/ (root)`, lalu klik "Save".
8. GitHub Pages akan membuat situs dalam beberapa detik.
9. URL akan muncul di bagian atas, biasanya `https://username.github.io/erp-kost-kontrakan`.

### Opsi B — Deploy lewat Git (kalau sudah terpasang)
1. Install Git di komputer kamu jika belum ada: https://git-scm.com/downloads.
2. Buka terminal di folder `programming for business`.
3. Jalankan perintah:
   ```bash
   git init
   git add index.html finalproject.html README.md DEPLOY.md
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/USERNAME/erp-kost-kontrakan.git
   git push -u origin main
   ```
4. Ganti `USERNAME` dengan nama akun GitHub kamu.
5. Setelah push selesai, buka repository GitHub kamu.
6. Masuk ke `Settings` > `Pages`.
7. Pilih source branch `main` dan folder `/`, lalu klik "Save".
8. GitHub Pages akan menampilkan URL publik.

### Catatan
- Pastikan file `index.html` berada di root repository.
- Jika branch default kamu bukan `main`, pilih branch yang sesuai di pengaturan Pages.
- Setelah melakukan perubahan pada file, commit dan push lagi untuk memperbarui situs.

## 3. Deploy ke Vercel

1. Buka https://vercel.com/
2. Daftar atau login.
3. Pilih "New Project" > "Import" atau drag-and-drop folder.
4. Pilih opsi "Static Site" jika diminta.
5. Setelah deploy selesai, Vercel akan memberikan URL publik.

## Catatan penting

- Gunakan `index.html` sebagai halaman utama.
- Jika kamu upload folder, pastikan `index.html` berada di root folder.
- Setelah deploy, salin URL publik dari layanan hosting dan bagikan ke orang lain.

## Saya bisa bantu lagi

Jika kamu ingin, saya bisa membantu langkah demi langkah untuk:

- menyiapkan akun GitHub dan membuat repository,
- mengunggah file ke GitHub Pages,
- atau membuat deploy manual di Netlify.
