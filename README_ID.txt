CATATAN METER AIR RUSUN PULO JAHE TOWER — proyek Android

Paket ini adalah proyek sumber Android, bukan APK yang sudah dikompilasi. Lingkungan pembuat file ini tidak menyediakan Android SDK/Gradle sehingga APK tidak dapat dikompilasi langsung di sini.

CARA PALING MUDAH MEMBUAT APK TANPA ANDROID STUDIO:
1. Buat akun/login GitHub dan buat repository baru.
2. Upload seluruh isi folder proyek ini ke repository (termasuk folder .github/workflows).
3. Buka tab Actions, pilih workflow "Build APK", lalu tekan Run workflow (atau tunggu build otomatis setelah push).
4. Setelah selesai, buka hasil workflow dan unduh artifact bernama CatatanMeterAir-debug-apk.
5. Ekstrak ZIP artifact; di dalamnya ada app-debug.apk. Pindahkan ke HP Android dan buka untuk instalasi. Jika diminta, izinkan instalasi aplikasi dari sumber tersebut.

STATUS FITUR OFFLINE:
- Halaman HTML dimuat dari aset lokal, bukan dari website hosting.
- Catatan disimpan dengan localStorage di dalam WebView aplikasi.
- Kamera/pemilih foto disiapkan.
- PENTING: OCR Tesseract.js dan ekspor ExcelJS pada HTML sumber masih dimuat dari CDN internet. Jadi OCR dan ekspor XLSX belum sepenuhnya offline. Untuk offline total, file pustaka itu harus dibundel lokal dan diuji.

CATATAN: APK debug untuk uji coba, bukan rilis bertanda tangan untuk distribusi luas. Backup data secara berkala; menghapus data aplikasi atau uninstall dapat menghapus catatan lokal.
