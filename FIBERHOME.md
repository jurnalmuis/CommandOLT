## OLT FIBERHOME
### Command Untuk Pengecekan di OLT Huawei
Masuk ke Folder ONU
````bash
cd onu
````
Cek berdasarkan VLAN
````bash
show onu service by svlan XXXX
slot pon onu domainname/FE/VEIP-serv       svlan cvlan 
----------------------------------------- 
18    4   1   1   FE/1                     XXXX
````
Cek Status ONT
````bash
show onu_state slot 18 pon 4 onu 1
SLOT 18 PON  4 ONU   1 status : active. >> Active : Modem Working
````
Cek Log ONT
````bash
show onu state-info slot 18 pon 4 onu 1
````
Cek Config ONT
````bash
show onu service-info slot 18 pon 4 onu 1
````
Cek ONT sudah on berapa lama
````bash
show onu_time slot 18 pon 4 onu 1
````
Cek Mac Address berdasarkan VLAN
````bash
show mac-address vlan XXXX
````
Cek SN ONT
````bash
show running-config slot 18 pon 4 onu 1
````
Cek WAN ONT
````bash
cd onu/lan
show onu_wan_service slot 18 pon 4 onu 1
````