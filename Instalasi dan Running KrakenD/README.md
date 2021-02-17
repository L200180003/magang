Cara Install KrakenD di Ubuntu
1. Buka terminal
2. Tambahkan key
   apt-key adv --keyserver keyserver.ubuntu.com --recv 5DE6FD698AD6FDD2 
3. Tambahkan repo ke sources.list
   echo "deb https://repo.krakend.io/apt stable main" | tee /etc/apt/sources.list.d/krakend.list
4. Update package list
   apt-get update 
5. Install KrakenD service
   apt-get install -y krakend 
*NOTE : Untuk cara install di OS lain :  https://www.krakend.io/docs/overview/installing/


Cara Running KrakenD 
1. Buat file JSON di https://designer.krakend.io, disini saya mencoba running dengan example file dari https://github.com/devopsfaith/krakend-ce/blob/master/krakend.json
2. Buka terminal dan masuk ke folder dimana file JSON berada
3. Jalankan perintah berikut
   krakend run -c krakend.json
 
