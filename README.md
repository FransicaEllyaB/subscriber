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

### IMAGES

> Screenshot Simulating Slow Subscriber

Saya menjalankan `cargo run` berkali kali pada publisher dapat dilihat bahwa terdapat 15 message yang berada dalam queue. Peningkatan tajam seperti ini karena subscriber membutuhkan waktu untuk memproses sebuah message sehingga message menjadi menumpuk. Di sisi lain `rabbitmq`, `publisher` mempublish banyak event dalam waktu singkat.

![{80F56319-8EA1-4C66-BE67-57FAF6B3A708}](https://github.com/user-attachments/assets/c433cd9c-c23e-44b2-8ceb-b26c2c10b318)

Screenshot ketika saya menjalankan `cargo run` sehingga menerima message dari `publisher` yang dijalankan beberapa kali.

![image](https://github.com/user-attachments/assets/866f94df-d799-4486-962e-c4f7d9a4bf19)
