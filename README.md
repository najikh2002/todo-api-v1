# Todo API v1 

Ini adalah Todo API sederhana yang dibangun dengan FastAPI bertujuan agar mempermudah kita dalam management pekerjaan yang mencakup otentikasi JWT (JSON Web Token) untuk akses yang aman.

## Fitur

- **Operasi CRUD Todo**: Melakukan operasi CRUD (Create, Read, Update, Delete) dasar untuk Todos.
- **Otentikasi JWT**: Secara aman mengamankan API Anda dengan otentikasi berbasis JWT.

## Persyaratan

- Python 3.x (Recomended 3.9.9)
- [FastAPI](https://fastapi.tiangolo.com/)
- [Uvicorn](https://www.uvicorn.org/)
- [Pydantic](https://pydantic-docs.helpmanual.io/)
- [MongoDB](https://www.mongodb.com/developer/languages/python/python-quickstart-fastapi/)

## Instalasi 
Masukkan beberapa perintah berikut ke dalam terminal:

1. Clone repositori:

   ```
   git clone https://github.com/najikh2002/todo-api-v1.git
   ```
2. Masuk pada folder project

    ```
    cd todo-api-v1
	```
3. Aktifkan lingkungan virtual agar paket yang dipasang masuk ke lingkungan virtual (tidak masuk langsung ke penyimpanan lokal)
    **Untuk operasi sistem Linux**
    ```
    source env/bin/activate    
    ```
    **Untuk operasi sistem Windows**
    ```
    env\Scripts\activate.bat 
    ```
4. Masuk ke folder *backend*
	```
    cd backend
    ```
5. Jalankan api-nya yang ada di app/app.py menggunakan *uvicorn*
	```
    uvicorn app.app:app
    ```

## Endpoint 
Untuk penggunaan api dibagi menjadi tiga yaitu CRUD, USERS dan Otentikasi JWT
#### todo (CRUD)
`GET` **/api/v1/todo :** Mengambil seluruh todo dari user

`POST` **/api/v1/todo/create :** Membuat todo

`GET` **/api/v1/todo/{todo_id} :** Mengambil todo dari todo_id

`PUT` **/api/v1/todo/{todo_id} :** Mengubah todo dari todo_id

`DELETE` **/api/v1/todo/{todo_id} :** Menghapus todo dari todo_id

#### users
`POST` **/api/v1/users/create :** Membuat user baru

`GET` **/api/v1/users/me :** Mendapat detail identitas sesuai user yang login

`POST` **/api/v1/users/update :** Memperbarui user

#### auth (Otentikasi JWT)
