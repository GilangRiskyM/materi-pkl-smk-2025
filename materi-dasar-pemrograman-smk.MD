# Materi Dasar Pemrograman PHP untuk SMK

## Daftar Isi

1. [Pengenalan PHP](#1-pengenalan-php)
2. [Instalasi PHP](#2-instalasi-php)
3. [Sintaks Dasar PHP](#3-sintaks-dasar-php)
4. [Variabel dan Tipe Data](#4-variabel-dan-tipe-data)
5. [Operator](#5-operator)
6. [Struktur Kontrol](#6-struktur-kontrol)
7. [Array](#7-array)
8. [Fungsi](#8-fungsi)
9. [Form dan Pemrosesan Data](#9-form-dan-pemrosesan-data)
10. [Dasar Pemrograman Berbasis Web](#10-dasar-pemrograman-berbasis-web)
11. [Latihan dan Tugas](#11-latihan-dan-tugas)
12. [Sumber Belajar Tambahan](#12-sumber-belajar-tambahan)

---

## 1. Pengenalan PHP

- **PHP** (Hypertext Preprocessor) adalah bahasa pemrograman server-side yang banyak digunakan untuk membuat website dinamis.
- PHP dapat terintegrasi dengan HTML dan database (misal: SQL).
- PHP bersifat open source dan memiliki komunitas besar.

---

## 2. Instalasi PHP

- Cara termudah: Gunakan **Laragon** (Windows), **MAMP** (Mac), atau **LAMP** (Linux).
- Download [Laragon](https://github.com/leokhoa/laragon/releases/download/6.0.0/laragon-wamp.exe), install, lalu setting terlebih dahulu, setelah itu klik start.
- Simpan file PHP di folder `laragon\www\` (untuk Laragon).

---

## 3. Sintaks Dasar PHP

### 3.1 Tag PHP

Kode PHP diawali dengan `<?php` dan diakhiri dengan `?>`.

```php
<?php
    echo "Hello, World!";
?>
```

### 3.2 Menampilkan Output

- `echo` atau `print` untuk menampilkan output ke browser.

```php
<?php
    echo "Selamat datang di Elmuna!";
    print "Belajar PHP itu mudah!";
?>
```

### 3.3 Komentar

- Komentar satu baris: `//` atau `#`
- Komentar banyak baris: `/* ... */`

```php
<?php
    // Ini komentar satu baris
    # Ini juga komentar satu baris
    /*
        Ini komentar
        lebih dari satu baris
    */
?>
```

---

## 4. Variabel dan Tipe Data

### 4.1 Variabel

- Diawali tanda `$` dan nama variabel (tanpa spasi, tidak boleh diawali angka).
- PHP bersifat **loosely typed** (tidak perlu deklarasi tipe data).

```php
<?php
    $nama = "Nama Kamu";
    $umur =  25;
    $tinggi = 170.5;
    $lulus = true;
?>
```

### 4.2 Tipe Data di PHP

- String: `"teks"`
- Integer: `15`
- Float: `3.14`
- Boolean: `true` atau `false`
- Array: `["apel", "jeruk"]`
- Object
- NULL

### 4.3 Contoh Penggunaan Tipe Data

```php
<?php
    $teks = "Elmuna Luar Biasa";
    $angka = 2025;
    $desimal = 7.5;
    $isActive = false;
?>
```

---

## 5. Operator

### 5.1 Operator Aritmatika

| Operator | Keterangan | Contoh   |
| -------- | ---------- | -------- |
| +        | Tambah     | $a + $b  |
| -        | Kurang     | $a - $b  |
| \*       | Kali       | $a \* $b |
| /        | Bagi       | $a / $b  |
| %        | Modulus    | $a % $b  |

### 5.2 Operator Perbandingan

| Operator | Keterangan       | Contoh   |
| -------- | ---------------- | -------- |
| ==       | Sama dengan      | $a == $b |
| !=       | Tidak sama       | $a != $b |
| >        | Lebih besar      | $a > $b  |
| <        | Lebih kecil      | $a < $b  |
| >=       | Lebih besar/sama | $a >= $b |
| <=       | Lebih kecil/sama | $a <= $b |

### 5.3 Operator Logika

| Operator | Keterangan | Contoh   |
| -------- | ---------- | -------- | --- | --- |
| &&       | AND        | $a && $b |
| \|\|     | OR         | $a       |     | $b  |
| !        | NOT        | !$a      |

---

## 6. Struktur Kontrol

### 6.1 Percabangan (if, else, elseif)

```php
<?php
    $nilai = 80;
    if ($nilai >= 75) {
        echo "Lulus";
    } else {
        echo "Tidak lulus";
    }
?>
```

### 6.2 Percabangan dengan elseif

```php
<?php
    $nilai = 85;
    if ($nilai >= 90) {
        echo "A";
    } elseif ($nilai >= 80) {
        echo "B";
    } else {
        echo "C";
    }
?>
```

### 6.3 Switch Case

```php
<?php
    $hari = "Selasa";
    switch ($hari) {
        case "Senin":
            echo "Hari pertama";
            break;
        case "Selasa":
            echo "Hari kedua";
            break;
        default:
            echo "Hari lain";
    }
?>
```

### 6.4 Perulangan

#### For

```php
<?php
    for ($i = 1; $i <= 5; $i++) {
        echo $i . "<br>";
    }
?>
```

#### While

```php
<?php
    $i = 1;
    while ($i <= 5) {
        echo $i . "<br>";
        $i++;
    }
?>
```

#### Do While

```php
<?php
    $i = 1;
    do {
        echo $i . "<br>";
        $i++;
    } while ($i <= 5);
?>
```

#### Foreach (untuk array)

```php
<?php
    $buah = ["apel", "jeruk", "pisang"];
    foreach ($buah as $item) {
        echo $item . "<br>";
    }
?>
```

---

## 7. Array

### 7.1 Array Numerik

```php
<?php
    $angka = [10, 20, 30, 40];
    echo $angka[2]; // 30
?>
```

### 7.2 Array Asosiatif

```php
<?php
    $siswa = [
        "nama" => "Gilang",
        "kelas" => "XII RPL",
        "umur" => 17
    ];
    echo $siswa["kelas"];
?>
```

### 7.3 Array Multidimensi

```php
<?php
    $kelas = [
        ["Andi", 16],
        ["Budi", 17],
        ["Citra", 16]
    ];
    echo $kelas[1][0]; // Budi
?>
```

---

## 8. Fungsi

### 8.1 Membuat dan Memanggil Fungsi

```php
<?php
    function salam() {
        echo "Selamat pagi!";
    }
    salam();
?>
```

### 8.2 Fungsi dengan Parameter dan Return

```php
<?php
    function tambah($a, $b) {
        return $a + $b;
    }
    $hasil = tambah(4, 7); // 11
    echo $hasil;
?>
```

---

## 9. Form dan Pemrosesan Data

### 9.1 Membuat Form HTML

```html
<form action="proses.php" method="post">
  Nama: <input type="text" name="nama" /><br />
  <input type="submit" value="Kirim" />
</form>
```

### 9.2 Menangani Data Form dengan PHP

```php
<?php
// File: proses.php
    $nama = $_POST['nama'];
    echo "Hai, $nama!";
?>
```

### 9.3 Validasi Sederhana

```php
<?php
    if (empty($_POST['nama'])) {
        echo "Nama harus diisi!";
    } else {
        $nama = $_POST['nama'];
        echo "Selamat datang, $nama!";
    }
?>
```

---

## 10. Dasar Pemrograman Berbasis Web

- PHP biasa digunakan bersama HTML, CSS, dan JavaScript.
- PHP berjalan di server, hasilnya dikirim ke browser.
- Untuk menampilkan PHP di browser, simpan file di `laragon\www\` (Laragon).

---

## 11. Latihan dan Tugas

### Latihan

1. Buat program PHP untuk menampilkan biodata sederhana.
2. Buat program menentukan bilangan ganjil/genap.
3. Buat program menghitung luas persegi panjang (input panjang dan lebar dari form HTML).
4. Buat array asosiatif data siswa dan tampilkan semua datanya.
5. Buat fungsi untuk menghitung rata-rata dari array angka.

### Tugas Project Mini

- **Aplikasi Data Siswa Sederhana**  
  Fitur:
  - Input data siswa (nama, kelas, nilai) via form
  - Tampilkan daftar siswa
  - Tampilkan siswa dengan nilai tertinggi

---

## 12. Sumber Belajar Tambahan

- [PHP Manual](https://www.php.net/manual/en/)
- [W3Schools PHP Tutorial](https://www.w3schools.com/php/)

---
