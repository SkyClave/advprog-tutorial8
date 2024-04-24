# Questions

## What is amqp?

AMQP (Advanced Message Queueing Protocol) adakah protokol komunikasi jaringan untuk message oriented middleware. AMQP fokus pada komunikasi process-process antar jaringan dan bergungsi untuk mengirimkan pesan antara komponen-komponen yang berbeda.

## What it means? guest:guest@localhost:5672 , what is the first quest, and what is the second guest, and what is localhost:5672 is for?

guest:guest@localhost:5672 adalah URL yang digunakan untuk melakukan akses messaging broker dengan AMQP. Guest yang pertama menunjukkan username dan guest kedua menunjukkan password. Username dan password ini adalah untuk autentikasi ketika koneksi ke RabbitMQ. Localhost:5672 menunjukkan hostname dan port number dari messaging broker. 5672 merupakan default port number dari RabbitMQ.

## Simulation slow subscriber

![Chart data](/assets/images/photo1.jpg)

Subsrciber dibuat lebih lambat 1 detik dan dapat dilihat dari chart. Terdapat banyak queued message karena menunggu pesan sebelumnya diproses subscriber. Dalam chart terdapat 40+ message lebih dalam queue setelah 10 kali menjalankan publisher.