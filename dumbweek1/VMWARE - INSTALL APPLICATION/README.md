# PROSES INSTALASI SERVER NGINX DAN DEPLOY APLIKASI NODEJS
## Instalasi Nginx
1. Hal pertama yang harus dilakukan setelah instalasi server ubuntu ialah mengupdate dan upgrade paket yang sudah ada dengan perintah `sudo apt update` kemudian dilanjutkan dengan `sudo apt upgrade`. 

![19-20](../asset/19.png)
![19-20](../asset/20.png)

2. setelah proses upgrade selesai barulah install nginx dan jalankan servicenya.

![21-22](../asset/21.png)
![21-22](../asset/22.png)

3. uji coba mengakses server nginx pada komputer lokal dengan cara memasukkan ip server

![23](../asset/23.png)

## Instalasi NodeJS dan deploy dumbplay

1. untuk melakukan instalasi nodejs cukup menjalankan perintah `sudo apt -y install nodejs` dan pastikan yang terinstall adalah versi 10.x

![24-25](../asset/24.png)
![24-25](../asset/25.png)

2. clone repository yang ada pada github.com/sgnd/dumbplay ke server local untuk nantinya dideploy

![26](../asset/26.png)

3. setelah itu cd ke dumbplay/frontend untuk menginstall semua paket yang ada dengan menjalankan perinyah `npm install`

![27](../asset/27.png)

4. selanjutnya jika semua paket terinstall, jalankan perintah `npm start` agar aplikasi bisa diakses pada komputer local

![28-29](../asset/28.png)
![28-29](../asset/29.png)

5. hasil setelah dijalankan pada komputer lokal

![30](../asset/30.png)
