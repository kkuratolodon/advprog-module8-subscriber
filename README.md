# Understanding subscriber and message broker.

- **what is amqp?**
  
    AMQP adalah singkatan dari Advanced Message Queuing Protocol, yang merupakan protokol jaringan yang dirancang untuk memfasilitasi pertukaran data antara sistem yang terpisah. Protokol ini mendefinisikan aturan-aturan mengenai bagaimana format, pengiriman, penerimaan, dan interpretasi data harus dilakukan. Dengan mengimplementasikan AMQP dalam Rust, kita dapat mengembangkan sistem yang efisien untuk komunikasi antar layanan, memungkinkan pertukaran pesan seperti event, request, atau command meskipun penerima tidak tersedia secara langsung atau tidak terhubung secara langsung dengan pengirim. Dengan kata lain, AMQP di Rust memungkinkan aplikasi di sistem yang berbeda untuk saling bertukar data.
    
- **what it means? guest:guest@localhost:5672 , what is the first quest,and what is the second guest, and what is localhost:5672 is for?**
  
    Dalam konfigurasi guest:guest@localhost:5672, "guest" pertama merujuk pada username yang digunakan untuk mengakses server AMQP, sering kali sebagai pengaturan default dalam pemasangan RabbitMQ lokal. "Guest" kedua adalah password yang dikaitkan dengan username tersebut untuk proses autentikasi. "localhost" menunjukkan bahwa server AMQP dijalankan pada mesin lokal, dan "5672" adalah port yang digunakan oleh server AMQP untuk menerima koneksi. Jadi, string ini menginstruksikan aplikasi untuk terhubung ke server AMQP di mesin lokal menggunakan username "guest" dan password "guest" melalui port 5672.
