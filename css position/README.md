# CSS Position

## Penjelasan Kode

### Position Static

- `.static-box { position: static; }`
  - Position `static` adalah nilai default yang ada pada elemen. Elemen ditempatkan sesuai dengan aliran dokumen normal dan tidak dapat diubah dengan properti `top`, `right`, `bottom`, atau `left`.

### Position Relative

- `.relative-box { position: relative; top: 20px; left: 20px; }`
  - Dengan `position: relative`, elemen ditempatkan sesuai dengan aliran dokumen normal tetapi bisa dipindahkan menggunakan properti `top`, `right`, `bottom`, dan `left`. Perpindahan ini relatif terhadap posisi aslinya.

### Position Absolute

- `.absolute-box { position: absolute; top: 50px; left: 50px; }`
  - Elemen dengan `position: absolute` ditempatkan relatif terhadap elemen induk terdekat yang memiliki posisi selain `static`. Jika tidak ada elemen induk yang diatur, maka elemen akan diposisikan relatif terhadap elemen `<html>`.

### Position Fixed

- `.fixed-box { position: fixed; top: 10px; right: 10px; }`
  - Elemen dengan `position: fixed` ditempatkan relatif terhadap jendela browser dan tidak akan bergerak saat halaman digulir. Properti `top`, `right`, `bottom`, dan `left` dapat digunakan untuk menentukan posisinya.

### Position Sticky

- `.sticky-box { position: sticky; top: 0; }`
  - Elemen dengan `position: sticky` adalah campuran antara `relative` dan `fixed`. Elemen ini berperilaku seperti elemen `relative` sampai mencapai posisi tertentu di halaman, kemudian berperilaku seperti elemen `fixed`.

## Kesimpulan

Properti `position` dalam CSS memberikan kontrol penuh atas bagaimana elemen diatur dan ditampilkan di halaman web. Dengan memahami perbedaan antara `static`, `relative`, `absolute`, `fixed`, dan `sticky`, Anda dapat menciptakan layout yang lebih dinamis dan responsif.
