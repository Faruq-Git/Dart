1. Error ini terjadi karena adanya konflik nama atau ambiguitas. Kompiler Dart bingung menentukan method toInt() mana yang harus dipanggil pada variabel angka (yang bertipe String), karena ada dua extension berbeda (StringNumber dan StringDouble) yang sama-sama mengimplementasikan method bernama toInt() untuk tipe target yang sama (String). Dart tidak menggunakan tipe kembalian (return type) untuk membedakan pemanggilan method yang ambigu.

Solusi: Memanggil Extension Secara Eksplisit dengan cara membungkus variabel menggunakan nama extension yang ingin digunakan secara spesifik. Cara ini mirip seperti melakukan casting atau memanggil constructor.
https://dartpad.dev/08689b4451cba256f0a1a510573f0247

2. Di dalam bahasa pemrograman Dart, hak akses private bersifat library-private, bukan class-private. Artinya, semua variable atau method yang diawali dengan tanda garis bawah (_) hanya dapat diakses oleh kode yang berada di dalam file (library) yang sama.

Solusi: Satukan di File yang Sama pastikan deklarasi class Counter, extension CounterStats, dan fungsi main() berada di dalam satu file yang sama (misalnya main.dart). Karena berada di library yang sama, extension secara otomatis legal untuk mengakses _value.
https://dartpad.dev/8f8e663e819b8b93d7f00fe5abe5c325
