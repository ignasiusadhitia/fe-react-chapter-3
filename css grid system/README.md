# CSS Grid System

Proyek ini menampilkan penggunaan dasar-dasar CSS Grid System untuk membuat tata letak halaman web yang fleksibel dan kompleks. Dengan menggunakan CSS Grid, Anda dapat mengatur elemen-elemen dalam tata letak grid dengan lebih mudah dan terstruktur.

## Penjelasan Kode

### Grid Container

- `.grid-container { display: grid; }`
  - Menggunakan `display: grid;` pada elemen induk untuk mengaktifkan CSS Grid dan membuat elemen-elemen anak diatur dalam sebuah grid.

### Grid Template Columns dan Rows

- `.grid-container { grid-template-columns: 1fr 2fr 1fr; grid-template-rows: auto 200px auto; }`
  - Properti `grid-template-columns` mendefinisikan jumlah dan ukuran kolom dalam grid. Pada contoh ini, grid memiliki tiga kolom dengan lebar masing-masing `1fr`, `2fr`, dan `1fr`, yang berarti kolom tengah akan dua kali lebih lebar dibanding kolom lainnya.
  - Properti `grid-template-rows` mendefinisikan jumlah dan ukuran baris dalam grid. Baris pertama dan ketiga akan menyesuaikan ukurannya secara otomatis (`auto`), sementara baris kedua memiliki tinggi tetap `200px`.

### Grid Gap

- `.grid-container { grid-gap: 20px; }`
  - Properti `grid-gap` digunakan untuk menentukan jarak antara sel-sel dalam grid. Dalam contoh ini, jarak antara sel diatur menjadi `20px`.

### Grid Template Areas

- `.grid-container { grid-template-areas: "header header header" "sidebar content content" "footer footer footer"; }`
  - Properti `grid-template-areas` digunakan untuk mendefinisikan area-area di dalam grid menggunakan nama area. Pada contoh ini:
    - "header header header" membuat elemen dengan area `header` mengisi seluruh baris pertama.
    - "sidebar content content" membuat elemen dengan area `sidebar` mengisi kolom pertama baris kedua, sementara elemen dengan area `content` mengisi kolom kedua dan ketiga.
    - "footer footer footer" membuat elemen dengan area `footer` mengisi seluruh baris ketiga.

### Grid Area

- `.header { grid-area: header; }`, `.sidebar { grid-area: sidebar; }`, `.content { grid-area: content; }`, `.footer { grid-area: footer; }`
  - Properti `grid-area` digunakan untuk menempatkan elemen anak di area yang ditentukan dalam `grid-template-areas`. Setiap elemen diberi area spesifik sesuai dengan penamaan area yang telah ditentukan.

## Kesimpulan

CSS Grid System adalah alat yang sangat kuat untuk menciptakan tata letak halaman web yang kompleks dan fleksibel. Dengan memahami dan menerapkan properti seperti `grid-template-columns`, `grid-template-rows`, `grid-gap`, `grid-template-areas`, dan `grid-area`, Anda dapat mengatur elemen-elemen di halaman web dalam berbagai layout yang berbeda, memberikan pengalaman pengguna yang lebih baik dan lebih terstruktur.
