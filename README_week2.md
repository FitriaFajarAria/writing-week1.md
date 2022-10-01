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


## Function

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

#### Macam-Macam Error

- Eval Error
   
Membuat instance yang mewakili kesalahan yang terjadi terkait fungsi global eval().

- Range Error (A number "out of range" has occurred)

Membuat instance yang mewakili kesalahan yang terjadi saat variabel numerik atau parameter berada di luar rentang validnya.

- Reference Error (An illegal reference has occurred)

Membuat instance yang mewakili kesalahan yang terjadi saat mereferensikan referensi yang tidak valid.

- Syntax Error (A syntax error has occurred)

Membuat instance yang mewakili kesalahan sintaks.

- Type Error (A type error has occurred)

Membuat instance yang mewakili kesalahan yang terjadi saat variabel atau parameter bukan tipe yang valid.

- URI Error (An error in encodeURI() has occurred)

Membuat instance yang mewakili kesalahan yang terjadi saat encodeURI() atau decodeURI() melewati parameter yang tidak valid.
URI (Uniform Resource Identifier) .

- Aggregate Error

Membuat instance yang mewakili beberapa kesalahan yang dibungkus dalam satu kesalahan ketika beberapa kesalahan perlu dilaporkan oleh suatu operasi, misalnya oleh Promise.any().

- Internal Non-Standard Error

Membuat instance yang mewakili kesalahan yang terjadi saat kesalahan internal di mesin JavaScript dilemparkan. Misalnya. "terlalu banyak rekursi".



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

# JS DASAR  Data Type Built in Prototype & Method

## Data Type

### Tipe Data JavaScript dan Struktur Data

Himpunan tipe dalam bahasa JavaScript terdiri dari nilai dan objek primitif.

#### Primitive values (Nilai Primitif)

Semua jenis kecuali objek mendefinisikan nilai yang tidak dapat diubah (yaitu, nilai yang tidak dapat diubah). Misalnya, String tidak dapat diubah. Kita dapat menyebut nilai jenis ini sebagai "nilai primitif".
 
- Boolean type = Boolean mewakili entitas logis dan dapat memiliki dua nilai: benar dan salah. 
   
Misalnya, dalam JavaScript, kondisional Boolean sering digunakan untuk memutuskan bagian kode mana yang akan dieksekusi (seperti dalam pernyataan if) atau ulangi (seperti dalam perulangan for).
   
   
                   /* JavaScript if statement */
                     if (boolean conditional) {
                     // code to execute if the conditional is true
                     }

                     if (boolean conditional) {
                      console.log("boolean conditional resolved to true");
                     } else {
                      console.log("boolean conditional resolved to false");
                     }

                     /* JavaScript for loop */
                     for (control variable; boolean conditional; counter) {
                     // code to execute repeatedly if the conditional is true
                     }
              

- Null type

Tipe Null memiliki tepat satu nilai, Nilai null mewakili ketidakhadiran yang disengaja dari nilai objek apa pun. Ini adalah salah satu nilai primitif JavaScript dan diperlakukan sebagai salah untuk operasi boolean. null mengungkapkan kurangnya identifikasi, yang menunjukkan bahwa variabel tidak menunjuk ke objek. 


                     typeof null          // "object" (not "null" for legacy reasons)
                     typeof undefined     // "undefined"
                     null === undefined   // false
                     null  == undefined   // true
                     null === null        // true
                     null  == null        // true
                     !null                // true
                     isNaN(1 + null)      // false
                     isNaN(1 + undefined) // true
                     
                     
- Undefined type

Variabel yang belum diberi nilai memiliki nilai yang tidak ditentukan. Properti undefined global mewakili nilai primitif yang tidak terdefinisi. Ini adalah salah satu tipe primitif JavaScript. Variabel yang belum diberi nilai bertipe undefined. Sebuah metode atau pernyataan juga mengembalikan undefined jika variabel yang sedang dievaluasi tidak memiliki nilai yang ditetapkan. Sebuah fungsi mengembalikan undefined jika nilai tidak dikembalikan.


                     function test(t) {
                     if (t === undefined) {
                     return 'Undefined value!';
                     }
                     return t;
                     }

                     let x;

                     console.log(test(x));
                     // expected output: "Undefined value!"
                     
                     
- Numeric types
                     
# JS DASAR DOM MANIPULATIOAN
