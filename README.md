# Belajar Vagrant #

* Vagrantfile sederhana
* Mapping port 80 di guest ke 8080 di host
* Mapping folder `/home/vagrant/aplikasisaya` ke host
* Provisioner untuk menginstal

    * git
    * Nginx
    * HHVM
    * MySQL
    * Laravel

* Konfigurasi Virtual Host

## Cara Menjalankan ##

* Masuk ke foldernya

```
cd belajar-vagrant
```

* Jalankan vagrant

```
vagrant up
```

* Jalankan provisioner

```
vagrant provision
```

* Konfigurasi host, tambahkan baris berikut dalam file `/etc/hosts` di **komputer anda**

```
127.0.0.1   aplikasisaya.contoh.com
```

* Test, browse ke `http://aplikasisaya.contoh.com:8080/`
