# Judul Aplikasi
...

## Deskripsi Masalah
Sulitnya orang untuk mengetahui kondisi rute ke tempat yang akan dituju

## Deskripsi Solusi
Membuat suatu media dimana user dapat mengunggah kondisi di suatu wilayah dengan keterangan waktu, foto, deskripsi, dan titik lokasi

## Use Case
- User 1 dapat mengunggah kondisi di suatu wilayah
- User 2 dapat mengetahui unggahan User 1 berdasarkan lokasi yang dicari, daftar unggahan disortir berdasarkan unggahan terbaru

## Struktur Data

### posts
Nama Atribut | Tipe Data | Contoh
---|---|---
id | UUID | 422fea1c-252b-4b93-a8f5-3988db287d38
description | String | Terjadi kecelakaan di sekitar jalan soekarno hatta yang menyebabkan kemacetan hingga lampu merah buah batu
coordinates | Geometry(POINT) | POINT (107.619125 -5.917464)
createdAt | Timestamp | 2022-10-18 18:51:33.380 +0700
updatedAt | Timestamp | 2022-10-18 18:51:33.380 +0700
user_id | UUID | 5fea61b6-e2e1-4aad-9abf-765110218fad

### users
Nama Atribut | Tipe Data | Contoh
---|---|---
id | UUID | 5fea61b6-e2e1-4aad-9abf-765110218fad
username | String | farhanrizkyyyy
password | String | d1bbb2af69fd350b6d6bd88655757b47
name | String | Farhan Rizky
phone_number | String | 083824289159
address | String | Banjaran
token | String | eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6ImZhcmhhbnJpemt5eXl5IiwiaWF0IjoxNjY2MTM4NjU5LCJleHAiOjE2NjYxNDU4NTl9.BBkjnWT--2G_ilvxZx8TKxvm8nsP0aAe1gqIJIdGmNk
role_id | Integer | 2

### routes
Nama Atribut | Tipe Data | Contoh
---|---|---
id | UUID | 151d561f-e02a-497d-bc2d-a7c3967c3894
from | Geometry(POINT) | POINT (107.579225 -7.046725)
to | Geometry(POINT) | POINT (107.5549014 -7.0058198)
route | Geometry(LINESTRING) | LINESTRING (107.579225 -7.046725, 107.5549014 -7.0058198)

### roles
Nama Atribut | Tipe Data | Contoh
---|---|---
id | Integer | 2
name | String | User


## Mockup UX
