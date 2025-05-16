## a. How much data your publisher program will send to the message broker in one run?
 Jumlah data yang dikirim oleh program publisher ke message broker dalam satu kali run bergantung pada banyaknya pesan yang diproduksi. Jika hanya satu pesan yang dikirim, data yang terkirim adalah ukuran pesan tersebut. Namun, jika publisher mengirim banyak pesan secara berurutan atau dalam batch, total data adalah jumlah semua pesan yang dikirim. Dengan kata lain, semakin banyak pesan, semakin besar data yang dikirim dalam satu run. Jadi, total data adalah akumulasi dari semua pesan yang dikirim selama eksekusi.

## b. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean?
URL “amqp://guest:guest@localhost:5672” yang sama pada publisher dan subscriber berarti keduanya terhubung ke message broker yang sama. Broker ini berada di alamat dan port yang identik. Keduanya juga menggunakan kredensial yang sama, yaitu username dan password “guest”. Publisher mengirim pesan ke broker tersebut, sementara subscriber menerima pesan dari broker yang sama. Dengan begitu, komunikasi antara publisher dan subscriber terjadi melalui broker yang sama.

### Running RabbitMQ as message broker.
![image](static\images\image.png)
