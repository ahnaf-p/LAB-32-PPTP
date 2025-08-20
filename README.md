# LAB-32-PPTP
Rabu 20 Agustus 2025  
  
# Point to Point Tunnel Protocol  
  PPTP di Mikrotik dapat dikonfigurasi menjadi PPTP server dan PPTP client atau langsung bersamaan keduanya. Untuk melihat service PPTP ini aktif atau tidak, kita bisa cek di **system > package > PPP**.  
![](IMAGES/)  
  
  PPTP adalah protokol jaringan yang memungkinkan kita untuk mengirimkan paket data atau membuat sebuah koneksi melalui internet yang bersifat secure. Fungsi PPTP, misalnya kita ingin menghubungkan antara kantor A dan B dan kita ingin menghubungkan kedua kantor tersebut melalui jaringan internat, maka cara yang paling mudah dan bsia dikatakan aman adalah mengunakan PPTP.  

# Konfigurasi PPTP  
![](IMAGES/)  
  
1. Kita masuk ke **PPP > Interface > PPTP Server**, lalu pastikan **Enable** nya di checklist dan default profilenya **default-encryption**.  
![](IMAGES/)  
2. Selanjutnya kita akan membuat akun untuk login, pergi ke **PPP > secret > add**. Isi name, password untuk login client. Untuk service PPTP ini ada 2 pilihan, yaitu **any** dan **pptp**, kita akan memilih yang lebih spesifik yaitu **pptp**. Profile kita pilih yang **default encryiption**, Local address itu merupakan alokasi IP Address yang akan didapat oleh PPTP server dan Remote address merupakan alokasi IP yang diberikan ke PPTP client. Untuk addressnya kita isi sesuai topologi.  
![](IMAGES/)  
3. Sampai disini, proses pembuatan PPTP server pada Office A sudah selesai.  

- WIP
