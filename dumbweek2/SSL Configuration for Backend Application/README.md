# SSL CONFIGURATION

- Karena pada server public saya sudah ada certbot, maka saya hanya perlu mengaktifkan let's encrypt pada server backend melalui certbot seperti saat saya mengaktifkan SSL pada server frontend.

![text](asset/1.png)
![text](asset/2.png)

- Tes akses ke website https://api.elga.instructype.com dan cek SSl certificate

![text](asset/3.png)

- Ubah configurasi api pada server frontend dalam directory `dumbplay/frontend/src/config/` 

![text](asset/4.png)

- Tes login dari https://elga.instructype.com menggunakan user yang sudah ditambahkan saat proses `reverse proxy backend`

![text](asset/5.png)
![text](asset/6.png)

