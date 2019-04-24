-- Buat Phone Gap
$ curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -
$ sudo apt-get install -y nodejs

-- cek versi
$ node --version  	(8.16.0)
$ npm --version 	(6.4.1)

-- install phonegap
$ sudo npm install -g phonegap

-- buat projek
$ phonegap create aplikasi/

-- run projek
$ cd aplikasi
$ phonegap serve

-- stop
ctrl-c



### NOW BUILD APK ###
-- build
apktool b folder -o cari.apk

-- buat tandatangan
keytool -genkey -v -keystore my-release.jks

-- tandatangani
apksigner -ks my-release.jks cari.apk
