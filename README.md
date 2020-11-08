# Labspy03
## Kondisi

### Profil
__Nama : Reza Riyaldi Irawan__

__NIM : 312010284__

__Kelas : TI.20.A.2__

### Daftar Isi
| No | ISI | Link | Source Code |
| -- | --- | ---- | ----------- |
| 1. | Latihan 1 | [lihat](https://github.com/RezaRiyaldi/labspy03/new/master?readme=1#latihan1) | [Code](https://github.com/RezaRiyaldi/labspy03/blob/master/latihan1.py) |
| 2. | Latihan 2 | [lihat](https://github.com/RezaRiyaldi/labspy03/new/master?readme=1#latihan2) | [Code](https://github.com/RezaRiyaldi/labspy03/blob/master/latihan2.py) |
| 3. | Program 1 | [lihat](https://github.com/RezaRiyaldi/labspy03/new/master?readme=1#program1) | [Code](https://github.com/RezaRiyaldi/labspy03/blob/master/latihan2.py) |

### Latihan1
Konsep program :
1. Menampilkan n bilangan acak yang lebih kecil dari 0.5.
2. nilai n diisi pada saat runtime

Program Menampilkan n Bilangan Acak Yang Lebih Kecil Dari 0.5
![latihan1](https://github.com/RezaRiyaldi/labspy03/blob/master/gambar/latihan1.png)

Penjelasan

1. Mengimport module `random` untuk membuat bilangan acak
```python
import random
```

2. Untuk menentukan jumlah input yang diinginkan dan dikonversi ke dalam bilangan bulat (integer) yang dimasukan ke variable `jum`
```python
jum = int( input("Masukan nilai n : "))
```

3. Untuk pengulangan range yang diinputkan oleh variable `jum`
```python
for i in range(jum):
```

4. Untuk menampilkan urutan data sesuai jumlah inputan dengan hasil di bawah 0.5
```python
angkaDec = random.uniform(0, 0.5)
    print("Data ke", i, " = ", angkaDec)
```

### Latihan2

Konsep program : 
1. Membuat program untuk menampilkan bilangan terbesar dari n buah data yang diinputkan.
2. Ketika memasukan angka 0 program akan berhenti.

Program Sederhana Untuk Menampilkan bilangan Terbesar dari n buah data yang di Masukkan
![latihan1](https://github.com/RezaRiyaldi/labspy03/blob/master/gambar/latihan2.png)

Penjelasan program

1. Membuat header `print(40*"=")` untuk menampilkan "=" sebanyak 40, begitupun yang `print(5*"=")` untuk menampilkan "=" sebanyak 5
```python
print(40*"=")
print(5*"=","Menentukan bilangan terbesar", 5*"=")
print(40*"=")
```
2. Deklarasi variable
```python
max = 0
```
3. Untuk perulangan hingga waktu yang tidak di tentukan atau selamanya
```pyhton
while True: 
```
4. Untuk menentukan jumlah input yang diinginkan dan dikonversi ke dalam bilangan bulat (integer) yang dimasukan ke variable `a`
```python
 a = int(input("Masukan bilangan : "))
```
5. Jika max kurang dari a maka max = a maka variable max = a atau nilai yang diinputkan
```pyhton
if max < a:
max = a
```
6. Jika a = 0 maka program akan berhenti dengan syarat break yang terpenuhi
```python
if a == 0: 
break 
```
7.  Menampilkan Bilangan Terbesard
```python
print ("Bilangan Terbesar Adalah : ", max) 
```

### Program1

Konsep program : 
1. Seorang pengusaha menginvestasikan uangnya untuk memulai usahanya dengan
modal awal 100 juta, pada bulan pertama dan kedua belum mendapatkan laba. pada
bulan ketiga baru mulai mendapatkan laba sebesar 1% dan pada bulan ke 5,
pendapatan meningkat 5%, selanjutnya pada bulan ke 8 mengalami penurunan
keuntungan sebesar 2%, sehingga laba menjadi 3%. Hitung total keuntungan selama 8
bulan berjalan usahanya.

Program Program Sederhana Menghitung Total Keuntungan Selama 8 Bulan
![latihan1](https://github.com/RezaRiyaldi/labspy03/blob/master/gambar/program1.png)

Penjelasan program
1. Deklarasi variable
```python
modal = 100000000
laba = [modal * 0, modal* 0, modal * 1/100, modal * 1/100, modal * 5/100, modal * 5/100, modal * 5/100, modal * 3/100]
bulan = 0
sum = 0
```
2. Dari variable `laba` terdapat list `modal * 0, modal* 0, modal * 1/100, modal * 1/100, modal * 5/100, modal * 5/100, modal * 5/100, modal * 3/100` yang bermaksud dari bulan pertama - akhir
3. Membuat header `print(39*"=")` untuk menampilkan "=" sebanyak 39, begitupun yang `print(5*"=")` untuk menampilkan "=" sebanyak 5
```python
print(39*"=")
print(5*"=","Menentukan bilangan terbesar", 5*"=")
print(39*"=")
```
4. Menampilkan modal awal menggunakan `f string` pada `{modal}` atau variable modal
```python
print(f"Modal awal pengusaha {modal}")
```
5. Melakukan perulangan yang di masukan kedalam variable `i` dari variable `laba`
```python
for i in laba:
```
6. Variable `i` akan ditambahkan dengan variable `sum`, setiap melakukan perulangan `sum` + `i` sampai program selesai
```python
sum = sum + i
```
7. Untuk menentukan bulan
```python
bulan += 1
```
8. Menampilkan program dengan `f string`
```python
print(f"Laba pada bulan ke - {bulan}, mendapat laba = {i}")
```
9. Hasil akhir
```python
print(f"Keuntungan yang didapat selama {bulan} bulan = {sum}")
```
