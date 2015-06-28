---
layout: post
title: Create Github Pages
---

Nah jadi ada 2 jenis github pages itu sendiri yakni page untuk user/organization dan pages untuk project.
Pages untuk user/organization mempunyai link sebagai berikut **username.github.io** sedangkan untuk project **username.github.io/repository-name**.

Cara membuat page untuk user/organization:


1. Membuat repository dengan nama **your-username.github.io** (username merupakan username github kamu atau nama organisasi kamu)
2. Clone repository yang sudah dibuat, bisa menggunakan terminal dengan perintah ***git clone https://github.com/your-username/your-username.github.io*** atau melalui client github yang tersedia untuk windows dan mac
3. Masuk kedalam folder **your-username.github.io** yang sudah di clone sebelumnya dan tambahkan file index.html
4. Lakukan perintah ***git add --all*** untuk menambahkan file kedalam stash
5. Commit dengan perintah *git commit -m "keterangan"*
6. Push ke server dengan perintah ***git push -u origin master*** atau ***git push origin master***
7. Sekarang github pages kamu bisa diakses dengan url **your-username.github.io**

Selanjutnya cara membuat pages untuk project:


1. Membuat repository dengan nama project kamu
2. Clone dengan perintah ***git clone https://github.com/your-username/your-repository-name.git***
3. Masuk kedalam folder yang telah di clone dan buat branch baru dengan nama gh-pages dengan perintah ***git checkout --orphan gh-pages*** 
dan lakukan perintah ***git rm -rf .***
4. Tambahkan file index.html
5. Lakukan perintah ***git add --all*** 
6. Commit dengan perintah ***git commit -m "keterangan"***
7. Push ke server dengan perintah ***git push -u origin gh-pages*** atau ***git push origin gh-pages***
8. Sekarang github pages kamu bisa diakses dengan url **your-username.github.io/your-repository-name**
9. Kamu juga bisa mengenerate secara langsung template site yang sudah disediakan oleh github dengan cara masuk ke repository project kamu dan pilih menu **Setting** dan kemudian pilih **Automatic Page Generator** dan kemudian tambahkan content dan layout yang sudah disediakan oleh github. 

Next post saya akan memberikan tutorial tentang membuat blog dengan menggunakan Jekyll yang dihosting di github pages. See you next post :)
