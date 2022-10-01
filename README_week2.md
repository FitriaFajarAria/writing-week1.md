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

Tipe data numerik memiliki dua tipe bawaan yaitu Number dan BigInt.

- BigInt adalah primitif numerik dalam JavaScript yang dapat mewakili bilangan bulat dengan presisi arbitrer. Dengan BigInts, kita dapat dengan aman menyimpan dan mengoperasikan bilangan bulat besar bahkan di luar batas bilangan bulat aman untuk Numbers. BigInt dibuat dengan menambahkan n ke akhir bilangan bulat atau dengan memanggil konstruktor. Kita dapat memperoleh nilai aman terbesar yang dapat ditambahkan dengan Numbers dengan menggunakan konstanta Number.MAX_SAFE_INTEGER. 
kita dapat menggunakan operator +, *, -, **,.

- NaN ("Bukan Angka") biasanya ditemui ketika hasil operasi aritmatika tidak dapat dinyatakan sebagai angka. Ini juga satu-satunya nilai dalam JavaScript yang tidak sama dengan dirinya sendiri.


- String type

Tipe Data String digunakan untuk mewakili data tekstual, setiap elemen dalam String menempati posisi dalam String. Elemen pertama berada pada indeks 0, berikutnya pada indeks 1, dan seterusnya. Panjang dari sebuah String adalah jumlah elemen di dalamnya. String JavaScript tidak dapat diubah. Ini berarti bahwa setelah string dibuat, tidak mungkin untuk mengubahnya.
Namun, masih dimungkinkan untuk membuat string lain berdasarkan operasi pada string asli. Sebagai contoh:
1. Sebuah substring dari aslinya dengan memilih huruf individu atau menggunakan substring().
2. Penggabungan dua string menggunakan operator penggabungan (+) atau concat().


- Symbol type

Simbol adalah nilai primitif yang unik dan tidak dapat diubah dan dapat digunakan sebagai kunci dari properti Objek. Dalam beberapa bahasa pemrograman, Simbol disebut "atom".Simbol sering digunakan untuk menambahkan kunci properti unik ke objek yang tidak akan bertabrakan dengan kunci yang mungkin ditambahkan oleh kode lain ke objek, dan yang disembunyikan dari mekanisme apa pun yang biasanya digunakan kode lain untuk mengakses objek. Untuk membuat Simbol primitif baru, kita menulis Symbol() dengan string opsional sebagai deskripsinya:

            const sym1 = Symbol();
            const sym2 = Symbol('foo');
            const sym3 = Symbol('foo');
            
 
 
 - Objects
 
 Dalam ilmu komputer, objek adalah nilai dalam memori yang mungkin dirujuk oleh pengenal.
 
 - Properties
 
Dalam JavaScript, objek dapat dilihat sebagai kumpulan properti. Dengan sintaks literal objek, sekumpulan properti terbatas diinisialisasi; maka properti dapat ditambahkan dan dihapus. Nilai properti dapat berupa nilai jenis apa pun, termasuk objek lain, yang memungkinkan membangun struktur data yang kompleks. Properti diidentifikasi menggunakan nilai kunci. Nilai kunci adalah nilai String atau nilai Simbol. Ada dua jenis properti objek: properti data dan properti pengakses. Setiap properti memiliki atribut yang sesuai. Setiap atribut diakses secara internal oleh mesin JavaScript, tetapi Anda dapat mengaturnya melalui Object.defineProperty(), atau membacanya melalui Object.getOwnPropertyDescriptor().
 

### Data property

Properti data mengaitkan kunci dengan nilai. Hal ini dapat dijelaskan dengan atribut berikut:

- value
Nilai yang diambil oleh akses get properti. Dapat berupa nilai JavaScript apa pun.

### Accessor property

Mengaitkan kunci dengan salah satu dari dua fungsi pengakses (dapatkan dan setel) untuk mengambil atau menyimpan nilai. Properti accessor memiliki atribut berikut:
- get = Fungsi yang dipanggil dengan daftar argumen kosong untuk mengambil nilai properti setiap kali akses get ke nilai dilakukan. 
- set = Fungsi yang dipanggil dengan argumen yang berisi nilai yang ditetapkan. Dieksekusi setiap kali properti tertentu dicoba untuk diubah. 
- enumerable = Nilai boolean yang menunjukkan jika properti dapat dihitung oleh for...in loop.
- configurable = Nilai boolean yang menunjukkan apakah properti dapat dihapus, dapat diubah menjadi properti data, dan dapat mengubah atributnya.


### Structured data: JSON

JSON (JavaScript Object Notation) Meskipun bukan subset ketat, JSON sangat mirip dengan subset sintaks JavaScript. Meskipun banyak bahasa pemrograman mendukung JSON, ini sangat berguna untuk aplikasi berbasis JavaScript, termasuk situs web dan ekstensi browser.

JSON dapat mewakili angka, boolean, string, null, array (urutan nilai berurutan), dan objek (pemetaan nilai string) yang terdiri dari nilai-nilai ini (atau array dan objek lain). JSON tidak secara asli mewakili tipe data yang lebih kompleks seperti fungsi, ekspresi reguler, tanggal, dan sebagainya. (Objek tanggal secara default membuat serial ke string yang berisi tanggal dalam format ISO, sehingga informasinya tidak sepenuhnya hilang.) Jika Anda memerlukan JSON untuk mewakili tipe data tambahan, ubah nilai saat diserialisasi atau sebelum dideserialisasi.

## String

Objek String digunakan untuk mewakili dan memanipulasi urutan karakter. String berguna untuk menyimpan data yang dapat direpresentasikan dalam bentuk teks. Beberapa operasi yang paling sering digunakan pada string adalah memeriksa panjangnya, membangun dan menggabungkannya menggunakan operator string + dan +=, memeriksa keberadaan atau lokasi substring dengan metode indexOf(), atau mengekstrak substring dengan substring () metode. String dapat dibuat sebagai primitif, dari literal string, atau sebagai objek, menggunakan konstruktor String(). Primitif string dan objek string memiliki banyak perilaku, tetapi memiliki perbedaan dan peringatan penting lainnya.

### Character access

Ada dua cara untuk mengakses karakter individu dalam sebuah string. Yang pertama adalah metode charAt() :

            'cat'.charAt(1) // gives value "a"
           
Cara lain adalah dengan memperlakukan string sebagai objek seperti array, di mana karakter individu sesuai dengan indeks numerik:

            'cat'[1] // gives value "a"

Object.defineProperty() mendefinisikan properti baru secara langsung pada objek, atau memodifikasi properti yang ada pada objek, dan mengembalikan objek.

            Object.defineProperty(obj, prop, descriptor)
            
            
   - obj (Objek untuk mendefinisikan properti).
   - prop (Nama atau Simbol properti yang akan didefinisikan atau dimodifikasi).
   - descriptor (untuk properti yang sedang didefinisikan atau dimodifikasi).
   - Return value (Objek yang diteruskan ke fungsi).

### Comparing strings

Dalam C, fungsi strcmp() digunakan untuk membandingkan string. Dalam JavaScript, kita cukup menggunakan operator kurang dari dan lebih besar dari.

### String primitives and String objects

JavaScript membedakan antara objek String dan nilai string primitif. String literal (dilambangkan dengan tanda kutip ganda atau tunggal) dan string yang dikembalikan dari panggilan String dalam konteks non-konstruktor (yaitu, dipanggil tanpa menggunakan kata kunci baru) adalah string primitif. Dalam konteks di mana metode akan dipanggil pada string primitif atau pencarian properti terjadi, JavaScript akan secara otomatis membungkus string primitif dan memanggil metode atau melakukan pencarian properti pada objek pembungkus sebagai gantinya.


                  const strPrim = "foo"; // A literal is a string primitive
                  const strPrim2 = String(1); // Coerced into the string primitive "1"
                  const strPrim3 = String(true); // Coerced into the string primitive "true"
                  const strObj = new String(strPrim); // String with new returns a string wrapper object.

                  console.log(typeof strPrim); // Logs "string"
                  console.log(typeof strPrim2); // Logs "string"
                  console.log(typeof strPrim3); // Logs "string"
                  console.log(typeof strObj);  // Logs "object"
                  
String primitif dan objek String juga memberikan hasil yang berbeda saat menggunakan eval(). Primitif yang diteruskan ke eval diperlakukan sebagai kode sumber Objek string diperlakukan seperti semua objek lainnya, dengan mengembalikan objek. Sebagai contoh:

                  const s1 = '2 + 2';              // creates a string primitive
                  const s2 = new String('2 + 2');  // creates a String object
                  console.log(eval(s1));           // returns the number 4
                  console.log(eval(s2));           // returns the string "2 + 2"
 
 Objek String selalu dapat dikonversi ke mitra primitifnya dengan metode valueOf().
 
                  console.log(eval(s2.valueOf()))  // returns the number 4
 
 ### Long literal strings
 
Biasanya kode akan menyertakan string yang sangat panjang, daripada memiliki garis yang terus-menerus sangat panjang, kita bisa secara khusus memecah string menjadi beberapa baris dalam kode sumber tanpa mempengaruhi konten string yang sebenarnya.Untuk itu dapat menggunakan operator (tambah dan kurang +-) untuk menambahkan beberapa string bersama-sama, seperti ini:

                    const longString = "This is a very long string which needs " +
                   "to wrap across multiple lines because " +
                   "otherwise my code is unreadable."
                   
Atau dapat menggunakan karakter garis miring terbalik (\) di akhir setiap baris untuk menunjukkan bahwa string akan berlanjut pada baris berikutnya.       

                    const longString = "This is a very long string which needs \
                    to wrap across multiple lines because \
                    otherwise my code is unreadable."
                    
### Constructor

String() Membuat objek String baru. Ia melakukan konversi tipe ketika dipanggil sebagai fungsi, bukan sebagai konstruktor, yang biasanya lebih berguna.

- Static methods

String.fromCharCode() Mengembalikan string yang dibuat dengan menggunakan urutan nilai Unicode yang ditentukan.

- String.fromCodePoint()

Mengembalikan string yang dibuat dengan menggunakan urutan titik kode yang ditentukan.

- String.raw()

Mengembalikan string yang dibuat dari string template mentah.

### Instance properties

String.prototype.length Properti long read-only dari string berisi panjang string.

### Instance methods

- String.prototype.at() Mengembalikan karakter pada indeks yang ditentukan. Menerima bilangan bulat negatif, yang menghitung mundur dari karakter string terakhir.
- String.prototype.charAt() Mengembalikan karakter pada indeks yang ditentukan.
- String.prototype.charCodeAt() Mengembalikan angka yang merupakan nilai satuan pada indeks yang diberikan.
- String.prototype.codePointAt() Mengembalikan bilangan bulat nonnegatif yang merupakan nilai kode titik.
- String.prototype.concat() Menggabungkan teks dari dua (atau lebih) string dan mengembalikan string baru.
- String.prototype.includes() Menentukan apakah string panggilan berisi searchString.
- String.prototype.indexOf() Mengembalikan indeks di dalam objek String pemanggilan dari kemunculan pertama searchValue, atau -1 jika tidak ditemukan.
- String.prototype.lastIndexOf() Mengembalikan indeks di dalam objek String pemanggilan terakhir dari searchValue, atau -1 jika tidak ditemukan.
- String.prototype.localeCompare() Mengembalikan angka yang menunjukkan apakah string referensi compareString muncul sebelum, sesudah, atau setara dengan string yang diberikan dalam urutan pengurutan.
- String.prototype.match() Digunakan untuk mencocokkan ekspresi reguler regexp dengan string.
- String.prototype.matchAll() Mengembalikan iterator dari semua kecocokan regexp.
- String.prototype.normalize() Mengembalikan Bentuk Normalisasi Unicode dari nilai string panggilan.
- String.prototype.padEnd() Pads string saat ini dari akhir dengan string yang diberikan dan mengembalikan string baru dengan panjang targetLength.
- String.prototype.padStart() Mengisi string saat ini dari awal dengan string tertentu dan mengembalikan string baru dengan panjang targetLength.
- String.prototype.repeat() Mengembalikan string yang terdiri dari elemen objek berulang kali menghitung.
- String.prototype.replace() Digunakan untuk mengganti kemunculan searchFor menggunakan replaceWith. searchFor dapat berupa string atau Regular Expression, dan replaceWith dapat berupa string atau fungsi.
- String.prototype.replaceAll() Digunakan untuk mengganti semua kemunculan searchFor menggunakan replaceWith. searchFor dapat berupa string atau Regular Expression, dan replaceWith dapat berupa string atau fungsi.
- 
# JS DASAR DOM MANIPULATIOAN
