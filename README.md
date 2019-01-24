### **Apa itu GIT?**

Pada tahun 2005, Linus Torvalds (orang yang membuat kernel Linux) membuat GIT dan sejak itu GIT secara aktif dikelola oleh Junio Hamano, programmer Jepang. Saat ini, GIT menjadi salah satu version control system yang paling terkenal dan ada jutaan project di seluruh dunia yang menggunakan GIT untuk version control nya (termasuk project komersil dan open source). GIT sepenuhnya gratis dan bisa di-download di Mac, Linux, Windows, dan Solaris, dari [website resminya](https://git-scm.com/downloads). Fitur-fitur unggulan dari GIT antara lain:

1. Version control system yang terdistribusi, GIT menggunakan pendekatan peer to peer, tidak seperti yang lainnya seperti Subversion (SVN) yang menggunakan model **client-server.**
2. GIT memungkinkan developer untuk memiliki branch kode yang independent dan massive. Membuat, menghapus dan menggabungkan branch tersebut menjadi lebih cepat, lancar dan tidak butuh waktu yang lama.
3. dalam GIT, semua operasinya bersifat atomic, artinya sebuah tindakan akan benar-benar diselesaikan dengan lengkap atau sama sekali gagal. Ini sangat penting, karena di beberapa version control system seperti CVS, operasinya bersifat non-atomic. Jika ada operasi yang ‘gantung’ dan terkait dengan repository, kondisi repository menjadi tidak stabil.
4. Dalam GIT, semuanya disimpan dalam folder .git. Berbeda dengan VCS lain seperti SVN atau CVS, dimana metadata file disimpan dalam folder tersembunyi seperti .cvs, .svn, .etc.
5. GIT menggunakan data model yang membanti memastikan integritas cryptographic apapun ada dalam repository. Setiap kali sebuah file ditambahkan atau di-commit, checksum-nya akan diciptakan; sama hal nya, juga di-retrieve lewat checksum-nya juga.
6. Fitur menarik lainnya yang ada di GIT adalah staging area atau index. Dengan stagin area, developer bisa memformat commit dan membuatnya bisa di-review sebelum benar-benar diterapkan.

GIT sangat sederhana dalam penggunannya. Untuk memulai, Anda bisa membuat repository atau men-checkout yang sudah ada. Setelah instalasi, perintah ```git-init``` akan men-setup semuanya. Selain itu, perintah ```git clone bisa``` membuat salinan repository lokal untuk user.


### **Langkah 1 – Install GIT**

Menginstall GIT di Windows sangat mudah, cukup dengan mendownload dan menjalankan instalasinya. Ikuti langkah berikut ini untuk meng-install GIT di Windows:

1. Buka [website ini](https://gitforwindows.org/) dan download installer GIT untuk Windows.
2. Setelah download, buka file tersebut untuk menjalankan proses instalasi. Ikuti semua instruksi, klik Next dan Finish hingga semua proses instalasi selesai.

![gambar](https://user-images.githubusercontent.com/46735362/51677971-cc8d8080-200d-11e9-8467-0837633d21c7.png)

3. Jalankan perintah berikut ini di terminal:

![user dan email](https://user-images.githubusercontent.com/46735362/51680412-46c10380-2014-11e9-8279-8d90fd05bc8d.png)


### **Langkah 2 - Membuat Repository Local**

1. Buka direktori aktif, misal: **C:\Pemrograman\Program1** (buka menggunakan Windows Explorer).
2. Klik kanan pada direktori aktif tersebut, dan pilih menu **Git Bash**, sehingga muncu _git bash command_.
3. Buat direktory praktikum pertama dengan nama  **Latihan1**.

```$ mkdir latihan```

```$ cd latihan1```

![buat directory](https://user-images.githubusercontent.com/46735362/51680584-bb943d80-2014-11e9-8fe1-5b77af98d162.png)

4. Sehingga terbentuk satu direktori baru dibawahnya, selanjutnya masuk kedalam direktori tersebut dengan perintah **cd** (_change directory_).
5. Direktori aktif menjadi: **C:\Pemrograman\Program1\Latihan1**.
6. Jalankan perintah ```git init```, untuk membuat repository local.

![git init](https://user-images.githubusercontent.com/46735362/51681072-2134f980-2016-11e9-9f3a-d75a19a3d62c.png)

7. Repository baru berhasil diinisialisasi, dengan terbentuknya satu direktori hiden dengan nama **.git**.
8. Pada direktori tersebut, semua perubahan pada _working directory_ akan disimpan.


### **Langkah 3 - Menambahkan File Baur Pada Repository**

1. Untuk membuat file dapat mennggunakan tex editor, lalu menyimpan filenya pada direktori aktif (repository).
2. Disini kita akan coba membuat satu file bernama README.md (text file).

```echo "#Latihan 1" >> README.md```

3. File **README.md** berhasil dibuat.

![echo](https://user-images.githubusercontent.com/46735362/51681803-50e50100-2018-11e9-93ca-2a6b9cbc81ca.png)

4. Untuk menambahkan file yang baru saja dibuat tersebut, gunakan perintah **git add**

```git add README.md```
5. file **README.md** berhasil ditambahkan.

![git add](https://user-images.githubusercontent.com/46735362/51682547-4297e480-201a-11e9-9ebd-5c997ee368a8.png)


