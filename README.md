## Docker Compose


1. Nginx, php 5.6
2. mysql5.6

Untuk membuat database
masuk ke bash container (mysql)
```docker ps
```docker exec -it (nama container) bash
```mysql -u root -p
```(password=mypassword)
Kemudian untuk mengimpor, karena disini saya mendownload aplikasi dari website malasngoding
docker exec -i namakontener mysql -u root -pmypassword --database=malasngoding_kios < malasngoding_kios.sql 

sebagai contoh
docker exec -i 1477ec91e9a7 mysql -u root -proot --database=malasngoding_kios < malasngoding_kios.sql

Untuk scrip docker-compose.yml dan dockerfile bisa dilihat diatas.