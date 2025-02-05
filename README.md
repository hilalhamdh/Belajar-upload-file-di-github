# Cara Upload file di Github menggunakan GIT
### Apa sih itu Github ? 

github yaitu sebuah platform yang digunakan untuk menyimpan codingan kita, memanage codingan kita dan lain-lain.
sudah paham kan?

Disini aku ajari cara mengupload file ke github dengan menggunakan tols GIT!
Git itu adalah sebuah tols untuk memanage source code dan untuk berkolaborasi dengan develop lainnya.
nah Git membutuhkan platform yaitu Github.
Jadi Git itu tols dan Github itu platformnya.

Pertama sebelum kita upload project kita, kita konfirgurasi akun github kita terlebih dahulu.
- Pertama buka Git Bahs dengan klik kanan -> pilih Git Bahs
  
-  masukkan username dengan perintah
    - git config --global user.name "hilalhamdh" (username github yang kita gunakan)
- masukkan email
    - git config --global user.name "hilal@gmail.com"

itulah cara untuk konfigurasi akun github kita

Selanjutnya kita akan mengupload file ke Github
sebelum kita upload file kita akan belajar basic git terlebih dahulu

### Basic Git

- git init
  - membuat repositori Git baru
- git status
  - untuk melihat status direktori kerja dan area staging di Git
- git log
  - melihat riwayat komit dalam proyek Git
- git add
  - untuk menambahkan perubahan ke area staging di Git
- git commit
  - menyimpan perubahan pada proyek ke repositori lokal
- git push
  - untuk mengunggah konten dari repositori lokal ke repositori jarak jauh

Perintah-perintah diatas adalah perintah Git yang akan kita gunakan.

### Langkah-langkah upload file
- pertama membuat repository baru di github.

  
- Klik kanan pada file yang ingin di upload pada komputer, lalu kemudian pilih git bash
- setelah masuk repository, masukkan perintah
  - git init
  - git status    (untuk melihat apakah semua file masuk dalam repository baru). ketika belum maka, masukkan perintah
  - git add .     (untuk mengupload semua file kedalam repository)
  - git commit -m ("upload file.txt")
- kemudian upload file dengan perintah
  - git remote add origin "https://github.com/hilalhamdh/tokoOnline.git
  - git push --set-upstream origin master
  - git push -u origin master
    
Selesaiiiii, kemudian kembali ke githubnya file telah diupload.

### Ketika Mendapatkan Masalah
a. $ git remote add origin https://github.com/hilalhamdh/tokoOnline.git
   error: remote origin already exists.
   
  - cara mengatasinya dengan memasukkan perintah
    
    $ git remote rm origin
    
b. error: src refspec master does not match any
   error: failed to push some refs to 'https://github.com/hilalhamdh/tokoOnline.git'

  - Cara mengatasinya dengan memasukkan perintah

     git checkout -b master

c. remote: Permission to hilalhamdh/tokoOnline.git denied to hilalcode.
    fatal: unable to access 'https://github.com/hilalhamdh/tokoOnline.git/': The requested URL returned error: 403

  - Cara mengatasinya dengan memasukkan perintah

    git config credential.username "hilalhamdh"
    
### cara Edit File
  - git fetch origin master
  - git add .
  - git commit -m "add new file"
  - git push origin master --force


     
   




