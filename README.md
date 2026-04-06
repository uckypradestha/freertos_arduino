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

