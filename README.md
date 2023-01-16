# Tutorial_contribute_scroll
menjadi early contributor di scroll via vps

# Update dan install go (jika belum)
Pertama, mari kita pastikan mesin linux up-to-date.
```
sudo apt update && sudo apt upgrade -y
```
Optional (jika belum install go)
```
sudo apt install golang-go
```
Pastikan go version
```
go version
```

# Eksekusi
sekarang kita download KZGCLI
```
wget https://github.com/jsign/go-kzg-ceremony-client/releases/download/v1.0.1/kzgcli-v1.0.1-linux-amd64.tar.gz -O kzgcli.tar.gz
```
ekstrak binary nya
```
tar xvf kzgcli.tar.gz
```
setelahnya anda bisa memindahkan nya ke usr/local/bin agar mudah di eksekusi dari directory manapun
```
sudo mv kzgcli /usr/local/bin
```
masuk ke local
```
cd /usr/local/bin
```
export path nya
```
chmod +x kzgcli
```

# Contribute
Buka https://github.com/jsign/go-kzg-ceremony-client lalu klik link seperti dibawah :

![image](https://user-images.githubusercontent.com/41656124/212543362-6dc3db17-6c97-4fee-abf9-e9b9e58c12fe.png)

Akan ada 2 plihan, tergantung anda mau tandatangan dengan github atau metamask.
copy link nya buka di website baru dan ikuti langkah verifikasi nya, maka akan menghasilkan session id :

![image](https://user-images.githubusercontent.com/41656124/212543700-93fe1d90-2572-4ec7-8e0d-13f92125e751.png)

simpan baik baik session id nya...

Buat screen
```
screen -S contribute
```
contribute
```
kzgcli contribute --session-id <paste-your-session-id>
```
silahkan save screen anda dengan ctrl a + d karena contribute membutuhkan waktu yang lama, 
ketika nanti sudah selesai maka akan auto generate file json, nah setelah itu simpan baik baik file tersebut
Berikut contoh kalau sudah selesai 

![image](https://user-images.githubusercontent.com/41656124/212679955-a11c09d3-5915-4564-b183-2a8ab7231438.png)

simpan baik baik isi dari contribute_receipt.json tersebut.

..

cara balik ke screen untuk cek apakah sudah selesai atau belum, jika belum ya tinggal ctrl a+d aja..
```
screen -Rd contribute
```

