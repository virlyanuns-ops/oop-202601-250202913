# Catatan Minggu 3: Inheritance

## Yang saya kerjakan
pada tugas minggu ini saya melengkapi tiga class,(ruang.java,Laptop.java, dan Alat.java). dalam pengerjaan ini Saya menambahkan field, konstruktor, getter, dan method getJenis(). Setelah selesai, saya menjalankan pengujian dan berhasil mendapatkan 8 tes tanpa error.

## Keputusan desain
Saya memutuskan bahwa field kode, nama, status, dan kondisi diletakkan di class induk Aset karena field tersebut digunakan oleh semua jenis aset.

Sementara itu, field yang memiliki fungsi khusus diletakkan di masing-masing subclass:
Ruang: kapasitas.

Laptop: spesifikasi dan nomor inventaris.

AlatLab: laboratorium dan tingkat risiko.

Dengan menggunakan inheritance, ketiga class tersebut dapat menggunakan kembali atribut dan validasi dari class Aset, sehingga kode menjadi lebih terstruktur dan tidak perlu menulis ulang bagian yang sama.

Salah satu contoh inheritance yang kurang tepat adalah jika class Laptop dibuat sebagai turunan dari class Baterai. Laptop bukan jenis baterai, tetapi memiliki baterai. Dalam kondisi tersebut, komposisi lebih tepat digunakan.

## Kendala
Kendala yang saya temui adalah PowerShell tidak mengizinkan script pengujian dijalankan karena pengaturan Execution Policy. Saya mengatasinya dengan menjalankan perintah:

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass

Setelah itu, saya menjalankan kembali pengujian Minggu 3 dan proses berhasil diselesaikan dengan status BUILD SUCCESS.
## Penggunaan AI
- Alat yang dipakai: chatGPT
- Bagian yang dibantu AI: Melengkapi dan memahami kode pada class Ruang.java, Laptop.java, dan AlatLab.java, serta memahami konsep inheritance, constructor, super, getter, dan override.


- Prompt utama: Membantu melengkapi kode class Laptop.java sesuai aturan Minggu 3.

Membantu melengkapi kode class Ruang.java dengan validasi kapasitas.

Membantu melengkapi kode class AlatLab.java dengan validasi laboratorium dan tingkat risiko.
- Yang saya ubah atau tolak dari saran AI, dan alasannya:
saya tidak langsung menerima semua saran dari Ai begitu saja, tapi saya juga mencoba memahami alur kode dengan keterangan dari dosen saat di kelas terutama pada bagian penggunaan super(), validasi,getter dan @override
- Satu hal yang saya pahami lebih baik sekarang:
Saya lebih memahami bahwa inheritance digunakan untuk mewariskan atribut dan method dari class induk ke class turunan. Saya juga memahami penggunaan super() untuk memanggil konstruktor induk dan @Override untuk menyesuaikan method pada subclass