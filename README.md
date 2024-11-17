# Jarkom-Modul-4-IT29-2024

## Anggota Kelompok
| Nama | NRP |
|---------|---------|
| Harwinda | 5027231079   |
| Muhammad Syahmi Ash Shidqi | 5027231085 |

# Topologi
## GNS3 (CIDR)
![topologi-modul-4](https://github.com/user-attachments/assets/2f456ceb-deb6-45a2-bce6-430633b80916)

## Subnetting
<img width="491" alt="image" src="https://github.com/user-attachments/assets/c2dcf46f-d7ab-41dd-a35c-d0445fbc7739">

## Gabungan 2 (B)
<img width="572" alt="image" src="https://github.com/user-attachments/assets/8db58974-772e-4a7a-866a-d081b7c38e71">

## Gabungan 3 (C)
<img width="575" alt="image" src="https://github.com/user-attachments/assets/12409176-5524-456c-8158-d66932858080">

## Gabungan 4 (D)
<img width="581" alt="image" src="https://github.com/user-attachments/assets/b2685460-24b3-477e-ab67-d8968ac2af3a">

## Gabungan 5 (E)
<img width="575" alt="image" src="https://github.com/user-attachments/assets/62c4ad35-0980-4d92-b836-2d5b065b9bab">

## Gabungan 6 (F)
<img width="586" alt="image" src="https://github.com/user-attachments/assets/a1153f10-96c3-44a9-ac74-bea021684621">

## Gabungan 7 (G)
<img width="581" alt="image" src="https://github.com/user-attachments/assets/5ea4dd64-1a84-4dd1-9127-3cdb9549a5d0">

## Gabungan 8 (H)
<img width="437" alt="image" src="https://github.com/user-attachments/assets/c1210df8-71f4-43b4-bd27-326e8853ca0a">

## Gabungan 9 (I)
<img width="438" alt="image" src="https://github.com/user-attachments/assets/6f4da465-4862-48db-b593-eb9ba78f2451">

## Gabungan 10 (J)
<img width="440" alt="image" src="https://github.com/user-attachments/assets/d794dbe5-2e37-40ee-a5f0-faf5ea22a0eb">

# Konfigurasi
## Hololive (Gateway)
```
#A8
auto eth1
iface eth1 inet static
    address 10.79.16.1
    netmask 255.255.255.252

#A9
auto eth2
iface eth2 inet static
    address 10.78.160.1
    netmask 255.255.255.252

#A16
auto eth3
iface eth3 inet static
    address 10.78.64.1
    netmask 255.255.255.252
```

## Holo-EN (Gateway)
```
#A8
auto eth0
iface eth0 inet static
    address 10.79.16.2
    netmask 255.255.255.252
    gateway 10.79.16.1 #ip sebelumnya

#A5
auto eth1
iface eth1 inet static
    address 10.79.4.1
    netmask 255.255.255.252

#A6
auto eth2
iface eth2 inet static
    address 10.79.8.33
    netmask 255.255.255.252
```

## Holo-Myth (Gateway)
```
#A5
auto eth0
iface eth0 inet static
    address 10.79.4.2
    netmask 255.255.255.252
    gateway 10.79.4.1

#A4
auto eth1
iface eth1 inet static
    address 10.79.0.1
    netmask 255.255.254.0


#A2
auto eth2
iface eth2 inet static
    address 10.79.2.129
    netmask 255.255.255.248
```

## Gura_Ame_Ina (Client)
```
#A4
auto eth0
iface eth0 inet static
    address 10.79.0.2
    netmask 255.255.254.0
    gateway 10.79.0.1
```

## VSLM
<img alt="image" src="https://github.com/user-attachments/assets/7bdbde47-e6b9-4f12-a8b0-e504350bc8aa">

<img alt="image" src="https://github.com/user-attachments/assets/d73ed795-277a-4704-b596-5fe773d84715">
