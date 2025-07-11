# belajar git 

1. inisialisasi git 
```
git init
```

2. mengatur versi remote dari repository saat ini 
```bash
git remote add <aliasRemote> <urlRemote>
git remote add origin https://github.com/M16Yusuf/belajar-git.git
# Melihat list remote
git remote
# megambil link/url dari remote repo
git remote get-url <aliasRemote>
# melakukan perubahan link
git remote set-url <aliasRemote> <urlBaru>
```

3. Melakukan penyimpanan sementara dari working directory ke staging area
```bash
git add ./src/1.txt
# atau
git add ./src
```

> titik pada direktori merujuk pada current direktori saat ini

4. git commit
penympanan permanen dari staging ke area local repository
menggunakan pesan singkat (option:m)

```bash
git commit -m "pesan commit"

git commit 

```


5. git push
```bash
git push <option> <aliasRemote> <branchlocal>

git push origin master
# jika mau ditambah dengan penyimpanan opsi remote dan branch (option: U) upstream => remote and bragnch
git push -u origin master
```


6. git pull
kalau sudah ada -u
git pull 
kalau belum ada -u
git pull origin master

```bash
git pull <aliasRemote> <branch>
```

7. git reverte
```bash
git reverte <commit-id>
```


8. git reset
```bash
git reset <relative position>

```


9. Branch
```bash
# melihat list branch
git branch
# buat branch "cabang"
git branch cabang 
# pindah ke branch "cabang"
git checkout cabang
# hapus branch "cabang"
git branch -d cabang
# rename branch dari cabang ke "bacang"
git branch -m cabang bacang
```


10. git checkout 
```bash
# pindah ke branch "cabang"
git checkout cabang
# berpindah cabang ke yang tidak ada 
git checkout -b <branchname>
```

11. git merge 
```bash
# menggabungkan 
git merge <...branchname>
```



Status file git di vs code
1. U => untrackerd 
file ada didir tapi tidak tersimpan didalam histori git
2. A => index added 
suatu file ditambahkan ke dalam staging area (belum tersimpan di repository)
3. <no stastus> => sudah ditambahkan/tersimpan di ddalam repository
4. M => suatu file yang sudah terdaftar di remote repository mengalami perubahan
