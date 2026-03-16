# Widgets Identification

## 1. `MaterialApp`
Widget utama yang membungkus seluruh aplikasi dengan gaya Material Design.

**Fungsi:**
- Menjadi root aplikasi
- Mengatur tema aplikasi
- Menentukan halaman awal melalui `home`

**Contoh penggunaan:**
```dart
MaterialApp(
  title: 'Flutter Demo',
  theme: ThemeData(
    colorScheme: ColorScheme.fromSeed(seedColor: Colors.deepPurple),
    useMaterial3: true,
  ),
  home: const RowColumnPage(),
)
```

---

## 2. `Scaffold`
Widget dasar yang menyediakan struktur halaman aplikasi.

**Fungsi:**
- Membuat kerangka halaman
- Menyediakan bagian seperti `appBar` dan `body`

**Contoh penggunaan:**
```dart
Scaffold(
  appBar: AppBar(...),
  body: Column(...),
)
```

---

## 3. `AppBar`
Widget yang menampilkan bar di bagian atas halaman.

**Fungsi:**
- Menampilkan judul halaman
- Menjadi bagian header dari tampilan aplikasi

**Contoh penggunaan:**
```dart
AppBar(
  title: const Text('My First App'),
  backgroundColor: Colors.orange[200],
  centerTitle: true,
)
```

---

## 4. `Column`
Widget layout untuk menyusun child secara vertikal dari atas ke bawah.

**Fungsi:**
- Mengatur widget dalam susunan vertikal

**Contoh penggunaan:**
```dart
Column(
  crossAxisAlignment: CrossAxisAlignment.center,
  mainAxisAlignment: MainAxisAlignment.center,
  children: <Widget>[
    ...
  ],
)
```

---

## 5. `Row`
Widget layout untuk menyusun child secara horizontal dari kiri ke kanan.

**Fungsi:**
- Mengatur widget dalam susunan horizontal

**Contoh penggunaan:**
```dart
Row(
  mainAxisAlignment: MainAxisAlignment.spaceEvenly,
  crossAxisAlignment: CrossAxisAlignment.start,
  children: <Widget>[
    ...
  ],
)
```

---

## 6. `Container`
Widget pembungkus serbaguna yang sering digunakan untuk mengatur tampilan dan posisi widget.

**Fungsi:**
- Memberi ukuran
- Memberi warna latar
- Mengatur `margin`
- Mengatur `padding`
- Membungkus widget lain

**Contoh penggunaan:**
```dart
Container(
  width: MediaQuery.of(context).size.width,
  margin: EdgeInsets.fromLTRB(20.0, 5.0, 20.0, 10.0),
  padding: EdgeInsets.all(20.0),
  color: Colors.pink[200],
  child: Text('What image is that'),
)
```

---

## 7. `AspectRatio`
Widget yang menjaga perbandingan lebar dan tinggi child tetap proporsional.

**Fungsi:**
- Menjaga rasio ukuran child
- Pada kode ini digunakan agar area gambar berbentuk 1:1

**Contoh penggunaan:**
```dart
AspectRatio(
  aspectRatio: 1.0,
  child: Container(...),
)
```

---

## 8. `Center`
Widget yang menempatkan child tepat di tengah area yang tersedia.

**Fungsi:**
- Membuat widget berada di posisi tengah

**Contoh penggunaan:**
```dart
Center(
  child: Image.network(...),
)
```