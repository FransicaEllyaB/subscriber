# TUTORIAL
---
### Nama  : Fransisca Ellya Bunaren
### NPM   : 2306152286
### Kelas : Adpro B
---
### REFLEKSI
> What is amqp?
AMQP atau Advanced Message Queuing Protocol adalah protokol standar terbuka yang berfungsi untuk komunikasi asinkron antar sistem melalui antrian pesan (message queue). AMQP memungkinkan sistem-sistem yang berbeda saling bertukar data secara andal, bahkan jika salah satu sistem sedang offline.

> What does it mean? guest:guest@localhost:5672,what is the first guest, and what is the second guest, and what is localhost:5672 is for?
`guest:guest@localhost:5672` adalah format umum yang digunakan untuk menyambung ke broker AMQP. Bagian pertama sebelum tanda `@`, yaitu guest:guest merupakan kombinasi dari username dan password—dalam hal ini, username-nya adalah "guest" dan password-nya juga "guest". Setelah tanda `@`, terdapat `localhost:5672` yang menunjukkan bahwa koneksi ditujukan ke komputer lokal (localhost) pada port 5672, yang merupakan port standar yang digunakan untuk komunikasi AMQP. Jadi secara keseluruhan, string ini digunakan untuk mengautentikasi dan menyambung ke server RabbitMQ lokal melalui protokol AMQP.