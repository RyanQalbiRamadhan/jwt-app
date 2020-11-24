#Praktikum Pemrograman Integratif B  
Nama : Ryan Gatutkaca Qalbi Ramadhan,  
NIM : 185150700111020

#Modul 3
- Membuat beberapa route untuk melakukan registrasi, login, view user, dan logout.
- Membuat model User.php untuk memberikan parameter data berupa username, email, dan password bagi user.
- Membuat controller UserController.php untuk menyimpan segala perintah terkait dengan data dari user.
- Membuat tabel "users" pada database "jwt-auth" dengan menggunakan perintah migration.
- Membuat file auth.php yang didapat dari dalam folder vendor dengan beberapa modifikasi.
- Mengaktivasi fitur eloquent, facades, middleware auth, serta mendaftar package JWT.
- Men-generate sebuah secret key yang tersimpan pada .env untuk JWT.

Penjelasan Screenshot
- Pertama user dapat melakukan registrasi dengan menginput email, username, dan password ke dalam form.
- Dalam percobaan ini dilakukan registrasi untuk dua user baru, yaitu "administrator" dan "ryanqalbi".
- Setelah data berhasil teregistrasi, user pun dapat login dengan data yang telah diinput sebelumnya.
- Jika proses login berhasil, maka user akan mendapatkan sebuah token untuk dapat melakukan perintah yang lainnya.
- Token tersebut digunakan sebagai bukti bahwa user telah login dan akan terus berlaku dalam waktu 1 jam.
- Dengan menggunakan token tersebut, user dapat melihat datanya dengan mengakses url "http://localhost:8000/auth/me" serta melihat list user dengan mengakses url "http://localhost:8000/auth/user".
- Apabila user melakukan logout, maka token yang telah didapat sebelumnya tidak dapat digunakan kembali.