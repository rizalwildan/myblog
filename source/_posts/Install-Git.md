title: Install Git
author: rizalwildan
tags:
  - Learn Git
categories: []
cover: /img/contact-bg.jpg
date: 2016-10-31 14:27:00
---
Setelah kita mengetahui apa itu Version Control Sistem dan apa itu Git serta pentingnya Git untuk Devloper tim, sekarang aku mau share bagaimana cara menginstall Git di komputer kalian. Sebenarnya cara menginstall Git tidak susah dan sama saja dengan menginstall aplikasi komputer pada umumnya, namun setiap sistem operasi memiliki metode sendiri-sendiri dalam menginstall aplikasi.

### Install Git di Mac OSX
Ada beberapa cara untuk menginstall Git di Mac. Bahkan, jika kamu pernah menginstall XCode, git mungkin sudah otomatis terinstall di sistem kamu. Untuk mengecheknya, buka terminal dan masukkan perintah git version.

```bash
$ git --version
git version 2.7.0 (Apple Git-66)
```
sebenarnya Apple sudah menyediakan [aplikasi Git di repository Open Source mereka](http://opensource.apple.com/source/Git/). Tetapi versi git yang ada di repository mereka cenderung ketinggalan dengan versi git utama. Jika kamu ingin menginstall versi git yang terbaru, mungkin kamu bisa mengikuti metode berikut ini:

**Install Via Stand-Alone Installer**

Cara ini merupakan cara paling termudah.
1. Download [Git for Mac Installer](https://sourceforge.net/projects/git-osx-installer/files/) versi terbaru.
2. Ikuti petunjuk untuk menginstall Git.
3. Jika proses installasi sudah selesai, buka terminal dan pastikan Git benar-benar telah terinstall dengan mengetik git --version:
```bash
$ git --version
git version 2.9.2
```
4. Konfigurasi Git username dan email kamu menggunakan perintah berikut, pastikan kamu menggunakan username dan email yang sudah terdaftar di [Github](https://www.github.com). Username dan email ini nantinya akan berguna sebagai detail identitas dari commit yang pernah kamu buat.
```bash
$ git config --global user.name "Username"
$ git config --global user.email "user@mail.com"
```
Selamat kamu sudah berhasil menginstall dan mengkonfigurasi aplikasi Git kamu di Mac OSX.

### Install Git di Windows
Kalau install aplikasi di windows sih tidak perlu di jelaskan panjang lebar, tinggal klik Next, Next, Next sudah beres. Kecuali kamu memang pengen membaca *User Agreement and Privacy Policy* secara seksama. Oke langsung saja langkahnya seperti berikut:
1. Download [Git](https://git-for-windows.github.io/) versi terbaru
2. Jika kamu berhasil membuka installer, pastinya kamu juga bisa melihat **Git Setup wizard screen**. Tentunya ikuti saja perintah **Next** sampai nanti ketemu perintah **Finish** untuk menyelesaikan installasi. Oh iya option default dalam proses installasi sangat dianjurkan ya.
3. Untuk menjalankan perintah git di windows, kamu bisa menggunakan *Windows Command Prompt* (CMD) atau *Git Bash* (konsol yang disediakan oleh git). 
4. Konfigurasi Git username dan email kamu menggunakan perintah berikut, pastikan kamu menggunakan username dan email yang sudah terdaftar di [Github](https://www.github.com). Username dan email ini nantinya akan berguna sebagai detail identitas dari commit yang pernah kamu buat.
```bash
$ git config --global user.name "Username"
$ git config --global user.email "user@mail.com"
```
Selamat kamu sudah berhasil menginstall dan mengkonfigurasi aplikasi Git kamu di Windows.

### Install Git di Linux
Metode installasi git ada dua yaitu viap apt (Debian/ubuntu) dan via yum / dnf (fedora).

**Debian/Ubuntu (apt-get)**

Paket git di Linux Debian/Ubuntu tersedia via apt, cara installnya seperti berikut:
1. Buka terminal shell, install Git menggunakan apt-get:
```bash
$ sudo apt-get update
$ sudo apt-get install git
```
2. Pastikan Git sudah berhasil terinstall dengan memasukkan perintah git --version.
```bash
$ git --version
git version 2.9.2
```
3. Jangan lupa konfigurasi Git global username dan email.

**Linux Fedora (dnf/yum)**

Paket Git di Linux Fedora tersedia via [dnf](https://fedoraproject.org/wiki/Dnf) dan [yum](https://fedoraproject.org/wiki/Yum), cara installnya seperti berikut:
1. Buka terminal shell, install Git menggunakan dnf atau menggunakan yum untuk Fedora versi sebelumnya:
```bash
$ sudo dnf install git
```
	atau
```bash
$ sudo dnf install git
```
2. Pastikan Git sudah berhasil terinstall dengan memasukkan perintah git --version.
```bash
$ git --version
git version 2.9.2
```
3. Jangan lupa konfigurasi Git global username dan email.