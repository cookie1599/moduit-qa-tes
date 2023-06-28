# moduit-qa-tes

Repository ini berisikan collection api dari website `https://reqres.in/`.


# Cara Menjalankan API Test Menggunakan Postman

sebelum menjalankan API Test pada Postman ini jangan lupa untuk
memasukan collection Moduit.postman_collection.json pada collection dan
memasukan envirotment url Envirotment URL.postman_environment.json.
berikut adalah cara menjalankan API Test menggunakan postman



**1. Menjalankan test untuk membuat user baru / POST Create User**

```
Buka postman lalu pilih collection POST isi dengan url `{{reqres}}api/users`. 
Setelah itu isi Body dengan tipe raw lalu pilih tipe data Json, lalu data json di isi dengan
{"name": "morpheus", "job": "leader"} lalu klik send. setelah itu akan memberikan 
response code 200 atau berhasil membuat user.

```

**2. Menjalankan test untuk read user / GET list user**

```
Buka postman lalu pilih collection GET isi dengan url `{{{reqres}}api/users?page=1`.
Setelah itu isi Parameters / Params dengan Key page dan value 1 lalu klik send.
setelah itu akan memberikan response code 200 / berhasil menampilkan list user.
```

**3. Menjalankan test untuk Update user / PUT list user**

```
Buka postman lalu pilih collection PUT isi dengan url `{{reqres}}api/users/2`.
Setelah itu isi Body dengan tipe raw lalu pilih tipe data Json, lalu data json diisi dengan 
{"name": "morpheus","job": "zion resident"} lalu klik send. setelah itu akan muncul 
response code 200 atau berhasil update data user.
```

**4. Menjalankan test untuk Menghapus user/DEL user**

```
Buka postman lalu pilih collection Delete user isi dengan url `{{reqres}}api/users/2`.
Setelah itu klik send. Nanti akan muncul response code 204 atau berhasil menghapus user dengan id 2.
```

