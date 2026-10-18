# Pixelgrow APK (Capacitor)

APK ini adalah "cangkang" Android: layar awal untuk mengisi alamat server, lalu game Pixelgrow dibuka layar penuh.
Server game tetap harus berjalan (paket `pixelgrow-demo.zip`), karena game ini multiplayer dan berbasis server.

## Cara mendapatkan APK (tanpa memasang Android Studio)
1. Buat repositori GitHub baru (privat boleh), unggah **seluruh isi folder ini** (termasuk folder `.github`).
2. Buka tab **Actions** → **Build APK** → **Run workflow**. Tunggu ±5–8 menit.
3. Buka run yang selesai → bagian **Artifacts** → unduh `pixelgrow-apk` → ekstrak → `app-debug.apk`.
4. Salin ke HP, buka, izinkan "pasang dari sumber tidak dikenal", lalu pasang.

## Cara memakai
- **Satu HP saja:** pasang Termux, jalankan server (lihat INSTALL-ANDROID.md di paket demo), lalu di aplikasi isi `http://localhost:3000`.
- **Server di komputer:** jalankan demo di komputer, isi alamat Wi-Fi yang tercetak (mis. `http://192.168.1.23:3000`). HP dan komputer harus satu Wi-Fi.
- **Server online:** isi alamat server publik Anda (disarankan https).

## Catatan
- Ini APK debug (cukup untuk dipasang sendiri). Untuk Play Store perlu APK/AAB bertanda tangan rilis.
- Alamat server disimpan; untuk mengganti, hapus data aplikasi atau pasang ulang.
- Ikon masih bawaan Capacitor. Ikon Pixelgrow ada di `client/dist/icon-512.png` pada paket demo.
