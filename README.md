# 💍 Undangan Pernikahan Digital Premium (Free & Open Source)

Template undangan pernikahan digital berbasis web yang elegan, responsif (mobile-first), dan sepenuhnya gratis. Dibuat menggunakan HTML dasar, **Tailwind CSS** (untuk *styling*), dan Vanilla JavaScript. 

Template ini dirancang agar **sangat mudah diedit oleh siapa saja**, bahkan bagi yang tidak memiliki *background* IT, langsung dari browser menggunakan **GitHub Codespaces** dan di-online-kan secara gratis melalui **Vercel**.

![Preview Undangan](https://img.shields.io/badge/Status-Siap_Pakai-success?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)

## ✨ Fitur Unggulan
- **Nama Tamu Dinamis:** Nama tamu dapat diubah otomatis hanya dengan memodifikasi link URL (menggunakan parameter `?to=NamaTamu`).
- **Splash Screen:** Animasi pembuka (hati pink berdetak) sebelum masuk ke sampul undangan.
- **Sampul Elegan:** Desain sampul dengan bingkai emas ukiran (vintage frame) yang menutupi foto mempelai.
- **Musik Otomatis:** Latar musik romantis yang dapat di-play/pause melalui tombol melayang.
- **Galeri Foto:** Grid galeri untuk menampilkan momen *Pre-Wedding*.
- **Integrasi Maps:** Embed peta Google Maps langsung di dalam undangan.
- **100% Responsif:** Tampilan akan tetap menyesuaikan ukuran layar HP meskipun dibuka melalui Laptop/PC.

---

## 🛠️ Cara Penggunaan (Panduan Lengkap)

Ikuti langkah-langkah di bawah ini untuk membuat undangan Anda sendiri dalam waktu kurang dari 15 menit.

### Langkah 1: Fork Repository Ini
Agar Anda memiliki salinan kode ini di akun GitHub Anda sendiri:
1. Pastikan Anda sudah login ke akun **GitHub**.
2. Klik tombol **Fork** di pojok kanan atas halaman repository ini.
3. Klik **Create Fork**. Sekarang kode ini sudah menjadi milik Anda.

### Langkah 2: Edit Menggunakan GitHub Codespaces
Anda tidak perlu menginstal aplikasi apapun di laptop. Kita akan mengeditnya langsung di browser!
1. Di repository hasil fork Anda, klik tombol hijau **<> Code**.
2. Pilih tab **Codespaces**, lalu klik **Create codespace on main**.
3. Tunggu beberapa saat hingga editor kode (VS Code versi web) terbuka.
4. Di panel sebelah kiri, Anda akan melihat folder `image` dan file `index.html`.

### Langkah 3: Cara Melihat Pratinjau (Preview) Langsung
Agar Anda bisa melihat hasil editan secara *real-time*:
1. Di menu paling kiri Codespaces, klik ikon **Extensions** (ikon 4 kotak).
2. Cari dan install ekstensi bernama **Live Server** (oleh Ritwick Dey).
3. Buka file `index.html`.
4. Di pojok kanan bawah, klik tombol **Go Live** (atau klik kanan pada kode dan pilih *Open with Live Server*).
5. Tab browser baru akan terbuka. Setiap kali Anda menekan `Ctrl + S` (Save), tampilan di tab tersebut akan otomatis berubah!

### Langkah 4: Sesuaikan dengan Data Anda
Di Codespaces, Anda perlu mengganti beberapa hal:

**A. Mengganti Gambar & Musik**
Siapkan file Anda dan masukkan (Drag & Drop) ke dalam folder `image`:
1. `foto.jpg` : Foto utama untuk sampul depan.
2. `bingkai-asli.png` : Gambar bingkai ukiran emas. *(PENTING: Pastikan background bingkai Anda benar-benar transparan. Gunakan web gratis seperti [remove.bg](https://www.remove.bg/) untuk menghapus background kotak-kotak palsu).*
3. `lagu.mp3` : Musik latar romantis Anda.

**B. Mengedit Teks (`index.html`)**
Buka `index.html` dan ubah teks seperti:
- Nama Mempelai ("Nina & Rizki")
- Tanggal & Waktu Acara
- Nama Orang Tua
- Lokasi Gedung & Link Google Maps iframe.

### Langkah 5: Simpan & Kirim ke GitHub (Commit & Push)
Jika editan sudah dirasa pas di *Live Server*:
1. Klik ikon **Source Control** di menu sebelah kiri (ikon bercabang).
2. Di kolom teks (Message), tulis pesan (Contoh: *"Update data undangan saya"*).
3. Klik tombol biru **Commit**, (pilih *Yes/Always* jika muncul peringatan).
4. Terakhir, klik tombol **Sync Changes** untuk mengirim editan Anda ke GitHub.

---

## 🚀 Langkah 6: Online-kan Web Menggunakan Vercel
Agar link undangan Anda bisa disebar ke tamu:
1. Kunjungi [Vercel.com](https://vercel.com/) dan buat akun/login menggunakan akun **GitHub** Anda.
2. Di Dashboard Vercel, klik tombol **Add New...** -> pilih **Project**.
3. Vercel akan membaca repository GitHub Anda. Cari nama repository undangan ini, lalu klik **Import**.
4. Biarkan pengaturan default, langsung scroll ke bawah dan klik **Deploy**.
5. Tunggu 30 detik hingga muncul kembang api 🎉. 
6. Web Anda sudah online! Klik **Continue to Dashboard** untuk melihat Link / Domain Anda (contoh: `https://undangan-nikah-ku.vercel.app`).

---

## 💌 Cara Membuat Link Khusus Nama Tamu
Untuk memunculkan nama tamu yang berbeda-beda, Anda cukup menambahkan parameter `?to=` di akhir link Vercel Anda.

**Format:**
`https://[link-vercel-anda].vercel.app/?to=[Nama Tamu]`

**Contoh:**
- Jika nama tamunya "Budi", linknya: `https://.../?to=Budi`
- Jika namanya "Bapak Andi & Keluarga", gunakan spasi biasa (saat di-copy biasanya spasi otomatis berubah menjadi `%20`): 
  `https://.../?to=Bapak Andi & Keluarga`

Nama "Tamu Spesial" di dalam kotak undangan akan otomatis berubah sesuai dengan nama yang ada di link URL!

---

### Catatan Tambahan (Tips Kustomisasi Bingkai)
Jika foto Anda tidak pas dengan lubang bingkai, Anda bisa menyesuaikan kode CSS pada `index.html`:
- Untuk membesarkan/mengecilkan **Bingkai**: Gunakan class `scale-...` (Contoh: `scale-110`, `scale-125`).
- Untuk membesarkan/mengecilkan **Foto**: Gunakan class presisi seperti `w-[150px] h-[200px]`.

---

**Dibuat dengan ❤️ untuk membantu momen bahagiamu.**
*Silakan Star (⭐) repository ini jika dirasa bermanfaat!*