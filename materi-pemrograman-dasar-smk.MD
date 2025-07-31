# Materi Pemrograman Dasar untuk SMK

## Daftar Isi

1. [Pengenalan Pemrograman](#1-pengenalan-pemrograman)
2. [Algoritma dan Flowchart](#2-algoritma-dan-flowchart)
3. [Variabel dan Tipe Data](#3-variabel-dan-tipe-data)
4. [Operator](#4-operator)
5. [Struktur Kontrol](#5-struktur-kontrol)
6. [Fungsi](#6-fungsi)
7. [Array](#7-array)
8. [Praktik dengan Python](#8-praktik-dengan-python)

---

## 1. Pengenalan Pemrograman

### 1.1 Apa itu Pemrograman?

Pemrograman adalah proses membuat instruksi untuk komputer dalam bentuk kode yang dapat dipahami dan dieksekusi oleh mesin.

### 1.2 Mengapa Belajar Pemrograman?

- **Karir yang Menjanjikan**: Programmer sangat dibutuhkan di era digital
- **Problem Solving**: Melatih kemampuan berpikir logis dan analitis
- **Kreativitas**: Dapat membuat aplikasi, game, website
- **Otomasi**: Mengotomatisasi tugas-tugas repetitif

### 1.3 Bahasa Pemrograman Populer

- **Python**: Mudah dipelajari, serbaguna
- **JavaScript**: Untuk web development
- **Java**: Platform independent
- **C++**: Performance tinggi
- **PHP**: Web development backend

### 1.4 Lingkungan Pengembangan

- **IDE (Integrated Development Environment)**
  - Visual Studio Code
  - PyCharm
  - Sublime Text
- **Compiler/Interpreter**
- **Debugger**

---

## 2. Algoritma dan Flowchart

### 2.1 Definisi Algoritma

Algoritma adalah urutan langkah-langkah logis untuk menyelesaikan suatu masalah.

### 2.2 Karakteristik Algoritma

- **Input**: Memiliki masukan (bisa 0 atau lebih)
- **Output**: Menghasilkan keluaran
- **Definiteness**: Setiap langkah jelas dan tidak ambigu
- **Finiteness**: Memiliki jumlah langkah terbatas
- **Effectiveness**: Setiap langkah dapat dilaksanakan

### 2.3 Contoh Algoritma Sederhana

**Algoritma Membuat Mie Instan:**

1. Siapkan air 400ml
2. Didihkan air
3. Masukkan mie ke air mendidih
4. Tunggu 3 menit
5. Masukkan bumbu
6. Aduk rata
7. Sajikan

### 2.4 Flowchart

Flowchart adalah representasi visual dari algoritma menggunakan simbol-simbol standar.

**Simbol Flowchart:**

- **Oval**: Start/End
- **Persegi Panjang**: Proses
- **Belah Ketupat**: Keputusan
- **Jajar Genjang**: Input/Output
- **Panah**: Alur

**Contoh Flowchart - Menentukan Bilangan Genap/Ganjil:**

```
[START] → [Input bilangan] → [bilangan % 2 == 0?]
    ↓                           ↓YES        ↓NO
[Output "Genap"] ←             ←            → [Output "Ganjil"]
    ↓                                          ↓
[END] ←←←←←←←←←←←←←←←←←←←←←←←←←←←←←←←←←←←←←←←←←←←
```

---

## 3. Variabel dan Tipe Data

### 3.1 Variabel

Variabel adalah tempat untuk menyimpan data yang nilainya dapat berubah selama program berjalan.

**Aturan Penamaan Variabel:**

- Dimulai dengan huruf atau underscore (\_)
- Tidak boleh dimulai dengan angka
- Tidak boleh menggunakan spasi
- Case sensitive (huruf besar/kecil berbeda)
- Tidak boleh menggunakan keyword/reserved words

**Contoh:**

```python
# Valid
nama = "Gilang"
umur = 17
_nilai = 85
namaLengkap = "Gilang Risky"

# Invalid
2nama = "Error"  # Dimulai dengan angka
nama lengkap = "Error"  # Ada spasi
class = "Error"  # Keyword
```

### 3.2 Tipe Data

#### 3.2.1 Tipe Data Primitif

**Integer (Bilangan Bulat):**

```python
umur = 17
jumlah_siswa = 30
suhu = -5
```

**Float (Bilangan Desimal):**

```python
tinggi = 165.5
berat = 55.2
pi = 3.14159
```

**String (Teks):**

```python
nama = "Gilang Risky"
alamat = 'Jakarta'
pesan = "Selamat datang di SMK!"
```

**Boolean (True/False):**

```python
lulus = True
hadir = False
aktif = True
```

#### 3.2.2 Tipe Data Komposit

**List (Array):**

```python
angka = [1, 2, 3, 4, 5]
nama_siswa = ["Andi", "Budi", "Citra"]
campuran = [1, "Dua", 3.0, True]
```

**Dictionary:**

```python
siswa = {
    "nama": "Gilang",
    "umur": 17,
    "kelas": "XII RPL"
}
```

---

## 4. Operator

### 4.1 Operator Aritmatika

```python
a = 10
b = 3

penjumlahan = a + b      # 13
pengurangan = a - b      # 7
perkalian = a * b        # 30
pembagian = a / b        # 3.333...
pembagian_bulat = a // b # 3
sisa_bagi = a % b        # 1
pangkat = a ** b         # 1000
```

### 4.2 Operator Perbandingan

```python
a = 10
b = 5

print(a > b)   # True
print(a < b)   # False
print(a >= b)  # True
print(a <= b)  # False
print(a == b)  # False
print(a != b)  # True
```

### 4.3 Operator Logika

```python
a = True
b = False

print(a and b)  # False
print(a or b)   # True
print(not a)    # False
```

### 4.4 Operator Assignment

```python
x = 10
x += 5   # x = x + 5 → 15
x -= 3   # x = x - 3 → 12
x *= 2   # x = x * 2 → 24
x /= 4   # x = x / 4 → 6.0
```

---

## 5. Struktur Kontrol

### 5.1 Percabangan (If-Else)

#### 5.1.1 If Sederhana

```python
nilai = 85

if nilai >= 75:
    print("Selamat! Anda lulus")
```

#### 5.1.2 If-Else

```python
umur = 17

if umur >= 18:
    print("Anda sudah dewasa")
else:
    print("Anda masih remaja")
```

#### 5.1.3 If-Elif-Else

```python
nilai = 85

if nilai >= 90:
    grade = "A"
elif nilai >= 80:
    grade = "B"
elif nilai >= 70:
    grade = "C"
elif nilai >= 60:
    grade = "D"
else:
    grade = "E"

print(f"Grade Anda: {grade}")
```

### 5.2 Perulangan (Loop)

#### 5.2.1 For Loop

```python
# Menampilkan angka 1-5
for i in range(1, 6):
    print(i)

# Iterasi list
buah = ["apel", "jeruk", "mangga"]
for item in buah:
    print(item)
```

#### 5.2.2 While Loop

```python
# Menampilkan angka 1-5
i = 1
while i <= 5:
    print(i)
    i += 1

# Input sampai benar
password = ""
while password != "12345":
    password = input("Masukkan password: ")
    if password != "12345":
        print("Password salah!")

print("Password benar!")
```

#### 5.2.3 Break dan Continue

```python
# Break - menghentikan loop
for i in range(1, 11):
    if i == 6:
        break
    print(i)  # Output: 1, 2, 3, 4, 5

# Continue - lanjut ke iterasi berikutnya
for i in range(1, 6):
    if i == 3:
        continue
    print(i)  # Output: 1, 2, 4, 5
```

---

## 6. Fungsi

### 6.1 Definisi Fungsi

Fungsi adalah blok kode yang dapat dipanggil berulang kali untuk menjalankan tugas tertentu.

### 6.2 Sintaks Fungsi

```python
def nama_fungsi(parameter):
    # kode fungsi
    return nilai  # opsional
```

### 6.3 Contoh Fungsi

#### 6.3.1 Fungsi Tanpa Parameter

```python
def salam():
    print("Selamat pagi!")

# Memanggil fungsi
salam()  # Output: Selamat pagi!
```

#### 6.3.2 Fungsi Dengan Parameter

```python
def salam_nama(nama):
    print(f"Selamat pagi, {nama}!")

# Memanggil fungsi
salam_nama("Gilang")  # Output: Selamat pagi, Gilang!
```

#### 6.3.3 Fungsi Dengan Return

```python
def luas_persegi(sisi):
    return sisi * sisi

# Menggunakan hasil return
hasil = luas_persegi(5)
print(hasil)  # Output: 25
```

#### 6.3.4 Fungsi Dengan Multiple Parameter

```python
def luas_persegi_panjang(panjang, lebar):
    return panjang * lebar

def biodata(nama, umur, kelas):
    return f"Nama: {nama}, Umur: {umur}, Kelas: {kelas}"

# Pemanggilan
luas = luas_persegi_panjang(10, 5)
bio = biodata("Gilang", 17, "XII RPL")
```

---

## 7. Array (List)

### 7.1 Membuat List

```python
# List kosong
daftar_kosong = []

# List dengan data
angka = [1, 2, 3, 4, 5]
nama = ["Andi", "Budi", "Citra"]
campuran = [1, "Dua", 3.0, True]
```

### 7.2 Mengakses Elemen List

```python
buah = ["apel", "jeruk", "mangga", "pisang"]

print(buah[0])   # apel (index pertama)
print(buah[1])   # jeruk
print(buah[-1])  # pisang (index terakhir)
print(buah[-2])  # mangga (dari belakang)
```

### 7.3 Operasi pada List

#### 7.3.1 Menambah Elemen

```python
buah = ["apel", "jeruk"]

# Menambah di akhir
buah.append("mangga")
print(buah)  # ['apel', 'jeruk', 'mangga']

# Menambah di posisi tertentu
buah.insert(1, "pisang")
print(buah)  # ['apel', 'pisang', 'jeruk', 'mangga']
```

#### 7.3.2 Menghapus Elemen

```python
buah = ["apel", "jeruk", "mangga", "pisang"]

# Menghapus berdasarkan nilai
buah.remove("jeruk")
print(buah)  # ['apel', 'mangga', 'pisang']

# Menghapus berdasarkan index
buah.pop(0)  # Menghapus index 0
print(buah)  # ['mangga', 'pisang']
```

#### 7.3.3 Mengubah Elemen

```python
angka = [1, 2, 3, 4, 5]
angka[2] = 10
print(angka)  # [1, 2, 10, 4, 5]
```

### 7.4 Iterasi List

```python
buah = ["apel", "jeruk", "mangga"]

# Cara 1
for item in buah:
    print(item)

# Cara 2 (dengan index)
for i in range(len(buah)):
    print(f"{i}: {buah[i]}")
```

---

## 8. Praktik dengan Python

### 8.1 Program Kalkulator Sederhana

```python
def kalkulator():
    print("=== KALKULATOR SEDERHANA ===")
    print("1. Penjumlahan")
    print("2. Pengurangan")
    print("3. Perkalian")
    print("4. Pembagian")

    pilihan = input("Pilih operasi (1-4): ")

    if pilihan in ['1', '2', '3', '4']:
        angka1 = float(input("Masukkan angka pertama: "))
        angka2 = float(input("Masukkan angka kedua: "))

        if pilihan == '1':
            hasil = angka1 + angka2
            print(f"Hasil: {angka1} + {angka2} = {hasil}")
        elif pilihan == '2':
            hasil = angka1 - angka2
            print(f"Hasil: {angka1} - {angka2} = {hasil}")
        elif pilihan == '3':
            hasil = angka1 * angka2
            print(f"Hasil: {angka1} × {angka2} = {hasil}")
        elif pilihan == '4':
            if angka2 != 0:
                hasil = angka1 / angka2
                print(f"Hasil: {angka1} ÷ {angka2} = {hasil}")
            else:
                print("Error: Tidak bisa dibagi dengan nol!")
    else:
        print("Pilihan tidak valid!")

# Menjalankan program
kalkulator()
```

### 8.2 Program Pengelola Data Siswa

```python
def kelola_data_siswa():
    siswa = []

    while True:
        print("\n=== PENGELOLA DATA SISWA ===")
        print("1. Tambah Siswa")
        print("2. Lihat Semua Siswa")
        print("3. Cari Siswa")
        print("4. Hapus Siswa")
        print("5. Keluar")

        pilihan = input("Pilih menu (1-5): ")

        if pilihan == '1':
            nama = input("Nama siswa: ")
            kelas = input("Kelas: ")
            nilai = float(input("Nilai: "))

            data_siswa = {
                'nama': nama,
                'kelas': kelas,
                'nilai': nilai
            }
            siswa.append(data_siswa)
            print("Data siswa berhasil ditambahkan!")

        elif pilihan == '2':
            if siswa:
                print("\n=== DAFTAR SISWA ===")
                for i, s in enumerate(siswa, 1):
                    print(f"{i}. Nama: {s['nama']}, Kelas: {s['kelas']}, Nilai: {s['nilai']}")
            else:
                print("Belum ada data siswa.")

        elif pilihan == '3':
            nama_cari = input("Masukkan nama yang dicari: ")
            ditemukan = False
            for s in siswa:
                if nama_cari.lower() in s['nama'].lower():
                    print(f"Ditemukan - Nama: {s['nama']}, Kelas: {s['kelas']}, Nilai: {s['nilai']}")
                    ditemukan = True
            if not ditemukan:
                print("Siswa tidak ditemukan.")

        elif pilihan == '4':
            nama_hapus = input("Masukkan nama siswa yang akan dihapus: ")
            for i, s in enumerate(siswa):
                if s['nama'].lower() == nama_hapus.lower():
                    siswa.pop(i)
                    print("Data siswa berhasil dihapus!")
                    break
            else:
                print("Siswa tidak ditemukan.")

        elif pilihan == '5':
            print("Terima kasih!")
            break
        else:
            print("Pilihan tidak valid!")

# Menjalankan program
kelola_data_siswa()
```

### 8.3 Program Tebak Angka

```python
import random

def tebak_angka():
    print("=== GAME TEBAK ANGKA ===")
    print("Saya memikirkan angka antara 1-100")

    angka_rahasia = random.randint(1, 100)
    percobaan = 0
    max_percobaan = 7

    while percobaan < max_percobaan:
        try:
            tebakan = int(input(f"Percobaan {percobaan + 1}: Masukkan tebakan Anda: "))
            percobaan += 1

            if tebakan == angka_rahasia:
                print(f"Selamat! Anda berhasil menebak angka {angka_rahasia} dalam {percobaan} percobaan!")
                break
            elif tebakan < angka_rahasia:
                print("Terlalu kecil!")
            else:
                print("Terlalu besar!")

            sisa_percobaan = max_percobaan - percobaan
            if sisa_percobaan > 0:
                print(f"Sisa percobaan: {sisa_percobaan}")

        except ValueError:
            print("Masukkan angka yang valid!")

    else:
        print(f"Game Over! Angka yang benar adalah {angka_rahasia}")

# Menjalankan game
tebak_angka()
```

---

## Latihan dan Tugas

### Latihan 1: Algoritma dan Flowchart

Buatlah algoritma dan flowchart untuk:

1. Menghitung luas segitiga
2. Menentukan bilangan terbesar dari 3 bilangan
3. Menghitung faktorial suatu bilangan

### Latihan 2: Program Sederhana

Buatlah program Python untuk:

1. Konverter suhu (Celsius ke Fahrenheit dan sebaliknya)
2. Kalkulator BMI (Body Mass Index)
3. Program untuk menentukan tahun kabisat

### Latihan 3: Fungsi dan Array

1. Buat fungsi untuk menghitung rata-rata dari sebuah list angka
2. Buat fungsi untuk mencari nilai maksimum dan minimum dalam list
3. Buat program untuk mengurutkan list angka dari kecil ke besar

### Tugas Akhir: Project Mini

Buatlah salah satu dari project berikut:

1. **Sistem Perpustakaan Mini**: Program untuk mengelola data buku (tambah, lihat, cari, pinjam, kembalikan)
2. **Aplikasi Kasir Sederhana**: Program untuk menghitung total belanja dengan berbagai item
3. **Game Quiz**: Program kuis dengan multiple choice dan scoring

---

## Tips Belajar Pemrograman

1. **Praktik Rutin**: Coding setiap hari minimal 30 menit
2. **Mulai dari Kecil**: Jangan langsung tackle project besar
3. **Debug dengan Sabar**: Error adalah bagian normal dari coding
4. **Baca Error Message**: Pesan error memberikan petunjuk masalah
5. **Gunakan Komentar**: Dokumentasikan kode Anda
6. **Ikuti Konvensi**: Gunakan naming convention yang konsisten
7. **Join Komunitas**: Bergabung dengan komunitas programmer
8. **Build Portfolio**: Kumpulkan project-project Anda

---

## Sumber Belajar Tambahan

### Website

- [Python.org](https://python.org) - Dokumentasi resmi Python
- [W3Schools Python](https://w3schools.com/python) - Tutorial interaktif
- [Codecademy](https://codecademy.com) - Kursus online interaktif
- [freeCodeCamp](https://freecodecamp.org) - Bootcamp gratis

### YouTube Channels

- Programmer Zaman Now
- Web Programming UNPAS
- Kelas Terbuka
- Sekolah Koding

### Tools Online

- [Repl.it](https://replit.com) - Online Python editor
- [CodePen](https://codepen.io) - Online code editor
- [GitHub](https://github.com) - Version control dan portfolio

---

_Selamat belajar pemrograman! Remember: "The best time to plant a tree was 20 years ago. The second best time is now." - Mulai coding sekarang juga!_ 🚀
