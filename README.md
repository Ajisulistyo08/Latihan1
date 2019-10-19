#Latihan 1

Tutorial menggunakan git
1.Tutorial membuat DVCS (Distributed Version Control System) menggunakan aplikasi git
2.Download Git, buka website resminya Git (git-scm.com).

![image](https://user-images.githubusercontent.com/56190945/67135088-5afefd80-f240-11e9-9c5f-a6f2108f9d67.png)
 
3.Kemudian unduh Git sesuai dengan arsitektur komputer kita. Kalau menggunakan 64bit, unduh yang 64bit. Begitu juga kalau menggunakan 32bit.

4.Setelah didownload dan di instal, Untuk mencobanya, silahkan buka aplikasi git, kemudian ketik perintah "git --version"
 
 
![image](https://user-images.githubusercontent.com/56190945/67135117-97caf480-f240-11e9-93e0-237e190da5a6.png)

 
5.Sebelum menambahkan Global Config , buatlah akun github diserver reopsitory, server yang digunakan adalah http://github.com
 
 ![image](https://user-images.githubusercontent.com/56190945/67135137-c943c000-f240-11e9-9d6c-17467d7c435b.png)

•	Setelah membuat akun github dan sudah login , buatlah repository server Pada laman github, klik tombol start a project, atau
•	Dari menu (icon +) klik New Repository
 
 
![image](https://user-images.githubusercontent.com/56190945/67135160-0445f380-f241-11e9-857d-7fc5b24e0201.png)

6. Isi nama repositorynya, misal: latihan1. lalu klik tombol Create repository
  
  
![image](https://user-images.githubusercontent.com/56190945/67135178-322b3800-f241-11e9-99ac-88778b5a26ba.png)

 
7.Menambahkan Global Config
•	konfigurasi ini bisa dilakukan untuk global repostiry atau individual repository.
•	apabila belum dilakukan konfigurasi, akan mengakibatkan terjadi kegagalan saat menjalankan perintah git commit
•	dengan mengetik:  
 	git config --global user.name “nama_user”
    
  ![image](https://user-images.githubusercontent.com/56190945/67135231-ca292180-f241-11e9-9a64-a4f1dc4c7119.png)
 
	git config --global user.email “nama_user”
 
  ![image](https://user-images.githubusercontent.com/56190945/67135242-f5137580-f241-11e9-8860-dd685e92410a.png)

8.Membuat Reposiory Local
•	Buka direktory aktif, (buka menggunakan Windows Explorer)
•	klik kanan pada direktory aktif tersebut, dan pilih menu Git Bash, sehingga muncul git bash commad
•	Buat direktory project praktikum pertama dengan nama latihan1
•	Dengan mengetik:


mkdir latihan1

  ![image](https://user-images.githubusercontent.com/56190945/67135267-33109980-f242-11e9-852d-9bcd17c18163.png)
 
cd latihan1
   
![image](https://user-images.githubusercontent.com/56190945/67135285-5c312a00-f242-11e9-974d-86822cd69412.png)

Sehingga terbentuk satu direktori baru dibawahnya, selanjutnya masuk kedalam direktori tersebut dengan    perintah cd (change directory)
direktory aktif menjadi: C:\users\USER\latihan1
 
![image](https://user-images.githubusercontent.com/56190945/67135304-97cbf400-f242-11e9-9e7e-6b8846ae9f79.png)

9.Membuat Reposiory Local
•	Jalankan perintah git init, untuk membuat repository local.
Dengan mengetik: git init

  ![image](https://user-images.githubusercontent.com/56190945/67135356-e11c4380-f242-11e9-8182-243674ddf6bc.png)
 
•	Repository baru berhasil di inisialisasi, dengan terbentuknya satu direktori hidden dengan nama .git
•	Pada direktori tersebut, semua perubahan pada working directory akan disimpan.


10. Menambahkan File baru pada repository
•	Untuk membuat file dapat menggunakan text editor, lalu menyimpan filenya pada direktori aktif (repository)
Dengan mengetik: echo “#Latihan 1” >> README.md
 
 ![image](https://user-images.githubusercontent.com/56190945/67135370-1de83a80-f243-11e9-909d-526e7cd673bd.png)
 
•	disini kita akan coba buat satu file bernama README.md (text file)
              File README.md berhasil dibuat


11.Menambahkan File baru pada repository
•	Untuk menambahkan file yang baru saja dibuat tersebut gunakan perintah git add.
Dengan mengetik: git add README.md

  ![image](https://user-images.githubusercontent.com/56190945/67135389-43754400-f243-11e9-9151-dde6f311a463.png)
  

![image](https://user-images.githubusercontent.com/56190945/67135406-699ae400-f243-11e9-9ea0-4b9be3320ede.png)

•	File README.md berhasil ditambahkan.


12. Commit (Menyimpan perubahan ke database)
•	Untuk menyimpan perubahan yang ada kedalam database repository local, gunakan perintah git commit -m “komentar commit”
Dengan mengetik: git commit -m “File pertama saya”
 
![image](https://user-images.githubusercontent.com/56190945/67136265-0febe700-f24e-11e9-9998-6f49d07773d6.png)


•	Perubahan berhasil disimpan.


13.Menambahkan Remote Repository
•	Remote Repository merupakan repository server yang akan digunakan untuk menyimpan setiap perubahan pada local repository, sehingga dapat diakses oleh banyak user.
•	Untuk menambahkan remote repository server, gunakan perintah git remote add origin [url]
Dengan mengetik: git remote add origin https://github.com/ajisulistyo08/latihan1.git
 
![image](https://user-images.githubusercontent.com/56190945/67136276-3ad63b00-f24e-11e9-84fd-b97fed76519c.png)

14.Push (Mengirim perubahan ke server)
•	 Untuk mengirim perubahan pada local repository ke server gunakan perintah git push.
Dengan mengetik: git push -u origin master
 

![image](https://user-images.githubusercontent.com/56190945/67136285-593c3680-f24e-11e9-85ba-ec0ada4c0277.png) 

•	Perintah ini akan meminta memasukkan username dan password pada akun github.com

15.Melihat hasilnya pada server repository
  
![image](https://user-images.githubusercontent.com/56190945/67136295-80930380-f24e-11e9-9ac6-391190b42444.png)

