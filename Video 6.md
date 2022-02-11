# ***Rangkuman Video 6***
# ***Git Branch dan Merge***

<p>&nbsp;</p>

## ***1. Git dalam Visual Studio Code***
Pada code editor Visual Studio Code, file dengan tanda huruf U di samping kanannya menandakan bahwa file tersebut Untracked atau belum dimasukkan ke dalam staging area. Visual Studio Code mempunyai terminal sendiri yang memungkinkan user menjalankan perintah Git tanpa melalui Git Bash.

File dengan tanda M di samping kanan menandakan bahwa file tersebut telah di modifikasi (Modified). Untuk menambahkan file ke staging area sekaligus membuat commit, dapat digunakan perintah “git add -am <”pesan”>”.

![Screenshot_12](https://i.ibb.co/zQ2FT11/Picture12.jpg)

<p>&nbsp;</p>
<p>&nbsp;</p>

## ***2. Branch***
Setiap commit terhubung pada suatu branch tertentu. Untuk mengetahui branch aktif tempat commit berada, ada istilah head yaitu pointer yang mengarah ke branch yang aktif.

Perintah “git branch <**nama_branch**> digunakan untuk menambahkan branch.

![Screenshot_13](https://i.ibb.co/wYXmyJ0/Picture13.jpg)

<p>&nbsp;</p>

### ***Berpindah Branch***
Cara berpindah branch dilakukan dengan perintah “git checkout <**nama_branch**>”

![Screenshot_14](https://i.ibb.co/YNjvvtt/Picture14.jpg)

Ketika dilakukan perubahan, misalnya penambahan file baru, commit tersebut tidak lagi berada di master branch, melainkan berada di branch ‘dosen’.

![Screenshot_15](https://i.ibb.co/m8NfgLd/Picture15.jpg)

### ***Grafik perjalanan branch***
Perjalanan dari branch dapat dilihat melalui sebuah graph dengan perintah

“git log --all --decorate --oneline --graph".

![Screenshot_16](https://i.ibb.co/9vC7RPR/Picture16.jpg)
![Screenshot_17](https://i.ibb.co/7XhcwXF/Picture17.jpg)
![Screenshot_18](https://i.ibb.co/pzxsmTf/Picture18.jpg)

<p>&nbsp;</p>
<p>&nbsp;</p>

## ***3. Merge***
Dua Jenis Merge:
1.	Fast Forward: branch yang ingin digabungkan berada pada direct path.
2.	Three-way Merge: branch yang ingin digabungkan tidak berada pada direct path.

<p>&nbsp;</p>

### ***a. Fast Forward Merge***
Merge dapat dilakukan dengan perintah “git merge <**nama_branch**>”

![Screenshot_19](https://i.ibb.co/qyhjX4w/Picture19.jpg)

Jika merge berhasil dilakukan, file dosen yang tadinya berada pada branch dosen akan muncul pada master branch

![Screenshot_20](https://i.ibb.co/1nY128h/Picture20.jpg)

**Menghapus Branch**

Penghapusan branch dilakukan dengan perintah “git branch -d <**nama_branch**>”. Sedangkan penghapusan branch yang belum dimerge dilakukan dengan perintah “git branch -D <**nama_branch**>”.

![Screenshot_21](https://i.ibb.co/hHJGsfM/Picture21.jpg)

<p>&nbsp;</p>

### ***b. Three-way merge***
Ketika user melakukan three-way merge, akan dilakukan commit dan user diminta memasukkan pesan commit.

![Screenshot_22](https://i.ibb.co/DbJDgCS/Picture22.jpg)

Setelah commit di merge ke master branch, grafik akan terlihat seperti gamabar di bawah

![Screenshot_23](https://i.ibb.co/vkFxLt0/Picture23.jpg)


