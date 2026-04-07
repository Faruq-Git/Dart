# Polimorfisme dan Abstraksi

1. pewarisan
   pewarisan memiliki 3 bentuk diantaranya:
     
   -Inheritance: extends keyword
   
   -super(): digunakan untuk memanggil constructor parent
   
   -@override: untuk override method
   
contoh kode:https://dartpad.dev/cbc53038c8c3f6ddc0b6691faf2d35f7

3. Pengantar Polimorfisme:
   Polimorfisme berarti "banyak bentuk" (poly = banyak, morph = bentuk)
   secara konsep: objek dari subclass dapat diperlakukan sebagai objek dari superclass
   contoh: semua Kucing, Anjing, Burung adalah Hewan
   
   Tipenya berupa:

   -i. Compile-time polymorphism: method overloading (tidak didukung Dart)
  
   -ii. Runtime polymorphism: Method overriding (didukung Dart)

4. Polimorfisme dengan inheritance
   Referensi tipe parent dapat menampung objek child
   
contoh kode: https://dartpad.dev/bfb5bcc5f3086c4138ae44ee79587ec7

5. Manfaat Polimorfisme

      -fleksibelitas: kode dapat bekerja dengna berbagai tipe
   
      -extensibility: mudah menambah tipe baru
   
      -code reusability: method umum di superclass
   
      -maintainability: perubahan mudah dikelola

6. is dan as Operator

   -is berfungsi untuk mengecek tipe objek

   -as berfungsi untuk casting tipe objek
   
contoh kode:https://dartpad.dev/6f75bffd60038612a0be1dde6f77cc7e

7. Pengantar Abstraksi
   
   Konsep: menyembunyikan detail implementasi, hanya menunjukkan fungsionalitas.
   
   hal ini bertujuan untuk:
   
   -i. fokus pada "apa" bukan "bagaimana"
   
   -ii. kontrak yang harus dipenuhi
   
   -iii. fleksibilitas implementasi
   
   caranya di Dart: abstract class dan interface

8. Abstract class
   
   -tidak bisa diinstansiasi langsung
   
   -dapat memiliki method abstract (tanpa implementasi) dan concrete (dengan implementasi)
   
contoh kode:https://dartpad.dev/adbaae6d1d85a780d28dd7ac57a4ba2a

9. Abstract method
   
   -method tanpa body (implementasi)
   
   -harus di override di subclass
   
contoh kode:https://dartpad.dev/aba44c19d5cbab422c6500b367a062f9

10. interface di Dart
    
    -fakta: sejak Dart 3.0 dart punya keyword interface
   
    -cara: semua interface class adalah implicit interface
   
    -gunakan implements untuk mengimplementasi interface
   
contoh kode:https://dartpad.dev/1c69bfc591778f5dec26dde890f8a3a9

11. perbedaan extends vs implements
    
    -hubungan: "is-a". "can-do"
    
    -inheritance: mewarisi implementasi. hanya kontrak
    
    -method: bisa concrete/abstract. semua harus di-implement
    
    -single: ya (single inheritance). banyak (multiple)

12. static members dan method
    
    static members adalah properti atau method yang dimiliki oleh class itu
    sendiri, bukan oleh objek class. Static member diakses langsung melalui
    class name.
    
    Properti dan method static sangat berguna untuk membuat utility class
    atau menyimpan konstanta yang terkait dengan class, sehingga dapat diakses
    langsung tanpa perlu membuat objek.
    
contoh kode:https://dartpad.dev/c82b94545ad93e1ef2bd526cbbb70ff4

bonus 1: https://dartpad.dev/cefa127080f0cbd9075477fd17b11fad

bonus 2: https://dartpad.dev/b1cce22bc70fdce00e0dfb45b1fdf6b4
