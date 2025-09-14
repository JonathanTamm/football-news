Jelaskan mengapa kita memerlukan data delivery dalam pengimplementasian sebuah platform?
# Data delivery sangat penting karena seluruh proses pertukaran informasi antara server dan pengguna terjadi melalui mekanisme ini. Tanpa ini, data tidak bisa diakses atau diperbarui secara real-time sehingga aplikasi tidak dapat menampilkan informasi yang akurat. Data delivery juga memastikan integrasi antar layanan berjalan lancar, baik itu ke aplikasi mobile maupun web. Jadi, keberadaan data delivery menjadi kunci agar platform dapat berfungsi secara konsisten, aman, dan responsif.

Menurutmu, mana yang lebih baik antara XML dan JSON? Mengapa JSON lebih populer dibandingkan XML?
# Menurut saya, JSON lebih baik untuk dunia modern saat ini. JSON memiliki struktur yang lebih ringkas, mudah dibaca manusia, dan parsingnya lebih cepat dibandingkan XML. JSON juga mendukung tipe data seperti angka, boolean, array, dan objek yang lebih natural untuk dipetakan ke bahasa pemrograman yang populer saat ini. Dalam aplikasi web juga JSON jauh lebih praktis dibandingkan XML.

Jelaskan fungsi dari method is_valid() pada form Django dan mengapa kita membutuhkan method tersebut?
# Method is_valid() digunakan untuk memeriksa apakah data yang dikirim melalui form memenuhi semua aturan yang sudah didefinisikan. Dengan memanggil method is_valid(), Django akan ngecek tipe data, panjang input, dan logika lain yang kita tentukan. Jika valid, kita bisa mengambil data bersih melalui cleaned_data. Tanpa pemanggilan method ini, ada risiko data tidak valid atau berbahaya masuk ke database.

Mengapa kita membutuhkan csrf_token saat membuat form di Django? Apa yang dapat terjadi jika kita tidak menambahkan csrf_token pada form Django? Bagaimana hal tersebut dapat dimanfaatkan oleh penyerang?
# csrf_token berfungsi untuk melindungi aplikasi dari serangan Cross-Site Request Forgery (CSRF). Token ini memastikan setiap permintaan benar-benar berasal dari halaman kita, bukan dari situs lain. Jika kita tidak menambahkan csrf_token, orang yang berniat jahat bisa membuat situs palsu yang diam-diam mengirim permintaan data ke server kita dengan memanfaatkan cookie milik korban, misalnya untuk menghapus data atau mengubah password tanpa sepengetahuan pemilik akun. Dengan token ini, server dapat memverifikasi bahwa permintaan aman dan asli.

Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step (bukan hanya sekadar mengikuti tutorial).
# Dimulai dengan menambahkan empat fungsi views baru agar data bisa dilihat dalam format XML, JSON, juga XML dan JSON berdasarkan ID tertentu. Setelah itu saya membuat routing URL di urls.py agar setiap view tadi bisa diakses lewat alamat yang tepat. Langkah berikutnya saya membuat halaman utama yang menampilkan semua data berita dan menambahkan tombol Add untuk pindah ke halaman form, serta tombol Detail pada setiap berita agar bisa membuka halaman detailnya. Setelah halaman utama selesai, saya membuat halaman form create_news.html untuk menambahkan berita baru ke dalam database. Lalu saya menyiapkan halaman news_detail.html yang menampilkan detail lengkap dari setiap berita ketika tombol Detail diklik. Setelah semua fitur itu selesai, saya menguji satu per satu untuk memastikan semuanya berjalan lancar dan akhirnya menjawab pertanyaan yang diminta pada README di folder utama.

Apakah ada feedback untuk asdos di tutorial 2 yang sudah kalian kerjakan?
# Ya, asdos sangat responsif dan sangat baik dalam menjelaskan tutorial 2 ketika kita bertanya.

XML
![alt text](image.png)

JSON
![alt text](image.png)

XML by ID
![alt text](image.png)

JSON by ID
![alt text](image.png)
