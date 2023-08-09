# COMMAND OLT

Isi hanya command untuk pengecekan OLT ZTE, HUAWEI, FIBERHOME.
> [!NOTE]
> UPDATE JIKA SENGGANG.

[OLT ZTE](ZTE.md)

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

## OLT HUAWEI
### Command Untuk Pengecekan di OLT Huawei
Masuk privilege Mode
```
enable
```

Cek berdasarkan VLAN
````bash
display vlan XXXX
````
````bash
-------------------------------------------------------------------
INDEX  TYPE  STATE   F /S /P   VPI  VCI   FLOWTYPE FLOWPARA   CVLAN
2310   gpon   *up*   0 /1 /2   14   1     vlan     201        -        >> State UP, ONT UP.
````
**NOTE**

F = x

S = y

P = z

VPI = a

Cek Display ONT
````bash
display ont info x y z a
````

Cek Config ONT
````bash
display current-configuration ont x/y/z a
````

Cek Redaman ONT
````bash
config  >> Masuk ke config Mode
interface gpon x/y
display ont optical-info z a
````

Cek Port / Lan yang Connect.
````bash
config  >> Masuk ke config Mode
interface gpon x/y
display ont port state z a eth-port all
````

Cek Mac Address berdasarkan vlan
````bash
display mac-address vlan XXXX
````

Cek Port ONT berdasarkan SN ONT
````bash
display ont info by-SN XXXXXXXXXXXXX
````

Cek Service ONT
````bash
display service-port port x/y/z ont a
````

## OLT FIBERHOME
### Command Untuk Pengecekan di OLT Huawei
