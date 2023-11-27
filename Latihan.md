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
$ cp '/etc/timezone'
# ubah nama file 'timezone' menjadi 'tz.txt'
$ mv timezone tz.txt
# list isi direktori ini
$ ls
# pindah ke direktori parent
$ cd ..
# hapus direktori 'test' seisinya
$ rmdir test
```

```
# temukan file dengan nama 'fdisk' memakai `locate`
$ locate fdisk
# temukan file dengan nama 'fdisk' memakai `find`
...
# temukan file pada home anda yang ukurannya > 200 MB
...
# temukan file pada home anda yang diubah < 3 hari
...
# temukan file pada home anda yang diakses > 30 hari
...
```

```
# tampilkan 5 baris pertama keluaran perintah `last`
$ last
# tampilkan dua baris terakhir file '/etc/passwd'
$ 
# cari file di '/usr/include' yang memuat kata 'sem_post'
$ 
# tampilkan kolom 1 dan 5 dari file '/etc/passwd'
$ head 
# tampilkan isi file '/etc/motd' dalam huruf kapital
$ 
```
