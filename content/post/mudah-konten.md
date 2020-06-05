---
title: "Mudah Membuat Konten Hugo"
date: 2020-06-05T23:25:58+07:00
Description: "Cara mudah membuat konten di Hugo"
Tags: ["hugo","markdown"]
Categories: []
DisableComments: false
---

Environment yang saya gunakan yaitu :
- Ubuntu 18.04
- Golang 1.14.4
- Hugo 0.72.0

## Folder project
Buka folder atau direktori project `Hugo` anda. Contoh blog saya ada di folder :

```
web/blog
```
kemudian klik kanan - open in Terminal untuk OS [Ubuntu](https://releases.ubuntu.com/18.04.4/), jika menggunakan [Visual Studio Code](https://code.visualstudio.com/download) silahkan Open Folder atau Add Folder to Workspace kemudian klik menu Terminal - New Terminal.

## Perintah membuat konten
Contoh saya ingin membuat konten dengan file `mudah-konten.md`, maka ketikan pada terminal yang sudah anda buka tadi dengan perintah :

```
hugo new post/mudah-konten.md
```
Atau jika ingin membuat konten manual bisa dengan membuka folder `content - post`, kemudian buat file `mudah-konten.md`.

## Mengisi konten
Buka file `mudah-konten.md` yang lokasinya ada di folder `content - post`, kemudian ubah title,Description,Tags sesuai keinginan anda. Tulis konten yang ingin anda buat dibawah sintaks `markdown ---`.

# Menjalankan Aplikasi
Untuk melihat hasil konten yang sudah kita buat, maka kita bisa menjalakan aplikasi project `Hugo` kita dengan perintah :

```
hugo server
```
Kemudian buka di `web browser`. `Default`-nya berjalan di URL [http://localhost:1313/](http://localhost:1313/).

Atau jika anda menggunakan [Visual Studio Code](https://code.visualstudio.com/download) dan ingin melihat hasil konten `markdown` tanpa menjalankan aplikasi bisa menekan shortcut `ctrl + shift +v` pada keyboard.

## Publish Server
Jika dirasa konten kita sudah sesuai dengan keinginan kita, maka kita bisa langsung membuild project `hugo` dengan perintah :

```
hugo
```
kemudian upload folder `public` (hasil generate) ke server.

Blog saya sendiri terhosting di [Github Page](https://pages.github.com/) dan menggunakan mekanisme auto deploy dengan skrip `deploy.sh`. Jadi saya tidak perlu mengetikan perintah panjang dari build sampai push ke repositori, cukup dengan mengetik perintah di terminal :

```
./deploy.sh
```

Jika anda ingin seperti saya, punya blog `Hugo` dengan hosting [Github Page](https://pages.github.com/) serta memiliki skrip auto deploy, bisa mengikuti tutorial dari [mas Rifky Fuady disini](https://rifkyfu32.github.io/blog/hugo-deploy-github/).