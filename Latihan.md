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
