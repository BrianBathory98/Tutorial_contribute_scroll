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
buka https://github.com/jsign/go-kzg-ceremony-client lalu klik link seperti dibawah
(https://web.whatsapp.com/dfe7f4b0-9eba-4ab8-8066-2f524d3534e7)
