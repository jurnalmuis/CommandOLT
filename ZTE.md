## OLT ZTE
### Command Untuk Pengecekan di OLT ZTE
Cek berdasarkan VLAN 
```bash
show vlan XXXX
```

Cek Mac Address berdasarkan VLAN
````bash
show mac vlan XXXX
````

Cek Mac Address berdasarkan interface 
````bash
show mac gpon onu gpon-onu_x/y/z:a
````

Cek Detail ONT
```bash
show gpon onu detail-info gpon-onu_x/y/z:a
```

Cek Config Interface ONT
```bash
show onu running config gpon-onu_x/y/z:a
```

Cek Config ONT
````bash
show running-config interface gpon-onu_x/y/z:a
````

Cek Redaman ONT
````bash
show pon power attenuation gpon-onu_x/y/z:a
````

Cek Interface berdasarkan SN Modem
````bash
show gpon onu by sn ZTEXXXXXXXXX
````

Cek ONT Untag
````bash
show gpon onu uncfg
````

Cek Traffic ONT
````bash
show interface gpon-onu_x/y/z:a
````

Cek VOIP / TELP
````bash
show gpon remote-onu voip-linestatus gpon-onu_x/y/z:a
````

Cek Port / LAN ONT
````bash
show gpon remote-onu interface eth gpon-onu_x/y/z:a
````

Cek Status ONT [ **Working** = Link UP, **LOS** = Link Down]
````bash
show gpon onu state gpon-olt_x/y/z a
````
