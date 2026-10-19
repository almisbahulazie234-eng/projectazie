E-TAG MANAGEMENT 3D LOBBY — VERCEL

ISI PAKET
- index.html: website statis
- vercel.json: konfigurasi Vercel
- assets/: tempat file model Blender GLB

PENTING
Model Blender (.blend) belum diekspor menjadi .glb. Jika model 3D asli ingin tampil, ekspor dari Blender sebagai glTF Binary (.glb), lalu simpan dengan nama:
assets/line-finishing-lobby.glb

CARA DEPLOY (PILIH SALAH SATU)

A. Dengan GitHub (mudah untuk pembaruan)
1. Ekstrak ZIP ini.
2. Buat repository baru di GitHub.
3. Upload semua ISI folder ini (index.html, vercel.json, folder assets) ke root repository.
4. Buka Vercel dan pilih Add New -> Project.
5. Import repository GitHub tersebut.
6. Framework Preset: Other. Build Command dan Output Directory kosongkan jika diminta.
7. Tekan Deploy.

B. Dengan Vercel CLI
1. Instal Node.js LTS.
2. Buka terminal di folder hasil ekstrak.
3. Jalankan: npm install -g vercel
4. Jalankan: vercel login
5. Jalankan: vercel --prod
6. Ikuti instruksi sampai Vercel menampilkan URL website.

CATATAN FIREBASE
Website memakai Firebase client-side. Pastikan Firestore Security Rules dan metode autentikasi dikonfigurasi aman di Firebase Console. Jangan menganggap konfigurasi Firebase di HTML sebagai pengganti aturan keamanan database.
