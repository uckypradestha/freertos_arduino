<h1>FreeRTOS pada Arduino</h1>

Real-Time Operating System (biasa di sebut RTOS) adalah sebuah Operating System (OS) yang digunakan untuk memenuhi kebutuhan aplikasi secara Real Time pada Embedded Device yang memproses data secara langsung tanpa ada nya penundaan (Buffer). Real Time karena system ini hampir bekerja setiap saat dimana ia dibutuhkan saat itu juga. Salah satu kelebihan Operating System RTOS adalah kemampuan nya untuk melakukan kerja secara konsisten baik secara waktu yang ia butuhkan maupun secara task aplikasi yang mampu ia kerjakan.

![GITHUB BANNER RTOS](https://github.com/user-attachments/assets/5563312f-66e0-437d-b826-533f07be094d)

RTOS dibutuhkan karena pada system Embedded karena biasa nya pada system Embedded, digunakan sebuah mikrokontroler dengan prosesor tunggal (Single Processor), sehingga pada pekerjaan Embedded System yang membutuhkan system secara Real Time dan melakukan lebih dari satu pekerjaan, dibutuhkan sebuah Operating System yang dapat melakukan penjadwalan (Scheduling) beberapa pekerjaan sehingga dapat dilakukan dalam sebuah prosesor tunggal, dan mudah dimodifikasi untuk melakukan berbagai pekerjaan. Karakter dasar dari Operating System RTOS adalah sebuah sistem yang mempunyai beberapa konsekuensi yang akan berpengaruh pada sistem apabila deadline (batas akhir waktu pelaksanaan sebuah pekerjaan) tidak terpenuhi.

<h2>Prinsip Kerja RTOS</h2>

RTOS memperkenalkan scheduler yang mengelola eksekusi task. Scheduler ini bisa bersifat sederhana maupun kompleks, mulai dari desain rate-monotonic yang sederhana hingga sistem canggih seperti FreeRTOS atau varian Linux real-time tingkat lanjut. Secara cara kerja RTOS seperti yang ditunjukkan pada Gambar

<div align="center">
  <img width="615" height="305" alt="rtos" src="https://github.com/user-attachments/assets/baf05112-4e98-4a51-99f0-deebaab43637" />
</div>

Sebelum mulai bekerja dengan RTOS, mari kita pahami terlebih dahulu apa itu task. Task adalah potongan kode yang dapat dijadwalkan untuk dieksekusi oleh CPU. Jadi, jika Anda ingin menjalankan suatu tugas, maka tugas tersebut harus dijadwalkan menggunakan delay dari kernel atau menggunakan interrupt. Proses ini diatur oleh scheduler yang terdapat di dalam kernel. Pada prosesor single-core, scheduler membantu task untuk dieksekusi dalam potongan waktu tertentu (time slice), sehingga terlihat seolah-olah beberapa task berjalan secara bersamaan. Setiap task dijalankan berdasarkan prioritas yang diberikan kepadanya.

<h2>Instal Library FreeRTOS di IDE</h2>

Untuk install library FreeRTOS di Arduino IDE lakukan langkah-langkah berikut:
1. Buka Arduino IDE, lalu masuk ke menu Sketch → Include Library → Manage Libraries. Setelah itu, cari FreeRTOS dan instal library tersebut seperti yang ditunjukkan di bawah ini.
   <img width="750" height="151" alt="image" src="https://github.com/user-attachments/assets/03ea9037-e65c-4e28-8c2b-e8c6d3eef0ea" />
2. Kita juga dapat mengunduh library dari GitHub, lalu menambahkan file .zip tersebut melalui menu Sketch → Include Library → Add .ZIP Library.
3. Setelah itu, restart Arduino IDE. Library ini menyediakan beberapa contoh program yang bisa Anda temukan melalui File → Examples → FreeRTOS seperti yang ditunjukkan pada Gambar.

<img width="410" height="500" alt="image" src="https://github.com/user-attachments/assets/0c3b55cd-c13b-4867-8977-f169b5c4e224" />

<h2></h2>

<br>
<div align="center">
  <a href="https://github.com/uckypradestha"><img src="https://github.com/uckypradestha/assets/raw/main/social/logo-social-github.png" width="3%" alt="Ultralytics GitHub"></a>
  <img src="https://github.com/uckypradestha/assets/raw/main/social/logo-transparent.png" width="3%" alt="space">
  <a href="https://www.linkedin.com/uckypradestha/"><img src="https://github.com/uckypradestha/assets/raw/main/social/logo-social-linkedin.png" width="3%" alt="Ultralytics LinkedIn"></a>
  <img src="https://github.com/uckypradestha/assets/raw/main/social/logo-transparent.png" width="3%" alt="space">
  <a href="https://twitter.com/uckypradestha"><img src="https://github.com/uckypradestha/assets/raw/main/social/logo-social-twitter.png" width="3%" alt="Ultralytics Twitter"></a>
  <img src="https://github.com/uckypradestha/assets/raw/main/social/logo-transparent.png" width="3%" alt="space">
  <a href="https://www.youtube.com/@ckypradestha"><img src="https://github.com/uckypradestha/assets/raw/main/social/logo-social-youtube.png" width="3%" alt="Ultralytics YouTube"></a>
  <img src="https://github.com/uckypradestha/assets/raw/main/social/logo-transparent.png" width="3%" alt="space">
  <a href="https://www.tiktok.com/@pradestha"><img src="https://github.com/uckypradestha/assets/raw/main/social/logo-social-tiktok.png" width="3%" alt="Ultralytics TikTok"></a>
  <img src="https://github.com/uckypradestha/assets/raw/main/social/logo-transparent.png" width="3%" alt="space">
</div>
