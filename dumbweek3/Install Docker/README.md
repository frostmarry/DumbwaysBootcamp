# INSTALL DOCKER

- Menambahkan beberapa paket setelah melakukan update dan upgrade
```
sudo apt-get install curl apt-transport-https ca-certificates software-properties-common
```

Berikut keterangnya:

	- apt-transport-https = tansfer file dan data melalui https.
	- ca-certificates = untuk cek sertifikat keamanan
	- curl = transfer data
	- software-properties-common = script untuk mengelola software.

![text](asset/1.png)

- Menambahkan repository docker dan update paket
```
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
sudo apt update
apt-cache policy docker-ce
```

![text](asset/2.png)
![text](asset/3.png)
![text](asset/4.png)


- Instal docker
``` 
sudo apt install docker-ce
```

![text](asset/5.png)

- Cek status docker
```
sudo systemctl status docker
```

![text](asset/6.png)

- Test menjalankan hello-world docker
```
docker run hello-world
docker images
```

![text](asset/7.png)

- Login ke docker
```
docker login
``` 
![text](asset/8.png)