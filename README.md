# PROSES PENGERJAAN KALKULATOR SEDERHANA

**Membuat Struktur HTML**

1. Buat file `index.html` dan atur struktur dasar HTML
2. Menambahkan Bootstrap untuk styling dan jQuery untuk penghitungan
3. Buat halaman utama dengan card untuk input bilangan, operasi, dan hasil

**Menambahkan Input dan Pilihan Operasi**

1. Input bilangan pertama (`#bilanganPertama`) dan bilangan kedua (`#bilanganKedua`) menggunakan `<input type="number">`
2. Dropdown `<select>` untuk memilih operasi (tambah, kurang, kali, bagi)
3. Menambahkan box hasil (`#boxHasil`) untuk menampilkan hasil perhitungan

**Tombol dan Penghitungan**

1. Tombol Hitung (`#hitung`) untuk penghitungan
2. Tombol Reset (`#reset`) untuk mengosongkan input dan hasil
3. Menggunakan SweetAlert2 (Swal) untuk menampilkan pesan error dan notifikasi reset

**Logika JavaScript**

1. Ambil nilai input dengan jQuery:  
   ```javascript
   let bilanganPertama = parseFloat($('#bilanganPertama').val())
   let bilanganKedua = parseFloat($('#bilanganKedua').val())
   let operasi = $('#operasi').val()
