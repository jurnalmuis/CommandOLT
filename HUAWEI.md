## OLT HUAWEI
### Command Untuk Pengecekan OLT Huawei
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