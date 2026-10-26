# mobile timer

Timer kubus khusus HP, dibuat sebagai web port (HTML + CSS + JavaScript) supaya bisa jalan di Android dan di-deploy ke Vercel.

Fitur:
- Timer 3x3 dan 2x2, scramble + diagram net scramble
- Tahan 0,55 detik (merah -> kuning -> hijau) untuk mulai
- Inspection 15 detik: ketuk sekali, lalu tahan sampai hijau untuk mulai
- Statistik AO5 / AO12 / AO100 / MEAN, PB, list waktu dengan +2 / DNF / hapus
- Cloud Firebase Firestore (project: mobile timer, ID timerv2-1-4, lokasi asia-southeast1): solve baru juga tersimpan di cloud, data cloud digabung ke lokal saat dibuka. LocalStorage tetap jadi penyimpanan utama supaya timer jalan offline.

Atribusi:
- Desain, font, dan beberapa konstanta timer diambil dari proyek open source CubeTime (CubeLabsNZ/CubeTime, lisensi GPL-3.0). Font Recursive (RecMonoVariable.ttf) dan Rubik (Rubik.ttf) berasal dari folder CubeTime/Ext/Fonts di repo tersebut.
- Ini adalah port web, bukan aplikasi Swift asli CubeTime, jadi kode Swift-nya tidak di-upload mentah ke sini.

Cara pakai:
- Buka `index.html` di browser HP, atau deploy repo ini ke Vercel sebagai proyek statis (tanpa build).
