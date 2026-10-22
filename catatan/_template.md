# Catatan Minggu 02: Class, Object, dan Encapsulation

## Yang saya kerjakan
Saya melengkapi class Aset pada file Aset.java dengan membuat field private, konstruktor, getter, dan setter. Saya juga menambahkan validasi agar kode dan nama aset tidak boleh kosong atau null, serta status dan kondisi tidak boleh null. Selain itu, saya menetapkan nilai awal status menjadi TERSEDIA dan kondisi menjadi BAIK. Setelah selesai mengubah kode, saya menjalankan pengujian untuk minggu ke-2.

## Keputusan desain
Saya menggunakan akses private pada semua field agar data di dalam class Aset tidak dapat diakses secara langsung dari luar class. Saya menyediakan getter untuk membaca data dan setter untuk mengubah nama, status, serta kondisi. Saya tidak membuat setter untuk kode karena kode aset tidak boleh diubah melalui setter. Saya juga menggunakan IllegalArgumentException untuk menolak nilai yang tidak sesuai dengan ketentuan.

## Kendala
Kendala yang saya alami adalah error karena menggunakan tipe data KondisiAset yang tidak ditemukan oleh compiler.Cara mengatasinya dengan mengganti tipe tersebut menjadi Kondisi,Saya menjalankan perintah .\scripts\uji.ps1 -Minggu 2 dan mendapatkan hasil BUILD SUCCESS, dengan 11 tes dijalankan serta tidak ada kegagalan maupun error.

## Penggunaan AI
-Alat yang dipakai: ChatGPT.

Bagian yang dibantu AI: memahami tugas minggu ini serta pemeriksaan error saat menjalankan pengujian.

Prompt utama:

"Bantu saya memahami tugas minggu ini."

"Bantu saya memastikan hasil pengujian minggu ke-2 sudah benar."

Yang saya ubah atau tolak dari saran AI, dan alasannya:
 Saya memperbaiki nama tipe data dari KondisiAset menjadi Kondisi sesuai dengan tipe data yang tersedia.

Satu hal yang saya pahami lebih baik sekarang: Saya lebih memahami penggunaan private, getter, setter, dan validasi pada class. Saya juga memahami bahwa script pengujian perlu dijalankan dengan nomor minggu yang sesuai agar tes minggu ke-2 ikut dijalankan.