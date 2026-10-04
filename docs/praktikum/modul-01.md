# Dokumen Teknis Modul 1 — Lingkungan Pengembangan, Git, dan Lalu Lintas HTTP

Nama/NIM : Neila Faaizah Asynur  
Repositori : [https://github.com/neilaasynur/modul1-105224028-Pemweb.git](https://github.com/neilaasynur/modul1-105224028-Pemweb.git)

## 1. Lingkungan Pengembangan
Berikut saya paparkan tabel versi sistem operasi yang saya gunakan, mulai dari Node.js, npm, Git, hingga Visual Studio Code.

| Perangkat | Versi | 
|-------|------|
| OS | Windows 11 |
| Node.js | v24.21.0 | 
| npm  | 11.19.0 |
| Git | 2.55.0.windows.5 |
| VS Code | 1.131.0 |

## 2. Alur Kerja Git
1. Keluaran git log --oneline --graph   
b734e4a (HEAD -> main, origin/main, origin/HEAD) menyiapkan dokumen teknis praktikum pemweb modul 1
4b11502 commit baru
557bc0f first commit

2. Tautan pull request yang telah digabungkan   
[tautan pull request yang telah di merge](https://github.com/neilaasynur/modul1-105224028-Pemweb/pull/1)

3. Konflik yang terjadi, cara penyelesaian, dan alasan pemilihan isi akhir   
Ketika melakukan pull request ini, tidak terjadi konflik sama sekali. Berbeda ketika saya melakukan merge dari branch "latihan/konflik" ke main di lokal. Ketika ingin merge branch tersebut, ada konflik karena adanya perbedaan isi pada file yang sama. Cara penyelesaian yang sama ambil adalah dengan memilih salah satu dari kedua branch, dan saya memilih isi file pada branch main. Hal ini saya ambil karena isi pada file main adalah revisi terakhir yang saya lakukan, sehingga saya merasa hal itu adalah yang terbaik.
![Gambar konflik]("D:\Kuliah\Semester 5\Praktikum PemWeb\Modul 1\docs\praktikum\konflik ketika merge (lokal).png")

## 3. Pengamatan Lalu Lintas HTTP
| No | URL | Metode | Kode Status | Content-Type | Header Lain yang Diamati|  
|-------|------|-------|------|-------|------|
| 1 | http://localhost:3000 | GET | 200 OK | text/html; charset=utf-8 | cache-control: no-cache, must-revalidate|
| 2 | http://localhost:3000/ halaman-tidak-ada| GET | 404 not found | text/html; charset=utf-8 | cache-control: no-cache, must-revalidate|  
| 3 | Satu berkas CSS atau JS dari localhost: http://localhost:3000/_next/static/chunks/%5Broot-of-the-server%5D__0cbk-n2._.css| GET | 200 OK | text/css; charset=UTF-8 | cache-control: no-cache, must-revalidate|  
| 4 | http://github.com (curl) | HEAD | 301 Moved Permanently |  | Location: https://github.com/|  
| 5 | https:// developer.mozilla.org (dengan cache) | GET | 302 Found | text/html; charset=utf-8 | location/en-US/|  
## 4. Kendala dan Penyelesaian
Selama pengerjaan tahapan dari modul, saya mengalami kendala bagaimana cara untuk memulai. Tetapi ketika saya mengikuti petunjuk yang telah diberikan di dalam modul, saya paham bagaimana alur pengerjaan, bagaimana pengecekan version tools, alur kerja git, serta pengamatan lalu lintas HTTP sesuai yang dipandu oleh modul. 
## 5. Catatan Pemanfaatan AI
Tidak menggunakan AI