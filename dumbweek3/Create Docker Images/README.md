# CREATE DOCKER IMAGE

- Membuat Dockerfile dengan isi sebagai berikut

![text](asset/1.png)

- Build dengan perintah sebagai berikut

```
docker build -t namaimage:tag .
```

![text](asset/2.png)

- Cek docker images yang sudah dibuild

```
docker images
```

![text](asset/3.png)

- Membuat container dari image yang sudah ada

```
docker create --name namacontainer -p portlocal:portaplikasi namaimage:tag
docker container start namacontainer
```

![text](asset/4.png)
![text](asset/5.png)

NB: pastikan port tidak bentrok dengan aplikasi lain (dalam kasus saya bentrok dengan pm2)

- Cek jika container sudah berjalan dengan `docker ps`

![text](asset/6.png)

- Untuk push image, buat image dengan format akundocker/namaimage:tag dan pastikan sudah login terlebih dahulu. lalu jalankan perintah 

```
docker push namaimage:tag
```

![text](asset/7.png)
![text](asset/8.png)

### Docker Hub saya:

[frostmarry/dumbplay-fe](https://hub.docker.com/repository/docker/frostmarry/dumbplay-fe)

[frostmarry/dumbplay-be](https://hub.docker.com/repository/docker/frostmarry/dumbplay-be)