# Nama: Muhammad Reza Maulana
# Nim: 312210303
# Kelas: TI.22.A3

# Tugas praktikum 5
# Soal

<img width="579" alt="Screenshot 180" src="https://user-images.githubusercontent.com/115542704/202370020-187d2651-fd02-4dbf-b415-670ad56cbbbf.png">

- Buatlah list kosong untuk menampung data-data yang ingin diinputkan

  `data = []`

- Pada program ini saya gunakan perulangan While

  Perulangan while disebut uncounted loop (perulangan yang tak terhitung), yaitu perulangan
yang dilakukan berdasarkan kondisi tertentu selama nilai kondisi bernilai TRUE.

- Kemudian gunakan perintah input() untuk menginput data

```
while True:
    nama = input("Nama : ")
    nim = input("NIM : ")
    tugas = int(input("Nilai Tugas : "))
    uts = int(input("Nilai UTS : "))
    uas = int(input("Nilai UAS : "))
    akhir = (tugas * 30 / 100) + (uts * 35 / 100) + (uas * 35 / 100)
```
    
- Gunakan perintah `.append()` Untuk menambahkan daftar list 

```
 data.append([nama, nim, tugas, uts, uas, int(akhir)])
```

- While disini digunakan untuk melakukan perulangan input ingin menambah data atau tidak (y/t)

```
    more = ""
    while more != "y" and more != "t":
        more = input("Tambah Data(y/t)?")
```

- Perintah if disini digunakan jika data tidak ingin ditambahkan lagi (t), kemudian tambahkan perintah break untuk menghentikan proses perulangan pada kondisi tertentu

```
    if more == "t":
        break
```

- lalu tampilkan daftar datanya

```
print("==================================================================")
print("| No |    Nama      |  NIM  | Tugas |  UTS  |  UAS  |  Akhir |")
print("==================================================================")

i = 0

for nilai in data:
    i += 1
    print("| {no}  | {nama:12s} | {nim:5s} | {tugas:5d} | {uts:5d} | {uas:5d} | {akhir:6.2f} |".format(no=i, nama=nilai[0], nim=nilai[1], tugas=nilai[2],uts=nilai[3],uas=nilai[4],akhir=nilai[5]))

print("==================================================================")
```

# OUTPUT

<img width="427" alt="reza ganteng" src="https://user-images.githubusercontent.com/115516607/202634162-e753245d-e699-4a7e-b543-c434f0b4d608.png">

# Flowchart

<img width="321" alt="Flowchart" src="https://user-images.githubusercontent.com/115516607/202644055-d16bd8a0-9b4f-4811-a483-566d8e06e1b0.png">

## SEKIAN TUTORIAL TERIMAKASIH

