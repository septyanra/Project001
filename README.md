
**"TUTORIAL PEMBUATAN REPOSITORY LOCAL dan PEMBUATAN FILE README.md MENGGUNAKAN Git"**


 **1. Instal Software Git**
      
   - Download **Git** melalui website resminya di https://git-scm.com. Unduh sesuai spesifikasi komputer anda, jika spesifikasi komputer anda 64bit unduh yang 64bit, begitupula dengan yang 32bit.
   
        ![2019-10-26 (26) 02](https://user-images.githubusercontent.com/57028466/67623548-3da3d380-f7ec-11e9-8d10-0e58fc68afea.png)      
         
   - Apabila sudah terinstal cobalah untuk buka **CMD** atau **PowerShell**, kemudian ketik perintah
   
      **git --version**
      
      ![2019-10-26 (28)](https://user-images.githubusercontent.com/57028466/67623629-37622700-f7ed-11e9-8284-2e0072e6dd2c.png)
      
 **2. SIGN UP Akun GitHub**
  
   - Buat akun GitHub dengan cara membuka laman https://github.com.
   - Masukan Username, Email dan Password yang akan digunakan pada akun GitHub.
   
      ![Capture 03](https://user-images.githubusercontent.com/57028466/67624015-827e3900-f7f1-11e9-989c-0e5b813af423.PNG)
      
   - Lakukan verifikasi akun dengan membuka E-mail. 
   
      ![Capture 09 EMAIL](https://user-images.githubusercontent.com/57028466/67624163-e9502200-f7f2-11e9-99c6-709b0d08ab69.png)
      
   - Setelah melakukan verifikasi, anda akan di alihkan ke page GitHub untuk selanjutnya membuat Repository baru, masukkan nama Repository anda dan klik **create repository**.
   
      ![2019-10-26 (19) projrct](https://user-images.githubusercontent.com/57028466/67624243-c07c5c80-f7f3-11e9-95c0-1f78a2620a46.png)
      
   - Berikut tampilan Repository baru
   
      ![2019-10-26 (42) baruuuuuuuuuuu](https://user-images.githubusercontent.com/57028466/67625659-82d4ff00-f806-11e9-952f-cc986a3ea08c.png)
      
  **3. Membuat Repository Local**
  
   - Klik kanan pada Dekstop, kemudian pilih menu **Git Bash Here**, sehingga muncul git bash commad
   
     ![2019-10-26 (40) 01](https://user-images.githubusercontent.com/57028466/67623926-95443e00-f7f0-11e9-9293-11618d184ec9.png)
   
   - Menambahkan Global Config, dengan melakukan konfigurasi **user.name** dan **user.email**, apabila belum dilakukan konfigurasi, akan mengakibatkan terjadi kegagalan saat menjalankan perintah **git commit**. Misal:
   
      **$ git config --global user.name "septyanra"**
      
      **$ git config --global user.email "septyanoera23@gmail.com"**
      
      ![2019-10-26 (14) potong](https://user-images.githubusercontent.com/57028466/67623810-41852500-f7ef-11e9-9d62-50da185f2fa3.png)
      
   - Buat direktory project praktikum pertama, dengan perintah ***mkdir***, misalkan dengan nama **LATIHAN_001**
   
      **$ mkdir LATIHAN_001**
      
   - Sehingga terbentuk satu direktori baru dibawahnya, selanjutnya masuk kedalam direktori tersebut dengan perintah ***cd*** (change directory) 
      
      **$ cd LATIHAN_001**
      
      ![2019-10-26 (14) mkdr dan cd](https://user-images.githubusercontent.com/57028466/67624421-f7537200-f7f5-11e9-8ba6-d301ecc0c746.png)
      
   - Buat repository local dengan menggunakan perintah **git init**
   
      **$ git init**
      
   - Repository baru berhasil di inisialisasi, dengan terbentuknya satu direktori hidden dengan nama **.git** 
   
      ![2019-10-26 (20) git init](https://user-images.githubusercontent.com/57028466/67624582-02a79d00-f7f8-11e9-9b41-3625ab85021f.png)

 **4. Menambahkan File Baru pada Repository**
 
   - Buat satu file README.md dengan menggunakan perintah 
   
      **$ echo "#LATIHAN_001" >> README.md**
      
   - File **README.md** berhasil dibuat 
      
     ![2019-10-26 (31) ECHOOOO 111111111111](https://user-images.githubusercontent.com/57028466/67624751-6d59d800-f7fa-11e9-827e-fe8813af8f70.png)
     ![2019-10-26 (31) ECHOOOO 2222222222222](https://user-images.githubusercontent.com/57028466/67624763-97ab9580-f7fa-11e9-817c-3e5fea16e61e.png)
     
   - Langkah selanjutnya menambahkan file yang baru dibuat, gunakan perintah **git add**.
      
      **$ git add README.md**
      
      ![2019-10-26 (24) git adddddd](https://user-images.githubusercontent.com/57028466/67624830-ac3c5d80-f7fb-11e9-9cea-2ce411890228.png)
      
 **5. Menyimpan Perubahan ke Database (***Commit***)**
 
   - Simpan perubahan kedalam database repository local, gunakan perintah **git commit -m “komentar commit”**
      
      **$ git commit -m "File Pertama Saya"**
      
   - Kemudian akan muncul 
     
     ![2019-10-26 (22) commit](https://user-images.githubusercontent.com/57028466/67624922-dcd0c700-f7fc-11e9-89ea-b80fbe849f14.png)
     
 **6. Menambahkan Remote Repository**
 
   - Remote Repository merupakan repository server yang akan digunakan untuk menyimpan setiap perubahan pada local repository, sehingga dapat diakses oleh banyak user. 
   - Untuk menambahkan remote repository server, gunakan perintah **git remote add origin [url]**
   
      **$ git remote add origin https://github.com/septyanra/Project001.git**
      
      ![2019-10-26 (24) server](https://user-images.githubusercontent.com/57028466/67625221-d7757b80-f800-11e9-976c-d2ed6fa15c76.png)
      
 **7. Mengirim Perubahan ke Server (***Push***)**
 
   - Gunakan Perintah **git push**
   
      **$ git push -u origin master**
      
   - Sebelumnya akan ada perintah untuk **GitHub login** setelah anda klik enter menggunakan perintah **git push**, gunakan akun GitHub yang telah dibuat diatas tadi. Kemudian klik **Login**
   
      ![2019-10-26 (21) log in github](https://user-images.githubusercontent.com/57028466/67625500-9aab8380-f804-11e9-92f9-a32212330004.png)
      
   - Penampakan setelah dilakukan Login  
    
      ![2019-10-26 (22) pushhh](https://user-images.githubusercontent.com/57028466/67625268-7c905400-f801-11e9-8175-4c4aa8bba33c.png)
  
   - Buka **github.com**, arahkan pada repositorinya. Untuk melihat perubahan yang terjadi.
   
      ![2019-10-26 (23) perubahan](https://user-images.githubusercontent.com/57028466/67625357-b9107f80-f802-11e9-8fa0-6d8a3a5d4b9d.png)
      
**8. Clone Repository**
    
   - Clone repository, pada dasarnya adalah meng-copy repository server dan secara otomatis membuat satu direktory sesuai dengan nama repositorynya (working directory).
   - Dengan menggunakan perintah **git clone [url]**
      
      **$ git clone https://github.com/septyanra/Project001.git**
      
      ![2019-10-26 (25) CLONE](https://user-images.githubusercontent.com/57028466/67625390-553a8680-f803-11e9-856e-938133d96bc8.png)
      
      
      
    

      

    
      
      
      
    
      
   

      
      
