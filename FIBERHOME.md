## OLT FIBERHOME
### Command Untuk Pengecekan di OLT Huawei
Cek berdasarkan VLAN
````bash
cd onu
show onu service by svlan XXXX
slot pon onu domainname/FE/VEIP-serv       svlan cvlan 
----------------------------------------- 
18    4   1   1   FE/1                     XXXX
````
Cek Status ONT
````bash
cd onu
show onu_state slot 18 pon 4 onu 1
SLOT 18 PON  4 ONU   1 status : active. >> Active : Modem Working
````
Cek Log ONT
````bash
cd onu
show onu state-info slot 18 pon 4 onu 1
````
Cek Config ONT
````bash
cd onu
show onu service-info slot 18 pon 4 onu 1
````
Cek ONT sudah on berapa lama
````bash
cd onu
show onu_time slot 18 pon 4 onu 1
````
Cek WAN ONT
````bash
cd onu/lan
show onu_wan_service slot 18 pon 4 onu 1
````
Cek Redaman ONT
````bash
cd onu
show optic_module slot 18 pon 4 onu 1
atau
show onu optical-info slot 18 pon 4 onu all
````
Cek Mac Address berdasarkan VLAN
````bash
show mac-address vlan XXXX
````
Cek SN ONT
````bash
show running-config slot 18 pon 4 onu 1
````
Cek Port berdasarkan SN ONT
````bash
show onu-info by XXXXXXXXXXXX
````
