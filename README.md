
# PRAKTIKUM 5
## Program
dibawah ini adalah program sederhana untuk membuat daftar nilai mahasiswa dengan mnggunakan **Dictionary**, dan menampilkan pilihan **Menu** Tambah, Ubah, Hapus, Cari, dan Lihat.

!<img width="520" alt="1" src="https://user-images.githubusercontent.com/115879313/204342417-5301a33e-e438-434e-bd93-49e9496ac765.png">
!<img width="519" alt="2" src="https://user-images.githubusercontent.com/115879313/204342731-238e21da-aae2-4c6b-9594-e2def546f12d.png">
!<img width="520" alt="3" src="https://user-images.githubusercontent.com/115879313/204342796-65d236a2-92a9-4989-b411-6248735cca92.png">
## Flowchart
Dan berikut adalah tampilan dari flowchartnya :
!<img width="217" alt="4" src="https://user-images.githubusercontent.com/115879313/204343059-d8ae9c51-a6ae-4813-b1ea-b47171a9dbd8.png">
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
 ![hasil1](https://user-images.githubusercontent.com/115879313/204343239-d3ea81ee-a64b-4832-9d34-69c3437d3277.jpg)
 - Mengubah Data dengan input `U` dan melihat data dengan input `L`
 ![hasil2](https://user-images.githubusercontent.com/115879313/204343284-34e43d67-76d7-4635-84d9-b57b07f4dca1.jpg)
 - Menghapus Data dengan input `H` dan melihat data dengan input `L`
 ![hasil3](https://user-images.githubusercontent.com/115879313/204343340-e923d146-dc6a-4a09-8e7c-8f4b7422336b.jpg)
 - Mencari Data dengan input `C`
 ![hasil4](https://user-images.githubusercontent.com/115879313/204343401-ea6ab43a-7632-4aeb-a5c9-062adf543b2e.jpg))
 - Keluar dari program dengan input `K`
 ![hasil5](https://user-images.githubusercontent.com/115879313/204344250-d3cd17ab-56b0-49f5-a46d-e0a936c58680.jpg)
# **Thank you may be useful** 
