# Praktikum-11

Nama : Syifa Aurellia Rahma

NIM : 312210009

Kelas : TI.22.A1

## Exception Handling
- Exception (eksepsi) merupakan suatu kesalahan (error) yang terjadi saat proses eksekusi program   sedang berjalan
- Kesalahan ini akan menyebabkan program berakhir dengan tidak normal.

## Handling
- Penanganan file adalah bagian penting dari aplikasi apa pun.

## Assertion
Assertion(pernyataan) adalah kewajaran program yang kamu bisa aktif/nonaktifkan ketika kamu selesai menjalankan program.
### The Assert Statement
- Saat menemukan pernyataan, Python mengevaluasi ekspresi yang menyertainya, yang mana semoga benar. Jika ekspresi salah, Python memunculkan pengecualian AssertionError.

#### Sintaks untuk pernyataan yaitu :

assert Expression[, Arguments]

Jika pernyataan gagal, Python menggunakan ArgumentExpression. ArgumentExpression sebagai argumen-argumen untuk AssertionError. 
Pengecualian AssertionError dapat ditangkap dan ditangani seperti pengecualian lainnya menggunakan try kecuali pernyataan, tetapi jika dibiarkan mereka akan menghentikan program dan menghasilkan backtrace.

#### Contoh :
- Berikut adalah fungsi fungsi yang mengubah suhu dari derajat Kelvin menjadi derajat Fahrenheit.Karena nol derajat Kelvin dingin, fungsi fungsi menyimpannya jika melihat negatif negatif suhu.
- Ketika kode di bawah dijalankan, menghasilkan hasil sebagai berikut:

![1](https://user-images.githubusercontent.com/115867244/208573276-4781ff65-7182-449b-baf6-af4f363ac788.png)

## Menangani Pengecualian
Jika Anda memiliki beberapa kode mencurigakan yang mungkin mengeluarkan pengecualian, Anda dapat mempertahankan program Anda letakkan kode yang mencurigakan di *try: blok. Setelah coba: blok, sertakan pernyataan sertakan *except: statement, diikuti oleh blok kode yang menangani masalah seanggun mungkin.

#### Contoh :
- Contoh-contoh ini membuka file, menulis konten file, dan keluar dengan aman karena ada tidak masalah
- Ketika kode di bawah dijalankan, menghasilkan hasil sebagai berikut:

![2](https://user-images.githubusercontent.com/115867244/208574095-1e0eba0a-7a0d-466f-9275-2b285bf025ad.png)

- Contoh ini mencoba membuka file yang Anda tidak memiliki izin menulis, sehingga membuat file pengecualian
- Ketika kode di bawah dijalankan, menghasilkan hasil sebagai berikut:

![3](https://user-images.githubusercontent.com/115867244/208575070-7548bde6-335c-4430-b05b-d7fd7ea1060c.png)

## Fasal kecuali tanpa Pengecualian
- Anda juga dapat menggunakan pernyataan exception tanpa exception yang didefinisikan sebagai berikut:

try: You do your operations here; ...................... except: If there is any exception, 
then execute this block. ...................... else: If there is no exception then execute this block.

Pernyataan coba-kecuali jenis ini menangkap semua pengecualian pengecualian yang terjadi. Menggunakan percobaan seperti try-expect pernyataan tidak dianggap sebagai praktik pemrograman yang baik, karena mereka menangkap semuanya pengecualian tetapi tidak membuat programmer mengidentifikasi kemungkinan penyebab masalah terjadi

## Klausa kecuali dengan Berbagai Pengecualian
- Anda juga dapat menggunakan pernyataan exception yang sama untuk menangani beberapa exception sebagai berikut:

try: You do your operations here; ...................... except(Exception1[, Exception2[,...ExceptionN]]]): If there is any exception from the given exception list, then execute this block. ...................... else: If there is no exception then execute this block.

### Klausa coba-akhirnya 
#### Contoh :
- Jika Anda tidak memiliki izin untuk membuka file dalam mode tulis yang dapat ditulis, maka ini akan menghasilkan hasil berikut:

![4](https://user-images.githubusercontent.com/115867244/208577382-4d341ea3-359a-410f-a0ff-0162eff9874b.png)

- Contoh yang sama dapat ditulis lebih bersih sebagai berikut:

![5](https://user-images.githubusercontent.com/115867244/208577710-b57a2d4b-b742-4c35-b388-642398203632.png)

- Ketika exception dilempar ke dalam blok try, eksekusi segera dilanjutkan ke akhir memblok. Setelah semua pernyataan di blok akhirnya dieksekusi, pengecualian dimunculkan lagi dan ditangani dalam pernyataan kecuali jika ada di lapisan berikutnya yang lebih tinggi dari percobaan-kecuali penyataan.

### Argumen Pengecualian 
#### Contoh :
- Berikut adalah contoh untuk satu pengecualian
- Ketika kode di bawah dijalankan, menghasilkan hasil sebagai berikut:

![6](https://user-images.githubusercontent.com/115867244/208578177-a3d3c6ed-9c5d-4410-ae7f-44ff2635255b.png)

![7](https://user-images.githubusercontent.com/115867244/208578201-413730ff-a2bc-42b0-82cf-c08a38ccc4af.png)

### Melempar Pengecualian 
#### Contoh :
- Pengecualian dapat berupa string, kelas, atau objek. Sebagian besar pengecualian adalah pengecualian dari inti Python menimbulkan adalah kelas dengan argumen=argumen yang merupakan turunan dari kelas. Mendefinisikan pengecualian baru cukup mudah dan dapat dilakukan sebagai berikut:

![8](https://user-images.githubusercontent.com/115867244/208578557-ac4896a5-9061-4aaf-8e29-5e4a4436ebbc.png)

### Pengecualian yang ditetapkan pengguna
- Python juga memungkinkan Anda membuat pengecualian sendiri dengan menurunkan kelas-kelas dari yang standar pengecualian bawaan.
- Berikut adalah contoh-contoh yang terkait dengan RuntimeError. Di sini, kelas dibuat yang merupakan subkelas dari subkelas RuntimeError. Ini berguna saat anda perlu menampilkan tampilan informasi yang lebih spesifik saat e pengecualian tertangkap.
- Di blok try, pengecualian yang ditentukan pengguna dimunculkan dan ditangkap di blok except. Itu variabel e digunakan untuk membuat instance dari kelas Networkerror.

![9](https://user-images.githubusercontent.com/115867244/208579496-ec342bed-e5d2-4476-b9ac-f680f7637c48.png)

## Sekian, Terima kasih
