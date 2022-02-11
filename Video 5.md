# ***Rangkuman Video 5***
# ***Git***

<p>&nbsp;</p>

## ***1. Instalasi dan Pengenalan Git***
Penginstallan git dapat dilakukan melalui website git-scm.com 

Git digunakan melalui console atau command prompt. Namun, Git mempunyai Git Client yaitu software untuk menggunakan Git tanpa console. Tidak seperti command prompt, Git Client tersedia dalam tampilan GUI (Graphical User Interface). Contoh dari Git Client, yaitu sourcefree.

Tata cara install Git
1.	Buka website git-scm.com
2.	Klik download for Windows
3.	Setelah proses pengunduhan selesai, klik filenya
4.	Lakukan proses instalasi sesuai preferensi

Pada opsi instalasi komponen, pastikan untuk mencentang Git Bash. Git Bash adalah terminal khusus untuk Git yang dapat menerima perintah-perintah bash atau shell command. Command Prompt secara default tidak bisa menerima perintah shell atau bash. 

Setelah selesai menginstall Git, buka Git Bash. Pada Git Bash, ketik “git” untuk memunculkan bantuan cara menggunakan Git

![Screenshot_1](https://i.ibb.co/Ms9HtN1/Picture1.jpg)

Ketik “clear” untuk menghilangkan isi terminal

Untuk mengecek versi Git, ketik “git --version"

![Screenshot_2](https://i.ibb.co/X7DxTJd/Picture2.jpg)

<p>&nbsp;</p>

Contoh-contoh perintah Git
- $ git init : untuk menginisiasi repo git di komputer
- $ git add <file(s)> : untuk menambahkan file ke dalam staging area
- $ git status : untuk mengetahui status repo
- $ git commit : untuk melakukan commit
- $ git config : untuk memasukkan konfigurasi ke dalam Git
- $ git branch : untuk membuat branch
- $ git help : untuk memunculkan perintah-perintah Git

<p>&nbsp;</p>

### **Tiga area pada repo git**
1.	**Working Tree** : folder tempat bekerja
2.	**Staging Area** : User memberi tahu Git bahwa telah terjadi perubahan
3.	**History** : Tempat tersimpannya commit

Staging area dan history akan tersimpan dalam satu folder (.git) yang tersembunyi.

Jika suatu folder diinisiasi sebagai repo git, maka Git akan memantau segala perubahan pada folder tersebut. Setiap perubahan dapat disimpan pada Staging area dengan menggunakan command git add. Selanjutnya dari staging area, dapat dilakukan commit dengan command git commit.

<p>&nbsp;</p>
<p>&nbsp;</p>

## ***2. Bekerja dengan Git***
Untuk mengecek directory aktif, gunakan command pwd

Untuk membuat sebuah folder menjadi repo git, terlebih dahulu kita haru masuk ke dalam folder tersebut. Karena directory saat ini masih di user, maka kita harus ubah directory ke folder repo menggunakan command cd <**nama folder**>

Untuk membuat folder biasa menjadi repo git, gunakan perintah **"git init"**

![Screenshot_3](https://i.ibb.co/cXdgNwM/Picture3.jpg)

Untuk melihat folder (.git) yang tersembunyi:

- Buka file explorer -> buka folder repo -> Klik tab View -> klik Options -> klik tab View -> Klik Show hidden files, folders, and drives -> unmark Hide extensions for known file types.

- Lalu jika kembali ke folder repo di file explorer, folder (.git) akan muncul.

<p>&nbsp;</p>
<p>&nbsp;</p>

### ***Memasukkan file ke staging area***
Git dapat digunakan dalam software code editor seperti Visual Studio Code atau Sublime Text.

Buka code editor yang digunakan lalu open folder repo dari dalam code editor. Melalui code editor, pada repo dapat ditambahkan file yang dapat kita edit. Namun, perubahan pada file tidak akan direkam oleh Git jika kita belum memasukkannya ke staging area.

Untuk mengecek commit dapat dijalankan perintah “git status”.

![Screenshot_4](https://i.ibb.co/vdzvR5n/Picture4.jpg)

Gambar diatas menunjukkan beberapa informasi, yaitu :
1.	Branch berada di branch master
2.	Git tidak mendeteksi adanya perubahan (commit) karena belum ada pembuatan commit.
3.	Terdapat file yang belum di track yaitu index.html

Agar file index.html bisa dicommit, harus terlebih dahulu dipindahkan ke staging area. Caranya adalah dengan menjalankan perintah “git add index.html”. Kemudian, jika dijalankan perintah “git status” lagi, maka akan diberikan informasi file baru yaitu index.html yang siap untuk dicommit. Untuk menghapus file dari staging area dapat dijalankan perintah “git rm --cached <**namaFile**>”.

![Screenshot_5](https://i.ibb.co/Mf3Ftcp/Picture5.jpg)

<p>&nbsp;</p>

### ***Konfigurasi nama dan email user***
Pada setiap commit diperlukan informasi user yang melakukan commit dan email user tersebut. Maka, gunakan perintah “git config --global user.name <“Nama”>” untuk menambahkan nama user dan perintah “git config --global user.email <“email”>” untuk menambahkan email user.

![Screenshot_6](https://i.ibb.co/1nyvtP8/Picture6.jpg)

<p>&nbsp;</p>

### ***Pembuatan commit***
1. Untuk melakukan commit, gunakan perintah “git commit -m <“pesan”>”

![Screenshot_7](https://i.ibb.co/6F0XynW/Picture7.jpg)

<p>&nbsp;</p>

2. Ketika menambahkan file baru atau mengedit file dalam repo, jika user tidak membuat commit untuk file tersebut, maka perubahan tidak akan ditrack/direkam.

![Screenshot_8](https://i.ibb.co/NjFmQQg/Picture8.jpg)

Gambar di atas menunjukkan contoh file baru yang belum direkam (untracked) dan perubahan pada file lama yang tidak diupdate oleh Git. Untuk menambahkan kedua file sekaligus ke dalam staging area, jalankan perintah “git add .” Setelah file dimasukkan ke dalam staging area, barulah commit dapat dibuat.

![Screenshot_9](https://i.ibb.co/L0dgxSt/Picture9.jpg)

<p>&nbsp;</p>

### ***Melihat riwayat commit***
1. Melihat iwayat lengkap dari semua commit, jalankan perintah “git log".
2. Melihat 3 commit terakhir, gunakan perintah “git log -3”
3. Melihat commit untuk file tertentu, gunakan perintah “git log -- <**namaFile**>”

![Screenshot_10](https://i.ibb.co/Jp2ft5C/Picture10.jpg)



<p>&nbsp;</p>

### ***Checkout***
Untuk melakukan checkout ke suatu keadaan, gunakan perintah “git checkout <5 digit pertama dari commit hashnya>”. Commit tetap harus dibuat setelah melakukan checkout.

![Screenshot_11](https://i.ibb.co/HhXD9PD/Picture11.jpg)


