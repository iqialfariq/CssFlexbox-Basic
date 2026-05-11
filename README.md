# 🧠 Penjelasan CSS Flexbox
<p align="justify">
Flexbox (Flexible Box Layout) adalah metode layout CSS satu dimensi yang digunakan untuk mengatur elemen dalam baris (row) atau kolom (column) secara fleksibel dan responsif. 
Dengan flexbox, elemen bisa otomatis melebar, mengecil, atau menyesuaikan ruang tanpa perlu menggunakan float atau positioning manual. </p>

  Margin memiliki 4 sisi:
  1. Mengatur elemen secara horizontal atau vertikal. 
  2. Membagi ruang kosong secara proporsional. 
  3. Memudahkan alignment (posisi) dan distribusi ruang. 
  4. Elemen bisa wrap ke baris baru jika ruang tidak cukup.

---

## 📌 Property dan Value CSS Flexbox

### 🌐 Flex Direction 
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

### 🌐 Flex Wrap
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
   
### 🌐 Justify Content 
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
