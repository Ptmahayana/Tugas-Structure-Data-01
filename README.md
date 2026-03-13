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
