# Tugas-Structure-Data-01
# 📄 PENJELASAN KONSEP ARRAY

Array adalah struktur data linear yang menyimpan elemen dengan tipe data yang sama dan disimpan dalam memori yang berurutan. Array biasanya di gunakan untuk menyimpan data sementara yang berukuran kecil, dan Array biasanya di akses menggunakan index.
Array memiliki 3 jenis yaitu Array 1 Dimensi, 2 Dimensi, & Multi Dimensi.

Contoh Array:
```python
import numpy as np

Mobil = np.array([Nissan, Mazda, Toyota])
print(Mobil)
```
# PENJELASAN KONSEP LIST

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
# ANALISIS KOMPLEKSITAS

Berikut adalah analisis kompleksitas pada kode yang sudah saya buat.
 
Soal 1: Input 10 Nilai
```python
nilai_mhs = []
for i in range(10):
    nilai = int(input("Masukkan angka: "))
    nilai_mhs.append(nilai)
```
Loop / Perulangan Pada kode ini berjalan tepat 10 kali. Jumlah input nya tetap, & tidak bergantung pada variabel apapun. karena looping nya berjalan konstan, maka kode ini memiliki kompleksitas O(1).

Soal 2: Nilai Tertinggi dan Terendah
```python
print("Nilai:", nilai_mhs)
print("Nilai maksimum:", max(nilai_mhs))
print("Nilai minimum:", min(nilai_mhs))
```
Function max() & min() bekerja dengan cara melihat satu persatu isi dari array / list untuk mencari yang terbesar dan terkecil.

max() akan looping dari index 0 sampai selesai.

min() juga akan looping dari index 0 sampai selesai.

oleh karna itu kompleksitas dari kode soal kedua ini adalaah O(n).

Soal 3: Rata - Rata
```python
print("Rata-rata:", sum(nilai_mhs)/len(nilai_mhs))
```
Function sum() bekerja dengan cara menjumlahkan semua angka dengan looping dari index 0 sampai selesai.

kompleksitas pada kode ini adalah O(n).

Soal 4: Menghitung lulus & tidak
```python
lulus = 0
tidak_lulus = 0
for nilai in nilai_mhs:          
    if cek_lulus(nilai):          
        lulus += 1
    else:
        tidak_lulus += 1
```
loop ini akan mengakses setiap elemen array 1 kali.
dan kompleksitas pada kode ini adlah O(n).

Soal 5: Chart Nilai Terkecil & Terbesar
```python
import matplotlib.pyplot as plt
nilai_tertinggi = max(nilai_mhs)          
nilai_terendah = min(nilai_mhs)            
```
Bagian ini menghitung nilai terkecil dan terbesar dari nilai yang di input, sama seperti soal kedua, maka kompleksitas dari kode ini adalah O(n).

 Soal 6: Chart Jumlah Mahasiswa lulus & tidak
 ```python
sizes = jumlah_anggota = [mhs_lulus, mhs_tidak_lulus]
```
di dalam kode terakhir ini tidak memiliki perulangan dan data yang di ambil disini adalah dari kode yang sebelumnya maka kompleksitas pada kode ini adalah O(1).

Kompleksitas dari keseluruhan program ini adalah O(n), alasannya adalah karna keseluruhan program ini bergerak linear.

# Screenshoot Hasil run
![Ss Hasil Run](images/Screenshot 2026-03-15 135540.png)
