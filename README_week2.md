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

Untuk membuat sebuah funtion pada java script kita harus membuat format functionya terlebih dahulu, contoh format penulisan function javascript. 

                     <script>
 
                        /membuat function di javascript
                        function nama_function(){
                        // isi function nya di buat di sini
                     }
 
                    </script>
                    
- Membuat Fungsi dengan Cara Biasa

                     function namaFungsi(){
                     console.log("Hello World!");
                     }
                     
- Membuat Fungsi dengan Ekspresi

                     var namaFungsi = function(){
                     console.log("Hello World!");
                     }
                     
- Membuat Fungsi dengan Tanda Panah

                    var namaFungsi = () => {
                    console.log("Hello World!");
                    }

- Membuat Fungsi dengan Kostruktor

                     var namaFungsi = new Function('console.log("Hello World!");');
                     
                     
##### Memanggil Function

Untuk memanggil fungsi di dalam Javascript kita bisa menuliskan dengan nama fungsinya seperti ini:

                     // membuat fungsi
                     function sayHello(){
                     console.log("Hello World!");
                     }

                     // memanggil fungsi
                     sayHello() // maka akan menghasilkan -> Hello World!
                     
Selain dengan cara di atas, kita juga bisa memanggil fungsi melalui atribut event pada HTML.

                     <!DOCTYPE html>
                        <html>
                        <head>
                         <script>
                       // membuat fungsi
                          var sayHello = () => alert("Hello World!");
                         </script>
                        </head>
                       <body>
                      <!-- Memanggil fungsi saat link diklik -->
                        <a href="#" onclick="sayHello()">Klik Aku!</a>
                       </body>
                       </html>
                       
                       
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

Fungsi Helper adalah fungsi JavaScript yang dapat di panggil dari template, Sintaks template Ember membatasi apa yang dapat diekspresikan untuk menjaga agar struktur aplikasi tetap jelas dalam sekejap. Saat perlu menghitung sesuatu menggunakan JavaScript dapat menggunakan fungsi pembantu.

### Arrow Function

Arrow function adalah cara lain menuliskan function. Ini adalah fitur terbaru yang ada pada ES6 (Javascript Version)


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
- String.prototype.slice() Mengekstrak bagian string dan mengembalikan string baru.


## Number

Number adalah objek pembungkus primitif yang digunakan untuk mewakili dan memanipulasi angka seperti 37 atau -9,25. Nilai dari tipe lain dapat dikonversi ke angka menggunakan fungsi Number(). When used as a function, Number(value) converts a string or other value to the Number type. If the value can't be converted, it returns NaN.

               Number("123"); // returns the number 123
               Number("123") === 123; // true

               Number("unicorn"); // NaN
               Number(undefined); // NaN

### Static properties

- Number.EPSILON Interval terkecil antara dua angka yang dapat diwakili.
- Number.MAX_SAFE_INTEGER Integer maksimum dalam JavaScript (253 - 1).
- Number.MAX_VALUE bilangan positif terbesar.
- Number.MIN_SAFE_INTEGER Integer minimum dalam JavaScript (-(253 - 1)).
- Number.MIN_VALUE Angka terkecil yang dapat diwakili positif—yaitu, angka positif yang paling dekat dengan nol.
- Number.NaN Nilai khusus "Not a Number".
- Number.NEGATIVE_INFINITY Nilai khusus mewakili tak terhingga negatif. Dikembalikan pada overflow.
- Number.POSITIVE_INFINITY Nilai khusus yang mewakili tak terhingga positif. Dikembalikan pada overflow.
- Number.prototype Memungkinkan penambahan properti ke objek Number.


### Static methods 
- Number.isNaN() Tentukan apakah nilai yang diteruskan adalah NaN.
- Number.isFinite() Tentukan apakah nilai yang diteruskan adalah bilangan berhingga.
- Number.isInteger() Tentukan apakah nilai yang diteruskan adalah bilangan bulat.
- Number.isSafeInteger() Tentukan apakah nilai yang diteruskan adalah bilangan bulat yang aman (nomor antara -(253 - 1) and 253 - 1).
- Number.parseFloat() Ini sama dengan fungsi parseFloat() global.
- Number.parseInt() Ini sama dengan fungsi parseInt() global.


Menggunakan objek Number untuk menetapkan nilai ke variabel numerik
Contoh berikut menggunakan properti objek Number untuk menetapkan nilai ke beberapa variabel numerik:

               const biggestNum = Number.MAX_VALUE;
               const smallestNum = Number.MIN_VALUE;
               const infiniteNum = Number.POSITIVE_INFINITY;
               const negInfiniteNum = Number.NEGATIVE_INFINITY;
               const notANum = Number.NaN;
               
### Integer range for Number

Contoh berikut menunjukkan nilai integer minimum dan maksimum yang dapat direpresentasikan sebagai objek Number. 
   
               const biggestInt = Number.MAX_SAFE_INTEGER; //  (2**53 - 1) =>  9007199254740991
               const smallestInt = Number.MIN_SAFE_INTEGER; // -(2**53 - 1) => -9007199254740991
               
Saat mem-parsing data yang telah diserialisasi ke JSON, nilai integer yang berada di luar rentang ini diperkirakan akan rusak saat parser JSON memaksanya ke tipe Number. Solusi yang mungkin adalah menggunakan String sebagai gantinya. Angka yang lebih besar dapat direpresentasikan menggunakan tipe BigInt.
Menggunakan Number() untuk mengonversi objek Date
Contoh berikut mengonversi objek Tanggal menjadi nilai numerik menggunakan Angka sebagai fungsi:

               const d = new Date("December 17, 1995 03:24:00");
               console.log(Number(d));
               

## Math

Math adalah objek bawaan yang memiliki properti dan metode untuk konstanta dan fungsi matematika. Ini bukan objek fungsi.
Matematika bekerja dengan tipe Number. Ini tidak bekerja dengan BigInt. Tidak seperti banyak objek global lainnya, Math bukanlah sebuah konstruktor. Semua properti dan metode Math bersifat statis. Banyak fungsi Math memiliki presisi yang bergantung pada implementasi. Ini berarti bahwa browser yang berbeda dapat memberikan hasil yang berbeda. Bahkan mesin JavaScript yang sama pada OS atau arsitektur yang berbeda dapat memberikan hasil yang berbeda.


### Static methods
- Math.abs() Mengembalikan nilai absolut dari x.
- Math.acos() Mengembalikan arccosinus dari x.
- Math.acosh()  Mengembalikan arccosinus hiperbolik dari x.
- Math.asin() Mengembalikan arcsine dari x.
- Math.asinh() Mengembalikan arcsinus hiperbolik suatu bilangan.
- Math.atan() Mengembalikan arctangent dari x.
- Math.atanh() Mengembalikan arktangen hiperbolik dari x.
- Math.atan2() Mengembalikan arctangent dari hasil bagi argumennya.
- Math.cbrt() Mengembalikan akar pangkat tiga dari x.
- Math.ceil() Mengembalikan bilangan bulat terkecil yang lebih besar dari atau sama dengan x.
- Math.clz32() Mengembalikan jumlah bit nol terdepan dari bilangan bulat 32-bit x.
- Math.cos() Mengembalikan kosinus dari x.
- Math.cosh() Returns the hyperbolic cosine of x. 
- Math.exp() Mengembalikan ex, di mana x adalah argumen, dan e adalah konstanta Euler (2,718…, basis logaritma natural).
- Math.expm1() Mengembalikan pengurangan 1 dari exp(x).
- Math.floor() Mengembalikan bilangan bulat terbesar yang kurang dari atau sama dengan x.
- Math.fround() Mengembalikan representasi float presisi tunggal terdekat dari x.
- Math.hypot() Mengembalikan akar kuadrat dari jumlah kuadrat argumennya.
- Math.imul() Mengembalikan hasil perkalian bilangan bulat 32-bit dari x dan y.
- Math.log() Mengembalikan logaritma natural dari x.
- Math.log10() Mengembalikan logaritma basis-10 dari x.
- Math.log2() Mengembalikan logaritma basis-2 dari x.
- Math.max() Mengembalikan bilangan terbesar dari nol atau lebih.
- Math.min() Mengembalikan angka terkecil dari nol atau lebih.
- Math.pow()  Mengembalikan basis x ke pangkat eksponen y (yaitu, xy).
- Math.random() Mengembalikan angka pseudo-acak antara 0 dan 1.
- Math.round() Mengembalikan nilai bilangan x yang dibulatkan ke bilangan bulat terdekat.
- Math.sign() Mengembalikan tanda x, yang menunjukkan apakah x positif, negatif, atau nol.
- Math.sin() Mengembalikan sinus dari x.
- Math.sinh() Mengembalikan sinus hiperbolik dari x.
- Math.sqrt() Mengembalikan akar kuadrat positif dari x.
- Math.tan() Mengembalikan tangen x.
- Math.tanh() Mengembalikan tangen hiperbolik dari x.
- Math.trunc() Mengembalikan bagian bilangan bulat dari x, menghapus setiap digit pecahan.


Dalam JavaScript, kita dapat melakukan hal berikut 

               50 * Math.tan(degToRad(60))
               
dengan menggunakan fungsi degToRad() untuk mengonversi 60 derajat ke radian, karena Math.tan() mengharapkan nilai input dalam radian.
Mengembalikan bilangan bulat acak antara dua batas ini dapat dicapai dengan kombinasi Math.random() dan Math.floor():

               function random(min, max) {
               const num = Math.floor(Math.random() * (max - min + 1)) + min;
               return num;
               }

               random(1, 10);


## Primitive & Non Primitive

## Primitif

Tipe data primitif hanya dapat menyimpan satu nilai pada satu waktu dan tidak dapat diubah menggunakan cara yang sama seperti tipe data non-primitif. Tipe data Primitif akan dianggap sama jika nilainya sama. tipe data primitif :
1. Numbers (Tipe data Number atau angka di JavaScript mewakili angka positif dan negatif entah itu bulat (integer) maupun desimal (floating-point)).
2. Strings (Tipe data String digunakan untuk mewakili data tekstual atau karakter).
3. Booleans (adalah tipe data yang hanya memiliki dua nilai, true dan false.)
4. undefined (nilai yang diberikan ketika variabel dideklarasikan tanpa inisialisasi atau tidak diberi nilai. Ini hanya berlaku untuk variabel let dan var, karena kita tidak dapat mendeklarasikan variabel const tanpa nilai).
5. null ( dapat digunakan untuk mewakili ketidakhadiran yang disengaja dari nilai objek. Kita dapat menetapkan null ke variabel untuk menunjukkan bahwa saat ini variabel tersebut tidak memiliki nilai apa pun, tapi nanti akan memilikinya).


## Non-primitif

Tipe data non-primitif (disebut secara kolektif sebagai Objek) dapat menyimpan lebih dari satu nilai pada satu waktu dan dapat diubah. Tipe data non-primitif akan dianggap berbeda meskipun nilainya sama dan dalam urutan yang sama. Tipe data non-primitif.
1. Objects (tipe data yang kompleks yang memungkinkan kita menyimpan kumpulan nilai dengan tipe data yang berbeda. Objek berisi properti yang didefinisikan sebagai pasangan kunci dan nilai (key dan value).
2. Arrays (jenis objek yang dapat digunakan untuk menyimpan beberapa nilai, tanpa properti seperti objek. Array memiliki indeks yang dimulai dari nol dengan kata lain elemen atau nilai pertama di dalam array memiliki indeks 0, elemen berikutnya memiliki indeks 1 dan seterusnya. kita bisa menggunakan indeks untuk memanipulasi nilainya) .
3. Functions


Kedua kategori mewakili dua cara berbeda tipe data ini disimpan ke dalam memori. Primitif disimpan berdasarkan nilai sedangkan Non-Primitif (Objek) disimpan berdasarkan referensi

### Perbedaan Tipe Data Primitif dan Non-primitif
#### Jumlah nilai yang dapat disimpan

- Primitif, satu nilai:

                  const nama = 'Fitria';
                  
- Non-primitif, lebih dari satu nilai:

                  const data = ['Fitria', 19, true, null, undefined];
 
 #### Perubahan Nilai
 
 - Primitif, tidak dapat diubah:
 
                  const nama = 'Fitria';
                  console.log(nama[0]); // F

                  nama[0] = 'F';
                  console.log(nama); // Fitria
                  
 - Non-primitif, dapat diubah:
 
                  const mahasiswa = ['Fitria', 'Fajar', 'Aria'];
                  mahasiswa[2] = 'Rain';

                  console.log(mahasiswa); // ["Fitria", "Fajar", "Rain"]
                  
  #### Perbandingan
  
  Kita bisa menggunakan operator kesetaraan ketat === untuk membandingkan dua buah variabel atau operan, ini akan mengembalikan nilai Boolean (true atau false).
  - Primitif, dianggap sama jika nilainya sama:
  
                  const firstName = 'Fitria';
                  const namaDepan = 'Fitria';

                  console.log(firstName === namaDepan); // true
                  
  - Non-primitif, dianggap berbeda meskipun nilai dan urutannya sama, tapi dianggap sama jika merujuk ke objek atau array yang sama.
  
                   const mahasiswa1 = ['fitria', 'fajar', 'aria'];
                   const mahasiswa2 = ['fitria', 'fajar', 'aria'];
                   console.log(mahasiswa1 === mahasiswa2); // false

                   const binatang1 = ['kucing', 'kelinci', 'ikan'];
                   const binatang2 = binatang1;
                   console.log(binatang1 === binatang2); // true
                   
                   
# JS DASAR DOM MANIPULATIOAN

DOM merupakan singkatan dari Document Object Model, dokumen (HTML) yang dimodelkan dalam sebuah objek. Objek dari dokumen ini menyediakan sekumpulan fungsi dan atribut/data yang bisa kita manfaatkan dalam membuat program Javascript. Inilah yang disebut API (Application Programming Interface). Penting untuk diingat, 
**DOM bukan bagian dari JavaScript, melainkan browser (Web API)**


![Gambar DOM](https://www.petanikode.com/img/js/dom/dom-api-html.png)

## Cara Menggunakan DOM

DOM adalah sebuah objek untuk memodelkan dokumen HTML.Objek DOM di javascript bernama document. Objek ini berisi segala hal yang kita butuhkan untuk memanipulasi HTML.
Jika kita coba ketik document pada console Javascript, maka yang akan tampil adalah kode HTML. Di dalam objek document, terdapat fungsi-fungsi dan atribut yang bisa kita gunakan untuk memanipulasi dokumen HTML. Sebagai contoh fungsi documen.write().Fungsi ini digunakan untuk menulis sesuatu ke dokumen HTML.

                     document.write("<h2>Hai Saya Sedang Megerjakan Tugas Writing</h2>");
                     
## Mengakses Elemen Dengan DOM

Apabila kita ingin mengakses elemen yang spesifik, terdapat beberapa fungsi yang bisa digunakan:
- getElementById() fungsi untuk memilih elemen berdasarkan atribut id.
- getElementByName() fungsi untuk memilih elemen berdasarkan atribut name.
- getElementByClassName() fungsi untuk memilih elemen berdasarkan atribut class.
- getElementByTagName() fungsi untuk memilih elemen berdasarkan nama tag.
- getElementByTagNameNS() fungsi untuk memilih elemen berdasarkan nama tag.
- querySelector() fungsi untuk memilih elemen berdasarkan query.
- querySelectorAll() fungsi untuk memilih elemen berdasarkan query.
- dan lain-lain.

contoh penerapan akses elemen berdasarkan ID:

                     <!DOCTYPE html>
                     <html>
                     <head>
                            <title>Contoh Penggunaan DOM</title>
                     </head>
                     <body>

                          <!-- Elemen div yang akan kita pilih dari JS -->
                         <div id="contoh"></div>


                         <script type="text/javascript">
                         // mengakses elemen contoh
                        var contoh = document.getElementById("contoh");

                        // mengisi teks ke dalam elemen
                       contoh.innerText = "Tutorial Javascript";

                        // memberikan CSS ke elemen
                      contoh.style.backgroundColor = "red";
                      contoh.style.padding = "10px";

                      </script>

                     </body>
                     </html>
                     
                     
Perlu diingat kalau getElementsByClassName itu akan ngereturn bentuk array; walaupun cuma ada 1 element dengan class itu
Kalau bisa diulangin lagi penggunaan id dan class (id cuma boleh 1 element per page, class bisa beberapa sekaligus dan per element bisa beberapa class).
                     
## Membuat Elemen dengan DOM

                     document.createElement('p');
                     
Maka, akan tercipta elemen <p> atau paragraf baru. Namun tidak akan ditampilkan ke dalam halaman web,karena belum menambahkannya ke dalam body dokumen. Cara menambahkannya ke body dokumen bisa gunakan fungsi append().     
   
                     <body>

                   <script>
                   // membuat element h1
                   var judul = document.createElement("h1");
        
                     // mengisi kontent elemen
                     judul.textContent = "Belajar Javascript";

                     // menambahkan elemen ke dalam tag body
                    document.body.append(judul);
                  </script>

                  </body>
   
 
   
## Menghapus Elemen dengan DOM
   
   menggunakan fungsi remove().
   
   
                    <body>

                     <h2 id="fitria">Delete Saya!</h2>

                   <script>
                   // memilih elemen berdasarkan ID
                  var h2 = document.getElementById('fitria');

                  // menghapus elemen yang sudah dipilih
                  h2.remove();

                 console.log("Elemen sudah dihapus");
                 console.log(h2);
                 </script>

                 </body>
   
   
## Mengubah Konten Element dengan DOM
   
   - Element.textContent (Element.textContent dapat kita gunakan untuk mengubah teks di dalam sebuah element).
   
                           .textContent = "<span>Teks Heading</span"
                              

   - Element.innerHTML (Element.innerHTML dapat kita gunakan untuk mengubah konten HTML di dalam sebuah element).
                        
                           .innerHTML = "<span>Teks Heading</span"
                              
                              
                              
## Berbagai HTML DOM Events (Interaksi User)
   
User experience itu bersifat dua arah selain menampilkan element HTML, halaman web juga harus bisa menangkap interaksi user, EventListener:
   
- Focus
- Change
- Hover   
- Click (Misalkan kita mempunyai element <input id=”user-input” />  dan <button id=”alert-button”>show</button>. Kita ingin menampilkan pop up box yang berisi teks di dalam input tadi).

- Blur ("Blur", lawan dari "focus", adalah event di mana sebuah element kehilangan fokus dari user (misal user klk mouse di luar element tersebut atau user klik tab untuk berpindah element)

- Scroll
- Submit 
   
Misalkan kita mempunyai element beberapa input dalam sebuah form <input name=”email /> dan <input type=”password” name=”password” />. Bagaimana caranya  kita mendapatkan isi dari kedua input tersebut saat submit form? Pasang event listener di form, lalu gunakan FormData untuk mengambil data dari masing-masing input
   
   
                  const form = document.getElementById("form")

                  form.addEventListener("submit", function(event) {
	                 // cegah page refresh
	               event.preventDefault()

               	const formData = new FormData(form)
	               const values = Object.fromEntries(formData) // { email: ... }
                  }


   
## Menangkap Interaksi User
   
- Element.addEventListener("event")
- Element.onevent

                              
