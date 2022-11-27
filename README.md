
# PRAKTIKUM 5
## Program
dibawah ini adalah program sederhana untuk membuat daftar nilai mahasiswa dengan mnggunakan **Dictionary**, dan menampilkan pilihan **Menu** Tambah, Ubah, Hapus, Cari, dan Lihat.
![img1](image/1.png)
![img2](image/2.png)
![img3](image/3.png)
## Flowchart
Dan berikut adalah tampilan dari flowchartnya :
![img4](image/4.png)
## Penjelasan
- Mendeklarasikan Dictonary kosong dengan synatax
`data = {}`
- Lalu membuat perulangan while dan untuk menginisialkan penambahan menu pilihan Tambah, Ubah, Hapus, Cari, Lihat, dan Keluar :
```py
while True:
    x = input("(T)ambah, (U)bah, (H)apus, (C)ari, (L)ihat, (K)eluar: ")
```
## Menambahkan Data
- Berikut adalah Syntax untuk menambahkan data dengan ketentuan jika kita mengetikkan `T` pada keyboard, maka akan melakukan penambahan data dan ditampung kedalam Dictonary `data` yang telah kita buat, dengan nama sebagai `keys` dan yang lainnya sbagai values.
```py   
    if x.lower() == 't':
        print("Tambah Data")
        nama = input("Nama           : ")
        nim = int(input("NIM            : "))
        uts = int(input("Nilai UTS      : "))
        uas = int(input("Nilai UAS      : "))
        tugas = int(input("Nilai Tugas    : "))
        n_akhir = tugas * 0.30 + uts * 0.35 + uas * 0.35
        data[nama] = nim, uts, uas, tugas, n_akhir
```
## Mengubah Data
- Printah dijalankan jika input yang dimasukkan adalah `U`, di dalam kondisi ini terdapat input dan kondisi, dimana jika input `nama` ada didalam variabel `data` maka akan muncul beberapa pilihan untuk mengubah semua data atau data tertentu saja.
- Jika input yang dimasukkan adalah `U`, di dalam kondisi ini terdapat input dan kondisi, dimana jika input `nama` ada didalam variabel `data` maka akan muncul beberapa pilihan untuk mengubah semua data atau data tertentu saja.
    ```py    
    elif x.lower() == 'u':
        print("Ubah Data")
@@ -88,7 +88,7 @@ while True:
## Melihat Data
- Selanjutnya adalah kode yang digunakan untuk melihat input yang sudah dimasukkan.
- Data dalam perulangan `for` di ambil dari variabel Dictionary `data` pada bagian value yang berbntuk list. variabel `i` digunakan untuk membuat nomer. Data yang akan ditambilkan adalah **Nama, NIM, Nilai Tugas, UTS, UAS** dan **Nilai Akhir**
- Data dalam perulangan `for` di ambil dari variabel Dictionary `data` pada bagian value yang berbntuk list. variabel `i = 0` digunakan untuk membuat nomer. Data yang akan ditambilkan adalah **Nama, NIM, Nilai Tugas, UTS, UAS** dan **Nilai Akhir**
    ```py
    elif x.lower() == 'l':
        if data.items():
@@ -127,4 +127,25 @@ Perulangan diatas adalah perulangan yang akan berjalan terus menerus dan akan be
    else:
        print("Pilih Menu Yang Tersedia")
```
```
## Hasil Output
- Apabila program dijalankan maka akan menghasilkan output sebagai berikut :
 - Menambahkan Data dengan input `T` dan melihat data dengan input `L`
 ![img4](image/o1.png)
 - Mengubah Data dengan input `U` dan melihat data dengan input `L`
 ![img5](image/o2.png)
 - Menghapus Data dengan input `H` dan melihat data dengan input `L`
 ![img6](image/o3.png)
 - Mencari Data dengan input `C`
 ![img7](image/o4.png)
 - Keluar dari program dengan input `K`
 ![img8](image/o5.png)
# **Thank you may be useful** 
