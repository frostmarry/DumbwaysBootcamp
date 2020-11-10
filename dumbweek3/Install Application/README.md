# INSTALL APPLICATION

- Sebelumnya install docker-compose karena docker dan docker-compose adalah 2 aplikasi yang berbeda.
```
sudo curl -L "https://github.com/docker/compose/releases/download/1.27.4/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose

sudo chmod +x /usr/local/bin/docker-compose

docker-compose --version

```

- Membuat file `docker-compose.yml` dengan isi seperti berikut

Untuk backend:

![text](asset/1.png)


Untuk frontend:

![text](asset/3.png)

- Menjalankan docker compose dengan perintah 

```
docker-compose up -d
```

backend:

![text](asset/2.png)


frontend:

![text](asset/4.png)

- Cek apakah docker compose sudah berjalan menggunakan `docker ps`

![text](asset/5.png)