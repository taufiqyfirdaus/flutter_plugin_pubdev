# Praktikum 5
**Langkah 1**<br><br>
Buatlah sebuah project flutter baru dengan nama flutter_plugin_pubdev. Lalu jadikan repository di GitHub Anda dengan nama flutter_plugin_pubdev.<br><br>
**Langkah 2**<br><br>
Tambahkan plugin auto_size_text menggunakan perintah flutter pub add auto_size_text<br>
![image](https://github.com/taufiqyfirdaus/flutter_plugin_pubdev/assets/74848393/422cd1b1-2bf8-434b-857b-3b5c0dca4dac)
<br><br>
**Langkah 3**<br><br>
Buat file baru bernama red_text_widget.dart di dalam folder lib lalu isi kode seperti berikut.<br>
![image](https://github.com/taufiqyfirdaus/flutter_plugin_pubdev/assets/74848393/8ec0804a-0656-42dd-b188-01da7ce222ae)
<br><br>
**Langkah 4**<br><br>
Masih di file red_text_widget.dart, untuk menggunakan plugin auto_size_text, ubahlah kode return Container() menjadi seperti berikut.<br>
![image](https://github.com/taufiqyfirdaus/flutter_plugin_pubdev/assets/74848393/a056483b-1828-471a-88ac-c63da853f36a)
<br><br>
**Langkah 5**<br><br>
Tambahkan variabel text dan parameter di constructor seperti berikut.<br>
![image](https://github.com/taufiqyfirdaus/flutter_plugin_pubdev/assets/74848393/6f9a79b9-9535-4d2d-a637-cda7151d886b)
<br><br>
**Langkah 6**<br><br>
Buka file main.dart lalu tambahkan di dalam children: pada class _MyHomePageState<br>
![image](https://github.com/taufiqyfirdaus/flutter_plugin_pubdev/assets/74848393/0ae3b297-130b-4650-bc58-90fc49ffe4f5)<br>
![image](https://github.com/taufiqyfirdaus/flutter_plugin_pubdev/assets/74848393/3b563fd6-8b68-4e19-ac44-47746bd054e6)
<br><br>
**Hasil**<br><br>
![image](https://github.com/taufiqyfirdaus/flutter_plugin_pubdev/assets/74848393/58b963c9-949c-4f14-ba36-ea47870c7dc9)
<br><br>

# Tugas Praktikum 
1. Selesaikan Praktikum tersebut, lalu dokumentasikan dan push ke repository Anda berupa screenshot hasil pekerjaan beserta penjelasannya di file README.md!
2. Jelaskan maksud dari langkah 2 pada praktikum tersebut!
   **jawab:**
   Sintaks flutter pub add auto_size_text digunakan untuk secara otomatis menambahkan paket Flutter bernama "auto_size_text" ke dalam proyek ini.
3. Jelaskan maksud dari langkah 5 pada praktikum tersebut!
   **jawab:**
   Terjadi error pada Langkah 4 karena perubahan yang dilakukan pada red_text_widget.dart memerlukan beberapa perubahan tambahan dalam proyek yaitu kita perlu mengimpor paket auto_size_text ke dalam berkas red_text_widget.dart agar Anda dapat menggunakan komponen-komponen dari paket tersebut dan juga diperlukan untuk menambahkan variabel text di constructor.
4. Pada langkah 6 terdapat dua widget yang ditambahkan, jelaskan fungsi dan perbedaannya!
   **jawab:**
   - **RedTextWidget:**<br>
     **Fungsi :** Fungsinya adalah untuk menampilkan teks dengan warna merah dan menggunakan fitur auto-sizing (mengubah ukuran teks sesuai dengan ruang yang tersedia).<br>
**Perbedaan :** Widget ini khusus dibuat untuk menampilkan teks dengan gaya dan perilaku tertentu, yaitu dengan warna merah, pembatasan maksimal dua baris, dan menggunakan auto-sizing untuk memastikan teks sesuai dengan ruang yang tersedia.
    - **Text Widget:**<br>
      **Fungsi :** Widget Text adalah widget bawaan Flutter yang digunakan untuk menampilkan teks statis. Dalam proyek ini, widget Text digunakan untuk menampilkan teks yang sama dengan yang ditampilkan oleh RedTextWidget, tetapi tanpa gaya khusus atau perilaku auto-sizing.<br>
**Perbedaan :** Widget Text adalah widget dasar yang digunakan untuk menampilkan teks tanpa pengaturan gaya atau perilaku khusus. Kita dapat menambahkan teks apa pun ke dalamnya, tetapi tidak ada perubahan ukuran atau gaya tertentu yang diatur secara otomatis.
5. Jelaskan maksud dari tiap parameter yang ada di dalam plugin auto_size_text berdasarkan tautan pada dokumentasi ini !
   **jawab:**
   - **text (String):**
     Parameter ini adalah teks yang akan ditampilkan oleh AutoSizeText. Ini adalah teks yang akan disesuaikan ukurannya sesuai dengan ruang yang tersedia.
   - **style (TextStyle):**
     Parameter ini digunakan untuk mengatur gaya teks seperti warna, ukuran font, tebal, dan sebagainya. Dalam contoh yang Anda berikan, warna teks diatur menjadi merah dengan ukuran font 14.
   - **maxLines (int):**
     Parameter ini digunakan untuk membatasi jumlah baris maksimal yang akan ditampilkan oleh AutoSizeText. Jika teks melebihi jumlah baris yang ditentukan, teks akan dipotong dengan "..." (elipsis).
   - **overflow (TextOverflow):**
     Parameter ini digunakan untuk menentukan bagaimana teks yang melebihi jumlah baris maksimal (maxLines) akan ditampilkan. TextOverflow.ellipsis digunakan dalam contoh Anda, yang berarti teks yang melewati batas akan ditampilkan dengan elipsis ("...").
6. Kumpulkan laporan praktikum Anda berupa link repository GitHub ke spreadsheet yang telah disediakan!
