# 🧠 Penjelasan CSS Flexbox
<p align="justify">
Flexbox (Flexible Box Layout) adalah metode layout CSS satu dimensi yang digunakan untuk mengatur elemen dalam baris (row) atau kolom (column) secara
fleksibel dan responsif. Dengan flexbox, elemen bisa otomatis melebar, mengecil, atau menyesuaikan ruang tanpa perlu menggunakan float atau positioning manual.
</p>

  Sifat utama flexbox:
  1. Mengatur elemen secara horizontal atau vertikal. 
  2. Membagi ruang kosong secara proporsional. 
  3. Memudahkan alignment (posisi) dan distribusi ruang. 
  4. Elemen bisa wrap ke baris baru jika ruang tidak cukup.

---

## 📌 Property dan Value CSS Flexbox

### 🔀 Flex Direction 
<p align="justify">
digunakan untuk menentukan arah utama (main axis) dari flex container. Dengan kata lain, ia mengatur apakah item flex ditata secara horizontal (baris) atau vertikal (kolom).
</p>

value flex-direction ada 4 yaitu:
1) row (default) - Item ditata dari kiri ke kanan (horizontal).
2) row-reverse - Item ditata dari kanan ke kiri. 
3) column - Item ditata dari atas ke bawah (vertikal). 
4) column-reverse - Item ditata dari bawah ke atas. 

  Contoh:
  ```css
      .row {
        flex-direction: row; /* item berjejer ke samping */
      }
  ```

---

### 📦 Flex Wrap
<p align="justify">
digunakan untuk menentukan apakah item flex di dalam container boleh membungkus ke baris/kolom baru ketika ruang tidak cukup. Secara default, flex items akan mencoba tetap berada dalam satu baris, meskipun ukurannya jadi sangat kecil.
</p>

value flex-wrap ada 3 yaitu:
1) nowrap (default) 
    • Semua item tetap dalam satu baris/kolom. 
    • Jika ruang tidak cukup, item akan mengecil. 
2) wrap 
    • Item akan otomatis pindah ke baris/kolom baru jika ruang tidak cukup. 
3) wrap-reverse
    • Sama seperti wrap, tetapi arah baris/kolom baru dibalik. 
    • Misalnya baris baru muncul di atas, bukan di bawah.
   
  Contoh:
  ```css
      .wrap {
        flex-wrap: wrap;
      }
  ```

---

### 📏 Justify Content 
<p align="justify">
digunakan untuk mengatur posisi atau jarak item di sepanjang main axis (sumbu utama). 
</p>

value flex-wrap ada 3 yaitu:
1) flex-start (default) 
    • Item ditempatkan di awal main axis. 
2) lex-end 
    • Item ditempatkan di akhir main axis.
3) center 
    • Item ditempatkan di tengah main axis. 
4) space-between 
    • Item diratakan: item pertama di awal, item terakhir di akhir, sisanya merata di antaranya. 
5) space-around 
    • Item diberi jarak merata dengan ruang di kiri dan kanan setiap item.
6) space-evenly 
    • Semua item memiliki jarak yang sama, termasuk di sisi luar.    

  Contoh:
  ```css
      .center {
        justify-content: center;     /* item rata tengah */
      }
  ```

---

### 🗂️ Align Content  
<p align="justify">
digunakan untuk mengatur distribusi ruang antar baris di sepanjang cross axis (sumbu tegak lurus main axis). Berbeda dengan align-items 
yang mengatur posisi item dalam satu baris, align content bekerja hanya jika ada lebih dari satu baris (misalnya ketika flex-wrap: wrap digunakan).  
</p>

value align-content ada 7 yaitu: 
1) stretch (default) 
    • Baris flex akan meregang untuk memenuhi ruang container 
2) flex-start 
    • Semua baris ditempatkan di awal cross axis. 
3) flex-end 
    • Semua baris ditempatkan di akhir cross axis. 
4) center 
    • Semua baris ditempatkan di tengah cross axis. 
5) space-between 
    • Baris pertama di awal, baris terakhir di akhir, sisanya merata di antaranya.
6) space-around
    • Baris diberi jarak merata dengan ruang di atas dan bawah setiap baris.
7) space-evenly
    • Semua baris memiliki jarak yang sama, termasuk di sisi luar.

  Contoh:
  ```css
      .flex-start {
        align-content: flex-start;
      }
  ```

---

### 🎯 Align Items 
<p align="justify">
digunakan untuk mengatur posisi item di sepanjang cross axis (sumbu tegak lurus main axis).  
</p>

value align-items ada 5 yaitu:
1) stretch (default) 
    • Item akan meregang memenuhi container di cross axis. 
2) flex-start 
    • Item ditempatkan di awal cross axis. 
3) flex-end 
    • Item ditempatkan di akhir cross axis. 
4) center 
    • Item ditempatkan di tengah cross axis. 
5) baseline 
    • Item disejajarkan berdasarkan baseline teks.

  Contoh:
  ```css
      .flex-start {
        align-items: flex-start;
      }
  ```

---

### 🔢 Order
<p align="justify">
order adalah property CSS yang dipakai di flex item (anak dari flex container). Fungsinya buat ngatur urutan tampilan item di dalam container, tanpa harus ubah urutan HTML.
</p>

  Contoh:
  ```css
      .ordered{
        order: 2;
      }
  ```

---

### 📈 Flex Grow 
<p align="justify">
Property CSS yang dipakai di flex item (anak dari flex container). Fungsinya menentukan seberapa besar item bisa melebar untuk mengisi ruang kosong di
dalam container.
</p>

  Contoh:
  ```css
      .FlexGrow {
        flex-grow: 2;
      }
  ```

---

### 🎛️ Align Self
<p align="justify">
Property CSS yang dipakai di flex item (anak dari flex container). Fungsinya: ngatur posisi vertikal item tertentu di dalam container, override aturan
align-items yang ada di parent.
</p>

  Contoh:
  ```css
      .AlignSelf {
        align-self: flex-start;
      }
  ```
