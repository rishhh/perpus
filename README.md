# Aplikasi Perpustakaan
Aplikasi Perpustakaan ini dijalankan di lingkungan/environment docker. Adapun langkah-langkah untuk menjalankannya, antara lain:

1. Clone repository perpus dan extract file zip tersebut.
2. Jalankan file docker-compose.yml dengan perintah docker-compose up -d, sebelum menjalankan file tersebut pastikan sudah terinstall docker compose
3. Setelah file dijalankan, maka otomatis docker akan membuat 2 container (container web dan container db) sekaligus mencreate database bernama perpus di container db
4. Import file db_perpus.sql ke dalam database perpus dengan perintah docker exec -i root_db_1 mysql -u root -proot --database=perpus < db_perpus.sql
5. Copy folder project perpus ke folder htdocs
6. Jalankan di browser dengan mengetikkan localhost/perpus
