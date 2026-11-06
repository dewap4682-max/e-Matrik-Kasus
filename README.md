# e-Matrik Kasus PWA untuk iPhone/iPad

PWA (Progressive Web App) ini dibuat agar pengguna iOS dapat memasang e-Matrik Kasus dari Safari ke Layar Utama. Ini **bukan APK yang dikonversi**; iOS tidak dapat menjalankan file `.apk` Android.

## Cara memasang pada iPhone/iPad
1. Unggah seluruh isi folder ini ke hosting web yang menggunakan **HTTPS** (misalnya GitHub Pages, Netlify, atau hosting situs milik Anda). Jangan hanya membuka `index.html` dari Files atau `file://`.
2. Buka alamat situs tersebut menggunakan **Safari** pada iPhone/iPad.
3. Tekan tombol **Bagikan** (kotak dengan panah ke atas), pilih **Tambahkan ke Layar Utama / Add to Home Screen**, lalu tekan **Tambah / Add**.
4. Buka ikon **e-Matrik** dari Layar Utama. Sesudah pemuatan awal, shell aplikasi dapat dibuka offline.

## Fitur prototipe web
- Akun Super User/Admin dengan kata sandi lokal.
- Kategori BOS, DPRD, BANK BRI, kategori tambah/edit/hapus khusus Super User, ikon bawaan atau unggah gambar.
- Input nomor/tanggal laporan, semua menu matrik, foto Saksi/E-Elektronik/Tersangka.
- Simpan JPG ke arsip lokal IndexedDB; lihat/bagikan arsip melalui Pengaturan; hapus arsip hanya sebagai Super User.
- Bagikan JPG lewat Web Share API jika didukung. PDF menggunakan dialog cetak Safari: pilih **Print/Cetak**, lalu simpan atau bagikan PDF dari lembar berbagi iOS.
- Backup JSON berisi kategori dan catatan teks. Foto dan berkas arsip JPG tidak masuk backup.
- Ikon Layar Utama menggunakan gambar timbangan hijau-emas yang dipilih pengguna; logo Kejaksaan Negeri Ponorogo tetap di header dalam aplikasi.

## Catatan penyimpanan dan keamanan
- Data tersimpan di browser/perangkat ini (IndexedDB); tidak ada sinkronisasi server.
- Membersihkan data situs, menghapus aplikasi web, atau menghapus data Safari dapat menghilangkan isi lokal. Unduh backup JSON dan simpan foto/laporan penting secara terpisah.
- Untuk penggunaan operasional/organisasi, hosting HTTPS, pengelolaan akun, retensi data, keamanan, dan prosedur backup perlu dikonfigurasi dan diuji lebih lanjut.
