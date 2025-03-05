# Pelatihan Linux 2025

#### 1. Mengunduh program wget, unzip, xxd & membuat folder "artists_who_can_sing"
```
sudo apt install wget ; sudo apt install unzip ; sudo apt install xxd ; mkdir artist_who_can_sing && cd artist_who_can_sing
```

#### 2. Mendownload file zip menggunakan wget
```
wget -O tutorials.zip "https://drive.usercontent.google.com/u/0/uc?id=1lV1HVmPTY_BOAK6ToXymRu7V5eVfR0ut&export=download"
```
#### 3. unzip ke folder “singing_tutorials”
```
unzip tutorials.zip -d singing_tutorials
```
#### 4. Masuk ke dalam folder & menampilkan list file & melihat list file yang tersembunyi
```
cd singing_tutorials/ && ls -a
```
#### 5. Mencari file “opera” dibuat oleh “NBAYoungboy” & dimasukkan ke folder “flag.txt”
```
strings .*opera*NBAYoungboy* | grep -a "FLAG{" > ../flag.txt
```
#### 6. Mengambil flag yang telah ditemukan lalu mundur 1 dir dan mengunduh file “plsrunmeiamnotmalwarefr”
```
cd .. && wget -O plsrunmeiamnotmalwarefr "https://files.catbox.moe/9l4qu8"
```
#### 7. Izin execute dan menjalankan program
```
 chmod +x plsrunmeiamnotmalwarefr && ./plsrunmeiamnotmalwarefr
```
#### 8. Melihat program yang dijalankan menggunakan command di terminal linux
```
ps aux
```
#### 9. Membuat file bernama ransom.moolah && mengecek keadaan
```
touch ransom.moolah && ps aux
```
#### 10. Mematikan process tersebut & memastikan bahwa programnya sudah mati.
```
kill -9 <PID> && ps aux
```
#### 11. Membuat user “yabadabadoo" dalam sudoers group & login sebagai user
```
sudo adduser yabadabadoo && sudo usermod yabadabadoo -aG sudo && su - yabadabadoo
```
