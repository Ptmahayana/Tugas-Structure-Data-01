# Tugas-Structure-Data-01
**📄 PENJELASAN KONSEP ARRAY**

Array adalah struktur data linear yang menyimpan elemen dengan tipe data yang sama dan disimpan dalam memori yang berurutan. Array biasanya di gunakan untuk menyimpan data sementara yang berukuran kecil, dan Array biasanya di akses menggunakan index.
Array memiliki 3 jenis yaitu Array 1 Dimensi, 2 Dimensi, & Multi Dimensi.

Contoh Array:
```python
import numpy as np

Mobil = np.array([Nissan, Mazda, Toyota])
print(Mobil)
```
**PENJELASAN KONSEP LIST**

List adalah struktur data linear yang menyimpan element secara berurutan. Berbeda dengan array, list seringkali dapat menampung tipe data berbeda dan ukurannya fleksibel.

Contoh List:
```python
nama = ["wowok", "owi", "dirga"]
print("List Nama :")
print(nama)
```
Kita juga dapat menambahkan data dengan menggunakan .append() & menghapus data menggunakan .remove().

Contoh Penggunaan .append():
```python
nama.append("bahlil")
print("List Nama :")
print(nama)
#setelah di run maka code ini akan otomatis menambahkan nama yang kita masukan ke dalam list yang sudah kita buat sebelumnya
```
Contoh Penggunaan .remove():
```python
nama.remove("owi")
print("List Nama :")
print(nama)
#setelah di run maka code ini akan menghilangkan salah satu nama dari dalam list
```
**ANALISIS KOMPLEKSITAS**

Berikut adalah analisis kompleksitas pada kode yang sudah saya buat.
 
Soal 1: Input 10 Nilai
```python
nilai_mhs = []
for i in range(10):
    nilai = int(input("Masukkan angka: "))
    nilai_mhs.append(nilai)
```
Loop / Perulangan Pada kode ini berjalan tepat 10 kali. Jumlah input nya tetap, & tidak bergantung pada variabel apapun. karena looping nya berjalan konstan, maka kode ini memiliki kompleksitas 0(1).

Soal 2: Nilai Tertinggi dan Terendah
```python
print("Nilai:", nilai_mhs)
print("Nilai maksimum:", max(nilai_mhs))
print("Nilai minimum:", min(nilai_mhs))
```
Function max() & min() bekerja dengan cara melihat satu persatu isi dari array / list untuk mencari yang terbesar dan terkecil.

max() akan looping dari index 0 sampai selesai.

min() juga akan looping dari index 0 sampai selesai.

oleh karna itu kompleksitas dari kode soal kedua ini adalaah 0(n).

Soal 3: Rata - Rata
```python
print("Rata-rata:", sum(nilai_mhs)/len(nilai_mhs))
```
Function sum() bekerja dengan cara menjumlahkan semua angka dengan looping dari index 0 sampai selesai.

kompleksitas pada kode ini adalah 0(n).

