Extention Methode

Slide 1: Review Sesi 8 – Builder Pattern

Builder Pattern untuk objek kompleks

Method chaining untuk fluent API

Contoh: Pizza.builder().size('large').addTopping('cheese').build()

Contoh cepat: https://dartpad.dev/1377b9918487bc7336dee694090814e2

Pengantar Extension Methods

Apa itu? Fitur untuk menambahkan metode baru ke tipe yang sudah ada

Tanpa modifikasi kode asli

Tersedia sejak Dart 2.7

Analog: Memberikan kemampuan baru tanpa mengubah benda aslinya

Masalah Tanpa Extetion Methode: https://dartpad.dev/feda307fc75fbc7d11f04b2adec84a76

Solusi Dengan Extention Methode: https://dartpad.dev/0c75e3577ce883fa1d27f16843c1b430

Sintaks Extention Methode: https://dartpad.dev/d14b66ba7f27b34de68d481f5b7e82a4

Tipe yang Bisa Di-extend

1. Built-in types: String , int , double , List , Map , etc.

2. Custom classes: Kelas buatan sendiri

3. Generic types: List<T> , Map<K, V>

4. Nullable types: String? , int?

https://dartpad.dev/6587b9e076a3f406f8397db8409e0d31

Extension untuk Null Safety: https://dartpad.dev/769760501ff93a6de23379e33ffb49b4

Utilities Untuk Dart Types: https://dartpad.dev/3bda435140e007cab0e2bece06adc04d

Generic Extentions: https://dartpad.dev/40dc0567e4bea596de508c72f79255bb

Unnamed Extensions

Extension tanpa nama (hanya untuk library yang sama)

https://dartpad.dev/47b3d3d69c7e4e6aacb3b5a77c43e33c

Konflik Nama Extension

Jika ada multiple extensions dengan nama method sama

https://dartpad.dev/a04a9c110b9967c3d3efe5c9486c64ba

Extention Untuk Custom Classes: https://dartpad.dev/2443b71685e9434bf71147807f16b427

Validator Extention: https://dartpad.dev/6c0d24fe2be7f7a938dcc44fcf962ec6
