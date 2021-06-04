# Cara Penggunaan
1. Install Docker [Link](https://docs.docker.com/get-docker/)
2. Pastikan Docker sudah terinstall
```console
$ docker -v
Docker version 19.03.1, build 74b1e89e8a
```
3. Clone Repository ini 
```console
$ git clone https://github.com/gymie/dicoding-backend-services.git namaproject
```
4. Jalan docker-compose up -d
```console
$ docker-compose up -d
Creating network "namaproject_default" with the default driver
Creating postgres ... done
Creating redis    ... done
Creating adminer  ... done
```

## Postgres
- USER : developer
- PASSWORD : supersecretpassword

-  Akses CLI Postgres
```console
$ docker exec -it postgres sh
```
- Buat database postgres
```console
/ # createdb -U developer testdb
```
- Connect ke database 
```console
/ # psql -U developer -d testdb
```
- Link Command PSQL [Link](https://www.postgresqltutorial.com/psql-commands/)
