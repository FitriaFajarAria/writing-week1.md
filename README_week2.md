# JS DASAR SCOPE AND FUNCTION
## Scope

Scope adalah konsep dalam flow data variabel. Scope dalam JavaScript adalah konsep yang digunakan untuk membatasi pengaksesan suatu variabel. 
Ada dua tipe scope yaitu lokal dan global.Menentukan suatu variabel bisa diakses pada scope tertentu atau tidak.

   - Global variables adalah variabel yang dideklarasikan di luar blok.
   - Local variables adalah variabel yang dideklarasikan di dalam suatu blok bisa berupa function-scoped atau block-scoped.

#### Blocks

Blocks adalah code yang berada didalam curly braces {}. Conditional, function, dan  looping menggunakan blocks.

#### Global Scope

Global scope berarti variabel yang kita buat dapat diakses dimanapun dalam suatu file. Agar menjadi Global Scope, suatu variabel harus dideklarasikan diluar Blocks.
Contohnya :

#### Local Scope

Local scope berarti kita mendeklarasikan variabel didalam blocks seperti function, conditional, dan looping.
Maka variabel hanya bisa diakses didalam blocks saja. Tidak bisa diakses diluar blocks. Contohnya :


## FUNCTION

Function adalah sebuah blok kode dalam sebuah grup untuk menyelesaikan 1 task/1 fitur. Saat kita membutuhkan fitur tersebut nantinya, kita bisa kembali menggunakannya.
##### Membuat Function

##### Memanggil Function

### Parameter dan Argumen

#### Parameter Function
Dengan parameter, function dapat menerima sebuah inputan data dan menggunakannya untuk melakukan task/tugas.
Saat membuat function/fitur, kita harus tahu data-data yang dibutuhkan. Misalnya saat membuat function penambahan 2 buah nilai.
Data yang dibutuhkan adalah 2 buah nilai tersebut.


#### Argumen Function

Argumen adalah nilai yang digunakan saat memanggil function.
Jumlah argumen harus sama dengan jumlah parameternya
Jadi jika di function penambahan ada 2 parameter nilai saat membuat function. Saat memanggil function kita gunakan 2 buah nilai argumen.


### Default Parameters

Default paramaters digunakan untuk memberikan nilai awal/default pada parameter function.
Default parameters bisa digunakan jika kita ingin menjaga function agar tidak error saat dipanggil tanpa argumen.


### Function Helper



### Arrow Function

Arrow function adalah cara lain menuliskan function. Ini adalah fitur terbaru yang ada pada ES6 (Javascript Version)


### Short Syntax Function



##  Errors dan Debugging

### Error

Saat menjalankan kode JavaScript, kesalahan yang berbeda dapat terjadi.Kesalahan dapat berupa kesalahan pengkodean yang dilakukan oleh programmer, 
kesalahan karena salah input, dan hal-hal yang tidak terduga lainnya. Lalu kemudian JavaScript akan membuat objek Error dengan dua properti yaitu nama dan pesan.

### Debugging

Debugging adalah proses menguji, menemukan, dan mengurangi bug (kesalahan) pada program komputer.
Kode pemrograman mungkin berisi kesalahan sintaks, atau kesalahan logis. Banyak dari kesalahan ini sulit untuk didiagnosis.
Seringkali, ketika kode pemrograman mengandung kesalahan, tidak akan terjadi apa-apa.Tidak ada pesan kesalahan, 
dan kita tidak akan mendapatkan indikasi di mana harus mencari kesalahan.Mencari (dan memperbaiki) kesalahan dalam kode pemrograman disebut debugging kode.
Debugging tidak mudah. Tapi untungnya, semua browser modern memiliki debugger JavaScript bawaan. 
kita bisa mengaktifkan debugging di browser dengan tombol F12, dan pilih "Konsol" di menu debugger.

#### Metode console.log()

Kita dapat menggunakan console.log() untuk menampilkan nilai JavaScript di jendela debugger. Contohnya :

            <!DOCTYPE html>
              <html>
                  <body>
                    <h1>Haii</h1>
                    <script>
                        a = 5;
                        b = 6;
                        c = a + b;
                        console.log(c);
                        </script>
                   </body>
              </html>



#### Debugging Pada Peramban Utama

Kita bisa mengaktifkan debugging di browser dengan menggunakan F12, dan pilih "Konsol" di menu debugger. Namun pada beberapa peramban 
terdapat juga cara untuk mengaktifkan debugging seperti contoh beberapa peramban dibawah :

- Chrome
  - Buka peramban.
  - Setting, pilih "Alat lainnya".
  - pilih "Alat pengembang".
  - Terakhir, pilih Konsol.


- Firefox
  - Buka peramban.
  - Setting, pilih "Pengembang Web".
  - Terakhir, pilih "Konsol Web".
