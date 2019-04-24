# Memulai Project Phonegap

### Install nodejs
$ curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -
$ sudo apt-get install -y nodejs

### Cek Versi
$ node --version  	(8.16.0)
$ npm --version 	(6.4.1)

### Install Phonegap
$ sudo npm install -g phonegap

### Buat Projek
$ phonegap create aplikasi/

### Run Projek
$ cd aplikasi
$ phonegap serve

### Stop Server
ctrl-c



### NOW BUILD APK
* $ apktool b folder -o cari.apk
* $ keytool -genkey -v -keystore my-release.jks
* $ apksigner -ks my-release.jks cari.apk
