# Konfigurasi dasar file JSON di KrakenD
Kali ini saya akan membuat konfigurasi file JSON sederhana yang mengambil data dari jsonplaceholder yang akan di tampilkan di lokal. 
1. Buka https://designer.krakend.io/ untuk melakukan konfigurasi file JSON. 
2. Langkah pertama yang perlu dilakukan adalah melakukan konfigurasi, untuk konfigurasi yang saya gunakan :
  - Service name : coba
  - Port : 7878
  - Host : https://jsonplaceholder.typicode.com/
3. Selanjutnya adalah konfigurasi endpoint. Disini saya mencoba mengambil data user yang ditampilkan berdasarkan ID.
- KrakenD Endpoint (yang menjadi endpoint di lokal) : /users/{id} 
- Add Backend Query (konfigurasi backend) : select host yang sudah ditambahkan yaitu https://jsonplaceholder.typicode.com/ dan pada Backend endpoint isi dengan /users/{id} yang mengarah pada data users di jsonplaceholder
4. Setelah selesai, download file JSON. Kemudian run di terminal dengan perintah krakend run -c coba_krakenD.json
5. Untuk mengecek apakah konfigurasinya berhasil, buka alamat http://localhost:7878/users/1 di browser
