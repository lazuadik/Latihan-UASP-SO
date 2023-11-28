```
# pindah ke direktori home anda
$ cd ~
# buat satu folder kosong 'test'
$ mkdir test
# masuk ke direktori 'test'
$ cd test
# tampilkan path direktori saat ini
$ pwd
# buat file kosong bernama 'empty.txt'
$ touch empty.txt
```

```
# copy file '/etc/timezone' ke direktori ini
$ cp '/etc/timezone' test
# ubah nama file 'timezone' menjadi 'tz.txt'
$ mv timezone tz.txt
# list isi direktori ini
$ ls test
# pindah ke direktori parent
$ cd ..
# hapus direktori 'test' seisinya
$ rm -r test
```

```
# temukan file dengan nama 'fdisk' memakai `locate`
$ locate fdisk
# temukan file dengan nama 'fdisk' memakai `find`
$ find -name fdisk
# temukan file pada home anda yang ukurannya > 200 MB
$ find -size +200M
# temukan file pada home anda yang diubah < 3 hari
$ find -mtime -3
# temukan file pada home anda yang diakses > 30 hari
$ find -atime +30
```

```
# tampilkan 5 baris pertama keluaran perintah `last`
$ last | head -n 5
# tampilkan dua baris terakhir file '/etc/passwd'
$ last | tail -n 2 etc/passwd
# cari file di '/usr/include' yang memuat kata 'sem_post'
$ grep -r 'sem_post' usr/include
# tampilkan kolom 1 dan 5 dari file '/etc/passwd'
$ awk -F: '{print $1, $5}' etc/passwd
# tampilkan isi file '/etc/motd' dalam huruf kapital
$ awk '{print toupper{$0}}' NAMAFILE
```

```
# jalankan `cat /dev/random > rand.txt` di background
cat /dev/random > rand.txt &
# tampilkan daftar job
jobs
# kirim sinyal STOP ke job tersebut
kill -STOP %1 atau kill -STOP 6873 
# lanjutkan job tersebut di background
kill -CONT %1 atau kill -CONT 6873
# kirim sinyal TERM ke job tersebut
kill -TERM %1 atau kill -TERM 6873
```

```
# echo hostname uname date cal who
$ hostname [Laptop Blablabla]
$ uname [Linux]
$ date [nampilin date]
$ cal [buat calendar]
$ who [

# cd pwd ls touch
$ cd .. [Parent]
$ cd Folder
$ cd ~ [Home]
$ cd / [Root]
$ pwd [nampilin path]
$ touch [bikin file kalo blm ada]

# cp mv rm mkdir rmdir
$ mv Florigo2.jpeg Florigo3.kpeg [ganti nama file]
$ mv Florigo2.jpeg ../ [pindahin ke parent]
$ mv Florigo2.jpeg DIR/ [pindahin ke direktori DIR]
$ mv Florigo2.jpeg DIR/Florigo3.jpeg [pindain sekaligus ganti nama]
$ cp Florigo3.jpeg ../ [copy paste ke parent]
$ cp Florigo3.jpeg DIR/ [misal di DIR sudah ada Florigo3, dia akan ke overwrite]
$ cp -r FOLDER Folder2 [copy secara keseluruhan di FOLDER ke FOLDER2]
$ rmdir [hapus direktori kosong]
$ rm -r FOLDER [hapus folder ampe bawah bawahnya]
$ rmdir -p dir/test/ [jika dir punya folder test dan test tidak punya file apa apa]
$ cp -i Florigo3.jpeg DIR/ [ditanya dulu apakah mau overwrite?]
$ mkdir NAMAFOLDER

# chmod ln
$ 
$ 
 
# locate find wc
$ locate Florigo2.jpeg
$ find Florigo2.jpeg
$ echo 'wkwkwk' | wc

# cat head tail sort uniq cut tr grep sed
$ cat Florigo2.jpeg
$ head -n 5 Florigo2.jpeg
$ tail -n 5 Florigo2.jpeg
$ sort 
 
# ps nice renice pidof kill
$ 
$ 

# & jobs fg bg
$ COMMAND... & [Untuk menjalankan proses di background, tambahkan tanda & pada akhir perintah]
$ fg %JOB [Memindahkan job ke foreground]
$ jobs [Menampilkan job yg sedang berlangsung]
$ bg %JOB [Memindahkan job ke background]
```
