# Latihan Membuat Database


## Tugas Praktikum 

#### 1. Buat sebuah database dengan nama latihan2!

![gambar 1](https://user-images.githubusercontent.com/115770247/232519325-51732a4c-1106-404a-975f-58ec59e9318c.png)

### Penjelasan:
 `CREAT DATABASE nama_database;` untuk membuat database baru. 
Dan `SHOW DATABASES;` Untuk melihat database yg kalian punya.

#### 2. Buat sebuah tabel dengan nama biodata (nama, alamat) didalam database latihan1!
#### 3. Tambahkan sebuah kolom keterangan (varchar 15), sebagai kolom terakhir!

![gambar 2](https://user-images.githubusercontent.com/115770247/232519849-4edbc6e1-8cfe-4362-aa4a-72fb9237c5d6.png)

### Penjelasan:
- `USE latihan2;` Digunakan Untuk mengunakan databes.
- `CREATE TABLE;` Digunakan untuk membuat sebuah table.
- `SHOW TABLES;` Digunakan  untuk melihat table di dalam database. 
- `DESC biodata;` Digunkan Untuk melihat table yg bernama biodata.

#### 4. Tambahkan kolom id (int 11) di awal (sebagai kolom pertama)!



![gambar 3](https://user-images.githubusercontent.com/115770247/232520330-865723df-912b-4d2d-8bc3-3b9d09c639c8.png)


### Penjelasan:
- `ALTER TABLE biodata ADD COLUMN id INT(11) FIRST;` Add field id dengan integer maks 11 angka, di atas Kolom Nama.

#### 5. Sisipkan sebuah kolom dengan nama phone (varchar 15) setelah kolom alamat!

![gambar 4](https://user-images.githubusercontent.com/115770247/232520488-e5634a39-cdb1-483a-8a14-8064b4bb39cf.png)


### Penjelasan:
- `ALTER TABLE biodata ADD COLUMN Phone VARCHAR(15) AFTER Alamat;` Add field Phone dengan VARCHAR(50), setelah kplom Alamat.

#### 6. Ubah tipe data kolom id menjadi char(11)!

![gambar 5](https://user-images.githubusercontent.com/115770247/232520579-1d9e7433-1e5c-43e3-a36d-39020c411f7d.png)


### Penjelasan: 
- `ALTER TABLE biodata MODIFY id CHAR(11);` Mengubah type id dari INT ke CHAR.

#### 7. Ubah nama kolom phone menjadi hp (varchar 20)!
#### 8. Tambahkan kolom email setelah kolom hp.

![gambar 6](https://user-images.githubusercontent.com/115770247/232520910-0d61a311-51c9-437c-81fa-30cf4e41dff5.png)


### Penjelasan:
- `ALTER TABLE biodata CHANGE Phone Ph VARCHAR(20);` Ubah field Phone menjadi Ph. 
- `ALTER TABLE biodata ADD COLUMN Email VARCHAR(50) AFTER Hp;` Add Kolom/field Email di bawah Hp.

#### 9. Hapus kolom keterangan dari tabel!
#### 10. Ganti nama tabel menjadi data_mahasiswa!
#### 11. Ganti nama field id menjadi nim!


![gambar 7](https://user-images.githubusercontent.com/115770247/232521092-7bcd07df-3094-46ed-8ab6-9c1c95530bd7.png)


### Penjelasan:
- `ALTER TABLE biodata DROP Keterangan;` Hapus field Keterangan dari table biodata.
- `ALTER TABLE biodata RENAME data_mahasiswa;` Mengganti nama table biodata menjadi data_mahasiswa.
- `ALTER TABLE data_mahasiswa CHANGE id NIM char(11);` Ubah kolom/field id menjadi NIM dengan char/string, maks 11 kata.

#### 12. Jadikan nim sebagai PRIMARY KEY!
#### 13. Jadikan kolom email sebagai UNIQUE KEY


![gambar 8](https://user-images.githubusercontent.com/115770247/232521303-be250bdc-0fb6-4a5d-8d1e-0ef44ceaed7d.png)


### Penjelasan:
- `ALTER TABLE data_mahasiswa ADD PRIMARY KEY (NIM);` Menjadikan data_mahasiswa menjadi PRIMARY KEY.
- `ALTER TABLE data_mahasiswa ADD UNIQUE KEY (Email);` Menjadikan Email sebagai UNIQUE KEY.
