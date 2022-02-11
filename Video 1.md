# ***Rangkuman Video 1***
# ***Git dan GitHub***

<p>&nbsp;</p>

Git dan GitHub merupakan dua hal yang berbeda. Git dapat digunakan tanpa GitHub, dan sebaliknya GitHub dapat digunakan tanpa adanya Git terinstall di komputer pengguna.

Git merupakan salah satu dari VCS (Version Control System).

<p>&nbsp;</p>

## 1. Version Control System
VCS adalah sistem yang mengelola dan menyimpan rekaman/snapshot perubahan dari sebuah source code.

Kenapa VCS harus digunakan? 
1.	Dapat melacak versi atau perubahan pada software. VCS merekam siapa yang melakukan dan kapan sebuah perubahan terjadi. Hal ini memungkinkan pengguna untuk kembali ke keadaan sebelum perubahan (checkout).
2.	Dapat memudahkan proses kolaborasi coding dalam tim
3.	Dapat digunakan untuk membagikan produk ke orang lain

Perbedaan VCS dengan Dropbox dan Google Drive :

Dropbox dan Google Drive tidak sefleksibel VCS karena kedua aplikasi tersebut tidak di desain untuk mengelola file berupa source code.

<p>&nbsp;</p>

## 2. Git
Git adalah sebuah VCS untuk mengelola perubahan file di dalam folder (repository atau repo). Riwayat perubahan file disimpan menggunakan serangkaian commit. Setiap commit akan direkam oleh satu snapshot.

Folder yang ditandai sebagai repository akan dipantau oleh Git, lalu Git akan menyimpan setiap perubahan yang terjadi pada folder tersebut.

Di dalam sebuah commit terdapat hash (penanda suatu commit), nama pengguna commit, tanggal pembuatan commit, dan pesan commit.

Dari suatu commit dapat dibuat cabang (branch) yang tidak terhubung dengan commit sebelum atau setelahnya. Suatu branch dapat digabungkan kembali ke master branch (Merge).

Git dapat digunakan secara local di komputer dengan menginstall software Git di komputer.

<p>&nbsp;</p>

## 3. GitHub
GitHub merupakan suatu website layanan cloud yang digunakan untuk membuat file yang dapat dikelola menggunakan Version Control milik GitHub. GitHub dapat melakukan hal yang dilakukan seperti Git di komputer.

Git dan GitHub dapat digunakan secara bersamaan. Misalnya user ingin mengirimkan source code dari komputer miliknya ke website GitHub, maka user dapat melakukan push. Sebaliknya, jika user ingin mengambil source code dari GitHub, dapat dilakukan pull.

Push = proses upload atau mengirimkan commit dari Git ke GitHub
Pull = proses mengambil commit dari GitHub ke Git

Syarat melakukan push dan pull adalah dengan membuat GitHub menjadi remote (sumber dari repo). Untuk melakukan push, clone suatu repo dari GitHub lalu pull commitnya. Sedangkan untuk melakukan push, edit dan save file lalu lakukan commit dah push.

GitHub sangat bermanfaat untuk proses kolaborasi. Repo yang berada di GitHub dapat terhubung ke banyak orang. Suatu proyek yang bermanfaat bisa disimpan di GitHub lalu orang lain dapat melihat, modifikasi, like, dll.

### **Istilah Git**
- Repo: folder project milik kita
- Commit: rekaman atau snapshot dari repo
- Hash: penanda unik pada suatu commit
- Checkout: berpindah ke suatu commit
- Branch: cabang bebas dari sebuah commit
- Merge: menggabungkan branch
- Remote: sumber yang memiliki repo
- Clone: mengambil repo dari remote
- Push: mengirimkan commit ke repo
- Pull: mengambil commit dari repo

