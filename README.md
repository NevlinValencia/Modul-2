2A
Program ini dapat mengubah tiga string input pengguna. Ini juga dapat menunjukkan apakah tahun input pengguna termasuk tahun kabisat atau tidak.
Program ini menghitung volume dan luas permukaan bola berdasarkan radius jari jari (jari jari) pengguna. Ini juga dapat mengubah suhu celsius pengguna menjadi reamur, kelvin, dan Fahreinheit. Ini juga dapat mengubah dua baris input pengguna: baris pertama berisi lima data integer yang akan dicetak dalam format karakter, dan baris kedua berisi tiga data char yang akan dicetak +1 setelah masing-masing char.

2B
Program ini dapat mencetak jumlah n yang dimasukkan oleh pengguna, dan kemudian meminta pengguna untuk memasukkan nama bunga sebanyak n juga, yang kemudian dirangkai dengan "-" sesuai dengan jumlah yang dimasukkan. Program ini juga dapat memverifikasi bahwa empat urutan warna yang dimasukkan pengguna sudah sesuai dengan yang seharusnya, jika sudah muncul boolean true dan sebaliknya.
Program ini menghitung total beban minimal dan perbedaan beban kanan dan kiri untuk mengetahui apakah beban yang dibawa Pak Andi akan membuat motor oleng. Ini dilakukan dengan nilai akar 2 dari jumlah input user.

2C
Untuk menghitung biaya pengiriman, program ini meminta pengguna mengetikkan berat paket dalam gram. Kemudian, berat total dibagi dengan 1000, dan biaya dasar dihitung berdasarkan berat kilogram, dengan biaya 10.000 untuk setiap kilogram. Kemudian, program ini menampilkan nilai akhir mata kuliah.
Apa hasil program jika nam 80.1 diberikan? Apakah program tersebut dilaksanakan sesuai dengan spesifikasi soal? Karena ketidakkonsistenan program, terutama pada variablel nam, program dideklarasikan sebagai float64, tetapi program mencoba mengassign string (seperti "A", "AB", dll.) ke nam dalam blok if.

Apa yang membuat program gagal? Mengapa hal ini terjadi? Jelaskan bagaimana program seharusnya berjalan! Jawaban: Ada kesalahan dalam program:

Tidak konsisten, program mencoba memasukkan string (seperti "A", "AB", dll.) ke nam dalam blok if, tetapi variablel nam dideklarasikan sebagai float64.
Kondisi if independen, sehingga beberapa blok if akan dieksekusi secara berurutan jika nam lebih besar dari beberapa batas, dan nilai akhir nmk akan ditimpa beberapa kali.
Sebagai contoh, jika nam = 80, maka semua kondisi berikut akan terpenuhi: nam lebih dari 80 akan menghasilkan nmk = "A", nam lebih dari 72,5 akan menghasilkan nmk = "AB", nam lebih dari 65 akan menghasilkan nmk = "B", nam lebih dari 57,5 akan menghasilkan nmk = "BC", nam lebih dari 50 akan menghasilkan n

Perbaikan dalam Program:
Untuk setiap kondisi, ganti nam = "A" dengan nmk = "A".
Untuk memastikan bahwa hanya satu kondisi terpenuhi dan mencegah nilai nmk terpengaruh oleh kondisi berikutnya, gunakan else if.
Program harus diperbaiki! Dengan masukan 93.5; 70.6; dan 49.5, keluaran yang diharapkan adalah 'A', 'B', dan 'D'. Jawabannya adalah bahwa masukan 93.5 menghasilkan output A, masukan 70.6 menghasilkan output B, dan masukan 49.5 menghasilkan output D.

3. Program ini mencari faktor-faktornya untuk memverifikasi apakah jumlah inputan pengguna, termasuk jumlah prima, benar atau tidak.






 
 
