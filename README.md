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

## CPT (VSLM)

### Topologi
<img alt="image" src="https://github.com/user-attachments/assets/7bdbde47-e6b9-4f12-a8b0-e504350bc8aa">

### Tree
<img alt="image" src="https://github.com/user-attachments/assets/d73ed795-277a-4704-b596-5fe773d84715">

### Pembagian IP

| Subnet	| Network ID	| Netmask	| Broadcast	| Range IP |
|----|-----|-----|-----|-----|
|A1	|10.78.18.128	|255.255.255.192	|10.78.18.191	|10.78.18.129 - 10.78.18.190|
|A2	|10.78.19.48	|255.255.255.248	|10.78.19.55	|10.78.19.49 - 10.78.19.54|
|A3	|10.78.19.56	|255.255.255.248	|10.78.19.63	|10.78.19.57 - 10.78.19.62|
|A4	|10.78.12.0	|255.255.254.0	|10.74.13.255|	|10.78.12.1 - 10.78.13.254|
|A5	|10.78.19.72	|255.255.255.252	|10.78.19.75|	10.78.19.73 - 10.78.19.74|
|A6	|10.78.19.76	|255.255.255.252	|10.78.19.79|	10.78.19.77 - 10.78.19.78|
|A7	|10.78.19.0	|255.255.255.224	|10.78.19.31	|10.78.19.1 - 10.78.19.30|
|A8	|10.78.19.80	|255.255.255.252|	10.78.19.83	|10.78.19.81 - 10.78.19.82|
|A9	|10.78.19.84	|255.255.255.252|	10.78.19.87	|10.78.19.85 - 10.78.19.86|
|A10|	10.78.19.88	|255.255.255.252|	10.78.19.91	|10.78.19.89 - 10.78.19.90|
|A11|	10.78.8.0	|255.255.252.0	|10.78.11.255	|10.78.8.1 - 10.78.11.254|
|A12|	10.78.19.92	|255.255.255.252|	10.78.19.95	|10.78.19.93 - 10.78.19.94|
|A13|	10.78.18.192|	255.255.255.192|	10.78.18.255|	10.78.18.193 - 10.78.18.254|
|A14|	10.78.19.96	|255.255.255.252	|10.78.19.99	|10.78.19.97 - 10.78.19.98|
|A15|	10.78.14.0	|255.255.254.0	|10.78.15.255	|10.78.14.1 - 10.78.15.245|
|A16|	10.78.19.100|	255.255.255.252	|10.78.19.103|	10.78.19.101 - 10.78.19.102|
|A17|	10.78.19.64	|255.255.255.248	|10.78.19.71	|10.78.19.65 - 10.78.19.70|
|A18|	10.78.19.32	|255.255.255.240	|10.78.19.47	|10.78.19.33 - 10.78.19.46|
|A19|	10.78.0.0	|255.255.248.0	|10.78.7.255	|10.78.0.1 - 10.78.7.245|
|A20|	10.78.16.0	|255.255.254.0	|10.78.17.255	|10.78.16.1 - 10.78.17.254|
|A21|	10.78.19.104|	255.255.255.252	|10.78.19.107|	10.78.19.105 - 10.78.19.106|
|A22|	10.78.18.0	|255.255.255.128	|10.78.18.127|	10.78.18.1 - 10.78.18.126|

### Konfigurasi

- Hololive
- Holo-EN
- Holo-ID
- Holo-Myth
- HoloAdvent
- Router4
- Holo-Council
- AREA15
- holoro
- holoh3ro
- Holo-JP
- DEV_IS
- GEN:0
- GEN:1
- GAMERS
- Kronii_Mumei
- Bae_Fauna
- Irys
- Gura_Ame_Ina
- Kiara_calli
- FuwaMoco
- Shiori_Nerissa
- Biboo
- Moona
- Risu
- lofi
- Ollie
- Anya
- Reine
- Zeta
- Kaela
- Kobo
- Ririka_Raden
- Ao
- Hajime_Kanade
- MiComent
- Sora_Robo_AZKi
- FBK_Matsuri
- Aki_Hachama
- Korone
- Okayu
- Mio
