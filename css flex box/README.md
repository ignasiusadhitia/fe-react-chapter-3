# CSS Flexbox

Proyek ini menampilkan penggunaan berbagai properti Flexbox untuk mengatur tata letak elemen di dalam sebuah kontainer secara fleksibel. Kode ini dirancang untuk membantu Anda memahami bagaimana menggunakan Flexbox untuk membuat tata letak yang responsif dan dinamis.

## Penjelasan Kode

### Flex Container

- `.flex-container { display: flex; }`
  - Menggunakan `display: flex;` pada elemen induk untuk mengaktifkan Flexbox dan membuat elemen anak diatur dalam sebuah kontainer fleksibel. Ini adalah dasar untuk memulai menggunakan Flexbox, di mana elemen anak akan diatur secara otomatis sesuai dengan aturan Flexbox.

### Flex Direction

- `.flex-container { flex-direction: row; }`
  - Properti `flex-direction` menentukan arah susunan elemen anak di dalam kontainer Flexbox. Nilai-nilai yang tersedia meliputi:
    - `row`: Menyusun elemen anak dari kiri ke kanan. Ini adalah nilai default.
    - `row-reverse`: Menyusun elemen anak dari kanan ke kiri.
    - `column`: Menyusun elemen anak dari atas ke bawah.
    - `column-reverse`: Menyusun elemen anak dari bawah ke atas.

### Justify Content

- `.flex-container { justify-content: space-between; }`
  - Properti `justify-content` digunakan untuk menyelaraskan elemen anak secara horizontal dalam kontainer Flexbox. Nilai-nilai yang tersedia meliputi:
    - `flex-start`: Menyelaraskan elemen anak di awal kontainer (kiri untuk `row`).
    - `flex-end`: Menyelaraskan elemen anak di akhir kontainer (kanan untuk `row`).
    - `center`: Menyelaraskan elemen anak di tengah kontainer.
    - `space-between`: Membuat ruang yang sama di antara elemen anak. Elemen pertama dan terakhir ditempatkan di ujung kontainer.
    - `space-around`: Membuat ruang yang sama di sekitar setiap elemen anak, termasuk di sisi luar elemen pertama dan terakhir.
    - `space-evenly`: Membagi ruang secara merata di antara semua elemen anak, termasuk ruang di sisi luar elemen pertama dan terakhir.

### Align Items

- `.flex-container { align-items: center; }`
  - Properti `align-items` digunakan untuk menyelaraskan elemen anak secara vertikal di dalam kontainer Flexbox. Nilai-nilai yang tersedia meliputi:
    - `stretch`: Membuat elemen anak merenggang untuk mengisi kontainer (nilai default).
    - `flex-start`: Menyelaraskan elemen anak di awal kontainer secara vertikal.
    - `flex-end`: Menyelaraskan elemen anak di akhir kontainer secara vertikal.
    - `center`: Menyelaraskan elemen anak di tengah kontainer secara vertikal.
    - `baseline`: Menyelaraskan elemen anak berdasarkan garis dasar teks.

### Flex Wrap

- `.flex-container { flex-wrap: wrap; }`
  - Properti `flex-wrap` menentukan apakah elemen anak harus dibungkus ke baris atau kolom baru jika ruang dalam kontainer tidak cukup. Nilai-nilai yang tersedia meliputi:
    - `nowrap`: Semua elemen anak akan tetap berada dalam satu baris atau kolom, meskipun ruang tidak cukup (nilai default).
    - `wrap`: Elemen anak akan dibungkus ke baris atau kolom baru jika ruang tidak cukup.
    - `wrap-reverse`: Elemen anak akan dibungkus ke baris atau kolom baru dalam urutan terbalik.

### Flex Grow

- `.flex-item { flex-grow: 1; }`
  - Properti `flex-grow` menentukan seberapa banyak elemen anak akan tumbuh relatif terhadap elemen lainnya dalam kontainer. Nilai `1` berarti elemen akan tumbuh untuk mengisi ruang yang tersedia secara proporsional dengan elemen lainnya. Jika nilai `0`, elemen tidak akan tumbuh.

### Flex Shrink

- `.flex-item { flex-shrink: 1; }`
  - Properti `flex-shrink` menentukan seberapa banyak elemen anak akan menyusut relatif terhadap elemen lainnya ketika ruang tidak mencukupi. Nilai `1` berarti elemen akan menyusut dengan proporsi yang sama ketika ruang terbatas. Jika nilai `0`, elemen tidak akan menyusut.

### Flex Basis

- `.flex-item { flex-basis: 100px; }`
  - Properti `flex-basis` menentukan ukuran awal elemen anak sebelum ruang tambahan dibagi di antara elemen lainnya. Nilai ini bisa dalam satuan panjang seperti `px`, `em`, atau persentase (`%`), atau bisa juga menggunakan kata kunci `auto`, yang berarti ukuran ditentukan oleh konten elemen.

## Kesimpulan

Flexbox adalah alat yang sangat kuat untuk menciptakan tata letak halaman yang responsif dan fleksibel. Dengan memahami dan menerapkan berbagai properti Flexbox seperti `flex-direction`, `justify-content`, `align-items`, `flex-wrap`, `flex-grow`, `flex-shrink`, dan `flex-basis`, Anda dapat dengan mudah mengatur elemen-elemen di halaman web untuk memberikan pengalaman pengguna yang lebih baik dan lebih dinamis.
