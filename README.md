# Jarkom-Modul-4-IT29-2024

## Anggota Kelompok
| Nama | NRP |
|---------|---------|
| Harwinda | 5027231079   |
| Muhammad Syahmi Ash Shidqi | 5027231085 |

# GNS3 (CIDR)
## Topologi
![topologi-modul-4](https://github.com/user-attachments/assets/2f456ceb-deb6-45a2-bce6-430633b80916)

### Subnetting
<img width="491" alt="image" src="https://github.com/user-attachments/assets/c2dcf46f-d7ab-41dd-a35c-d0445fbc7739">

### Gabungan 2 (B)
<img width="572" alt="image" src="https://github.com/user-attachments/assets/8db58974-772e-4a7a-866a-d081b7c38e71">

<img width="442" alt="image" src="https://github.com/user-attachments/assets/19a0100e-22f8-4026-be20-37b0bc28260b">


### Gabungan 3 (C)

<img width="575" alt="image" src="https://github.com/user-attachments/assets/12409176-5524-456c-8158-d66932858080">

<img width="445" alt="image" src="https://github.com/user-attachments/assets/92bdf1af-2391-41d8-8c53-9fdfe8fe9485">


### Gabungan 4 (D)

<img width="581" alt="image" src="https://github.com/user-attachments/assets/b2685460-24b3-477e-ab67-d8968ac2af3a">

<img width="443" alt="image" src="https://github.com/user-attachments/assets/54efd0fe-4acc-438e-92f0-a89e46af4c8a">


### Gabungan 5 (E)

<img width="575" alt="image" src="https://github.com/user-attachments/assets/62c4ad35-0980-4d92-b836-2d5b065b9bab">

<img width="444" alt="image" src="https://github.com/user-attachments/assets/2d21dfa6-0639-48a2-85cf-5f530524d003">


### Gabungan 6 (F)

<img width="586" alt="image" src="https://github.com/user-attachments/assets/a1153f10-96c3-44a9-ac74-bea021684621">

<img width="443" alt="image" src="https://github.com/user-attachments/assets/f507496e-e281-49af-a4ec-790f82d23764">


### Gabungan 7 (G)

<img width="581" alt="image" src="https://github.com/user-attachments/assets/5ea4dd64-1a84-4dd1-9127-3cdb9549a5d0">

<img width="448" alt="image" src="https://github.com/user-attachments/assets/359281ca-d7b8-49ee-b1dc-987fb54b4902">




### Gabungan 8 (H)

<img width="437" alt="image" src="https://github.com/user-attachments/assets/c1210df8-71f4-43b4-bd27-326e8853ca0a">
<br>

<img width="445" alt="image" src="https://github.com/user-attachments/assets/79e06e9a-7883-4eb7-ae96-98176d33e98d">




### Gabungan 9 (I)

<img width="438" alt="image" src="https://github.com/user-attachments/assets/6f4da465-4862-48db-b593-eb9ba78f2451">
<br>

<img width="446" alt="image" src="https://github.com/user-attachments/assets/1d3f61c2-b529-497d-9795-c27024872b2c">




### Gabungan 10 (J)

<img width="440" alt="image" src="https://github.com/user-attachments/assets/d794dbe5-2e37-40ee-a5f0-faf5ea22a0eb">
<br>

<img width="443" alt="image" src="https://github.com/user-attachments/assets/b04ae076-20f2-4320-9ff9-973d7f543c13">


## Konfigurasi
### Hololive (Gateway)
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

### Holo-EN (Gateway)
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

### Holo-Myth (Gateway)
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

### Gura_Ame_Ina (Client)
```
#A4
auto eth0
iface eth0 inet static
    address 10.79.0.2
    netmask 255.255.254.0
    gateway 10.79.0.1
```




# CPT (VSLM)

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
```
Fa0/1:10.78.19.101 (A16)
Netmask: 255.255.255.252

Fa1/0: 10.78.19.81 (A8)
Netmask: 255.255.255.252

Fa1/1: 10.78.19.85 (A9)
Netmask: 255.255.255.252
```

- Holo-EN
```
Fa0/0: 10.78.19.82 (A8)
Netmask: 255.255.255.252

Fa0/1: 10.78.19.73 (A5)
Netmask: 255.255.255.252

Fa1/0: 10.78.19.77 (A6)
Netmask: 255.255.255.252
```

- Holo-ID
```
Fa0/0: 10.78.19.86 (A9)
Netmask: 255.255.255.252

Fa0/1: 10.78.19.93 (A12)
Netmask: 255.255.255.252

Fa1/0: 10.78.19.89 (A10)
Netmask: 255.255.255.252

Fa1/1: 10.78.19.97 (A14)
Netmask: 255.255.255.252
```

- Holo-Myth
```
Fa0/0: 10.78.19.74 (A5)
Netmask: 255.255.255.252

Fa0/1: 10.78.19.49 (A2)
Netmask: 255.255.255.248

Fa1/0: 10.78.12.1 (A4)
Netmask: 255.255.254.0
```

- HoloAdvent
```
Fa0/0: 10.78.19.78 (A6)
Netmask: 255.255.255.252

Fa0/1: 10.78.19.1 (A7)
Netmask: 255.255.255.224
```

- Router4
```
Fa0/0: 10.78.19.50 (A2)
Netmask: 255.255.255.248

Fa0/1: 10.78.19.57 (A3)
Netmask: 255.255.255.248
```

- Holo-Council
```
Fa0/0: 10.78.19.51 (A2)
Netmask: 255.255.255.248

Fa0/1: 10.78.18.129 (A1)
Netmask: 255.255.255.192
```

- AREA15
```
Fa0/0: 10.78.19.90 (A10)
Netmask: 255.255.255.252

Fa0/1: 10.78.8.1 (A11)
Netmask: 255.255.252.0
```

- holoro
```
Fa0/0: 10.78.19.94 (A12)
Netmask: 255.255.255.252

Fa0/1: 10.78.18.193 (A13)
Netmask: 255.255.255.192
```

- holoh3ro
```
Fa0/0: 10.78.19.97 (A14)
Netmask: 255.255.255.252

Fa0/1: 10.78.14.1 (A15)
Netmask: 255.255.254.0
```

- Holo-JP
```
Fa0/0: 10.78.19.102 (A16)
Netmask: 255.255.255.252

Fa0/1: 10.78.19.65 (A17)
Netmask: 255.255.255.248
```

- DEV_IS
```
Fa0/0: 10.78.19.66 (A17)
Netmask: 255.255.255.248

Fa0/1: 10.78.19.33 (A18)
Netmask: 255.255.255.240
```

- GEN:0
```
Fa0/0: 10.78.19.67 (A17)
Netmask: 255.255.255.248

Fa0/1: 10.78.0.1 (A19)
Netmask: 255.255.248.0
```

- GEN:1
```
Fa0/0: 10.78.7.242 (A19)
Netmask: 255.255.248.0

Fa0/1: 10.78.16.1 (A20)
Netmask: 255.255.254.0

Fa1/0: 10.78.19.105 (A21)
Netmask: 255.255.255.252
```

- GAMERS
```
Fa0/0: 10.78.19.106 (A21)
Netmask: 255.255.255.252

Fa0/1: 10.78.18.1 (A22)
Netmask: 255.255.255.128
```

- Kronii_Mumei
```
(A1) 
IPv4: 10.78.18.130
Netmask: 255.255.255.192
Gateway: 10.78.18.129
```

- Bae_Fauna
```
(A1) 
IPv4: 10.78.18.131
Netmask: 255.255.255.192
Gateway: 10.78.18.129
```

- Irys
```
(A3) 
IPv4: 10.78.19.58
Netmask: 255.255.255.248
Gateway: 10.78.19.57
```

- Gura_Ame_Ina
```
(A4) 
IPv4: 10.78.12.2
Netmask: 255.255.254.0
Gateway: 10.78.12.1
```

- Kiara_calli
```
(A4) 
IPv4: 10.78.13.56
Netmask: 255.255.254.0
Gateway: 10.78.12.1
```

- FuwaMoco
```
(A7) 
IPv4: 10.78.19.2
Netmask: 255.255.255.224
Gateway: 10.78.19.1
```

- Shiori_Nerissa
```
(A7) 
IPv4: 10.78.19.7
Netmask: 255.255.255.224
Gateway: 10.78.19.1
```

- Biboo
```
(A7) 
IPv4: 10.78.19.19
Netmask: 255.255.255.224
Gateway: 10.78.19.1
```

- Moona
```
(A11) 
IPv4: 10.78.8.142
Netmask: 255.255.252.0
Gateway: 10.78.8.1
```

- Risu
```
(A11) 
IPv4: 10.78.9.88
Netmask: 255.255.252.0
Gateway: 10.78.8.1
```

- lofi
```
(A11) 
IPv4: 10.78.8.2
Netmask: 255.255.252.0
Gateway: 10.78.8.1
```

- Ollie
```
(A13) 
IPv4: 10.78.18.194
Netmask: 255.255.255.192
Gateway: 10.78.18.193
```

- Anya
```
(A13) 
IPv4: 10.78.18.214
Netmask: 255.255.255.192
Gateway: 10.78.18.193
```

- Reine
```
(A13) 
IPv4: 10.78.18.217
Netmask: 255.255.255.192
Gateway: 10.78.18.193
```

- Zeta
```
(A15) 
IPv4: 10.78.14.2
Netmask: 255.255.254.0
Gateway: 10.78.14.1
```

- Kaela
```
(A15) 
IPv4: 10.78.14.83
Netmask: 255.255.254.0
Gateway: 10.78.14.1
```

- Kobo
```
(A15) 
IPv4: 10.78.14.154
Netmask: 255.255.254.0
Gateway: 10.78.14.1
```

- Ririka_Raden
```
(A18) 
IPv4: 10.78.19.34
Netmask: 255.255.255.240
Gateway: 10.78.19.33
```

- Ao
```
(A18) 
IPv4: 10.78.19.37
Netmask: 255.255.255.240
Gateway: 10.78.19.33
```

- Hajime_Kanade
```
(A18) 
IPv4: 10.78.19.40
Netmask: 255.255.255.240
Gateway: 10.78.19.33
```

- MiComent
```
(A19) 
IPv4: 10.78.0.2
Netmask: 255.255.248.0
Gateway: 10.78.0.1
```

- Sora_Robo_AZKi
```
(A19) 
IPv4: 10.78.5.228
Netmask: 255.255.248.0
Gateway: 10.78.0.1
```

- FBK_Matsuri
```
(A20) 
IPv4: 10.78.16.2
Netmask: 255.255.254.0
Gateway: 10.78.16.1
```

- Aki_Hachama
```
(A20) 
IPv4: 10.78.17.68
Netmask: 255.255.254.0
Gateway: 10.78.16.1
```

- Korone
```
(A22) 
IPv4: 10.78.18.2
Netmask: 255.255.255.128
Gateway: 10.78.18.1
```

- Okayu
```
(A22) 
IPv4: 10.78.18.53
Netmask: 255.255.255.128
Gateway: 10.78.18.1
```

- Mio
```
(A22) 
IPv4: 10.78.18.85
Netmask: 255.255.255.128
Gateway: 10.78.18.1
```
