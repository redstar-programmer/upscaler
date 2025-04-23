# Redstar Upscaler
Video Upscaling Video Kuat FFMPEG, Real-Esrgan, Flowframes-NOW mendukung ** UI multi-bahasa **!

🌐 Bahasa:
[Bahasa Inggris] (readme.en.md) | [Korea] (readme.md) | [日本語] (readme.ja.md) | [中文] (readme.zh.md) |
[Français] (readme.fr.md) | [Deutsch] (readme.de.md) | [Español] (readme.es.md) | [Português] (readme.pt.md) |
[Рский] (readme.ru.md) | [Italiano] (readme.it.md) | [Tiếng việt] (readme.vi.md) | [Bahasa Indonesia] (Readme.id.md) |
[ภ ไทย] (readme.th.md) | [ال] (readme.ar.md)

<p align = "center">
  <Img src = "https://github.com/user-attachments/assets/632c3a83-5416-8d38-0e153b633" height = "/"/>
</p>

<p align = "center">
  <strong> ffmpeg, realesrgan, alur frames -based video upscaling tool </strong> <br>
  <em> basis GUI terbaru, pengaturan prasetis, beberapa dukungan pemrosesan file </em>
</p>

---

Unduh: [rilis]

## ✨ Sponsor The Redstar 'Upscaler

Apakah Anda ingin menyukai proyek ini atau pengembangan dukungan?  
Bantu fitur yang lebih baik dan pembaruan yang stabil dengan sponsor kecil!

-<img src = "https://img.shields.io/badge/donate-paypal-blue.svg?logo=paypal" height = "20"/> <br> ** paypal **: )  
-<img src = "https://img.shields.io/badge/sponsor-gigub20sponsors-f69b4?logo=githubsponsors" height = "20"/> <br> ** sponsor github **: [https://github.com/spons/sponsar ** **: [https://github.com/spons/sponsar


> 💡 Biaya server, waktu pengembangan, dan secangkir kopi adalah kekuatan besar. Terima kasih!

## Daftar isi

- [👋 PENDAHULUAN] (#Troduction)  
-[💾 Instalasi dan Persiapan] (#Instalasi dan Persiapan)  
- [🔧 Fungsi Utama] (#Fungsi Utama)  
-[🚀 Cara menggunakan (start cepat)] (#use-quick-start)  
-[⚙️ Detail Deskripsi] (#detail-fungsi-deskripsi)  
- [🙏 Terima kasih] (#terima kasih ditulis)  
- [📜 Sejarah] (#History)

## 👋 PENDAHULUAN
** Redstar Upscaler ** adalah alat GUI berbasis Python yang secara otomatis meningkatkan video ke resolusi tinggi menggunakan `ffmpeg`, 'real-esrgan', dan 'flowframe'. 

-Ekstraksi bingkai video → peningkatan → kombinasi video sekaligus
-Mengsek
-Opsional melalui flowframe
-Audio codec ekstraksi dan pemrosesan otomatis
-Apakah pekerjaan di lokasi asli atau jalur yang ditunjuk

> ⚠️ dikembangkan dan diuji di lingkungan Windows.

Di bawah ini terhubung ke YouTube dengan mengklik layar penggunaan sederhana. <br>
[! [Lihat video demonstrasi] (https://img.youtube.com/vi/g-jtwrws3co/0.jpg)] (https://youtu.be/g-jtwrws3co "

## 💾 Instalasi dan Persiapan

1. Instalasi alat eksternal berikut dan konfirmasi lokasi (namun, file distribusi berisi file instalasi FFMPEG, Real-Esrgan dan FlowFrame (lihat program di jalur))
   - [ffmpeg] (https://www.ffmpe.org/download.html)
   -[Real-esrgan] (https://github.com/xinntao/real-esrgan
   - [flowframes] (https://github.com/n00mkrad/flowframes) *(pilih) *
2. Jalankan readstar's upscaler.exe setelah unzip
3. Dalam kasus flowframe, model yang dimuat sesuai dengan lingkungan pengguna mungkin berbeda, jadi pastikan untuk menjalankan flowframe dan kemudian <br> interpolasi AI dan AI Model Redstar Upscaler Resources/flowframes_models.ini harus cocok. <br> Model yang tidak diturunkan tercatat dikomentari melalui tampilan #, dan pastikan untuk memeriksa apakah urutan model jendela pengaturan Redstar Upscaler dicocokkan dengan urutan model flowframe <br>.

## 🔧 fungsi utama

Lai [Image] (https://github.com/user-attachments/assets/93dc232e-8742-4ae3-935-9395c26a61f4)
-Video pilihan ganda dan pekerjaan berurutan
-Demehkan video drag/drop
-✅ apakah akan menjalankan program utama dan memilih seleksi langsung
-Kisk mode hemat
-Mukal -Multilingal (15 bahasa)
<br> <br>
Lai [Gambar] (https://github.com/user-attachments/assets/3341f4ca-af20-4647-93d0-4841466757)
-Selver aplikasi preset dan otomatis
-Deteksi otomatis codec audio dan pengaturan setrate
-Deteksi otomatis dan pemilihan model realesrgan
-Ffmpeg, real-esrgan, detail flowframe
Pengaturan opsi -Dange sesuai dengan versi flowframes <br>
<br> <br>
Lai [Gambar] (https://github.com/user-attachments/assets/25d60d82-53a2-4064-bbef-d439d3d6)
Konfirmasi Pesanan Eksekusi Upscale (dapat disalin dan dieksekusi secara terpisah dari CMD)
<br> <br>
Lai [Image] (https://github.com/user-attachments/assets/2fd69862-d038-401d-a9a6-83dc8c769f0)
-Monitor Kemajuan keseluruhan pekerjaan kelas atas
Konfirmasi logging -upscale (file log dibuat sebagai tanggal di folder log di folder nyata)
-Rusementa hasil otomatis setelah selesainya pekerjaan ([Redstar] awalan)
-Setting operasi setelah selesai <br>
<br> <br>
## 🚀 Cara menggunakan (Mulai Cepat)

1. Tambahkan file video (MP4, MKV, AVI, MOV, FLV, WMV, MPG, Webm, 3GP, OGV)
2. Periksa lokasi kerja atau periksa "Gunakan jalur file asli"
3. Klik tombol "Pengaturan" di video yang ditambahkan
4. FFMPEG, Realesrgan, Detail Flowframe
5. Klik diterapkan hanya untuk seluruh file / pilih file
4. Klik tombol Konfirmasi Tugas
7. Klik tombol Mulai setelah memeriksa perintah untuk dijalankan

> ✨ Hasil kerja dibuat di folder yang dipilih oleh dua gambar yang ditingkatkan dan dua frame file video interpolasi.
> ✨ File yang diselesaikan disimpan sebagai nama file dengan awalan [Redstar].
---

## ⚙️ Detail Deskripsi

| Item | Deskripsi |
| ------ | ------ |
| ** Pengaturan jalur tugas ** | Berikan jalur default atau opsi "Gunakan jalur file asli" |
| ** Dukungan Format Video ** | MP4, MKV, AVI, MOV, FLV, WMV, MPG, Webm, 3GP, OGV, dll.
| ** Model kelas atas ** | Realesr-animevideov3, Realesr-General, 4Xplus, dll.
| ** Pemrosesan Audio ** | Berbagai dukungan pengkodean format seperti 'AAC', 'mp3', dan 'FLAC' |
| ** Flowframe Terkait ** | Atur interpolasi (FPS × 2, × 4, × 8) |
| ** Mode Penghematan Disk ** | Fungsi Penghapusan Otomatis Gambar Menengah Disediakan |

## 🙏 Thanksgiving

-Realsrgan oleh [xinntao] (https://github.com/xinntao/real-esrgan)
-Flowframes oleh [n00mkrad] (https://github.com/n00mkrad/flowframes)
-Jika Anda ingin berpartisipasi dalam proyek ini atau menyarankan fungsi, silakan tinggalkan pendapat tentang [masalah] (https://github.com/redstar-javscraper/rredstar_upscaler/issues).

# 📜 Sejarah

V 1.1.0
 >. Konfigurasi Menu (File Buka, Tutup, Pengaturan Log, Pengaturan Bahasa)
 > 2. Tambahkan beberapa pengaturan bahasa (Bahasa yang tersedia: Korea, Inggris, 日本語, 中文, Français, Deutsch, Español, Português, ркий, tiếng việt, Bahasa Indonesia ال)
 3. Pesan dan beberapa perubahan kode sesuai dengan penambahan pengaturan bahasa
 > 4. Perubahan beberapa konfigurasi UI
 >. FFMPEG, Real-Esrgan, Flowframe Setiap Informasi Versi (Layar Utama)
 > 6. FlowFrames 1.41.0 Respons (Versi saat ini 1.41.0 memiliki masalah perintah CMD, jadi hanya 1.40.0 dan 1.36.0 yang dapat digunakan)
 > Selesaikan masalah di mana item model AI ditampilkan sebagai huruf kecil
 8. Opsi FFMPEG (piksel, codec video)
 > 9. Penguatan Cek Cuda untuk PC Pengguna -Dapat digunakan dan periksa jenis GPU (Layar Utama)

V 1.0.0
 >.
 >. UI perubahan
 > 3. Peningkatan rentang video/audio yang dapat diproses
 > 4. Tambahkan mode hemat disk
 > Distribusi termasuk program utama

V 0.1.92
 >. Flowframe masalah kegagalan interpolasi dengan duplikat input di kotak kombo model AI saat mengubah jalur
 > 2. Tambahkan status pemilihan kotak kombo untuk pekerjaan interpolasi

V 0.1.91
 >.
 > 2. Penyesuaian file distribusi

V 0.1.9
 >. Aplikasi Perubahan Model Flowframes
 >. Flowframes 1.36.0 Model baru, implementasi model 1.40.0
 3. Tidak ada lagi kegagalan perintah flowframes terjadi lagi
 > 4. Anda dapat menambahkan file dengan drag/drop
 > Menyelesaikan masalah yang tidak diterapkan

V 0.1.8
 >.
 2. Jika flowframe diinstal di jalur default (mis. C: \ Users \ Administrator
 3. Saat menambahkan beberapa file 
 > 4. Setelah menambahkan beberapa file,

V 0.1.7
 >. Perubahan Ukuran Program
 2. Selesaikan masalah kesalahan saat bekerja dengan file tanpa suara
 > 3. Ubah seluruh konfigurasi UI (kembali dikonfigurasi agar sesuai dengan perubahan ukuran)

V 0.1.6
 >.
 >. Selesaikan masalah bahwa informasi versi tidak dilihat sebagai versi baru dalam judul program.
 > Selesaikan masalah di mana file config.ini disimpan di jalur lain
 > 4. Saat mengubah drainase kelas atas Realesrgan, kotak kombo model kelas atas juga diubah bersama
 > 5. Tambahkan fungsi Periksa Perbarui
 > 6. Beberapa modifikasi logika
 > 7. Resolusi dan FPS
 > 8. Resolusi (sebelumnya) Modifikasi Pengguna (harus dimasukkan dalam bentuk 1024x768)

V 0.1.5
 >.
 2.
 3. Tambahkan beberapa video kotak kombo "Perhitungan FPS" untuk mencegah kasus tersebut dihitung sebagai FPS yang salah saat menghitung FPS dari beberapa video.
        -> r_frame_rate / avg_frame_rate dapat dipilih, dan default dihitung oleh r_frame_rate
 > 4. Saat memilih file video, kemajuan informasi video 
 > 5. Setelah file ditendang, ubah untuk membuka folder yang dipilih terakhir secara default saat memilih file lagi.

V 0.1.4
 >. Config.ini Metode Membaca File Perubahan
 > 2. Ubah informasi video dari Python AV ke FFMPEG
 > 3. Tambahkan fungsi ujung windows saat bekerja
 > 4. Dalam daftar pekerjaan, seluruh nama file ditampilkan sebagai tooltip
 >. Dalam daftar pekerjaan, setiap resolusi file (sebelum) / resolusi (setelah) / fps (sebelum) / fps (posting) notasi
 > 6. Penghapusan kotak input FPS (penghapusan karena setiap notasi file)
 > 7. Penghapusan Ukuran Perkiraan FPS Output (Penghapusan karena setiap file untuk setiap file)
 > 8. Status Kemajuan ditulis sebagai dua Proessbar dengan file/pekerjaan lengkap

V 0.1.3
 > 1. Perbaiki kesalahan perhitungan file FPS dengan beberapa informasi FPS saat mengimpor file

V 0.1.2
 >. UI Konfigurasi Perubahan   
 > 2. Perubahan logika batin  
 > Selesaikan masalah yang tidak dijalankan saat memilih dua model di bawah ini di antara model Realesrgan  
 > 4. Ubah cara menggunakan model realesrgan   
 > -> Salin file model baru (*.param) ke folder model di folder instalasi RealEsrgan tersedia.  
 >.  
 > 6. Kode Migrasi File Config.ini  
 > 7. FFMPEG Dekomposisi Gambar AAC-> FLAC  
 > 8. Modifikasi bug lainnya

V 0.1.1
 >. Penulisan Awal, FFMEPG, Realesrgan, dan Flowframe.