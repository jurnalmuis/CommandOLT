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
> x = F | y = S | z = P | a = VPI

Cek Display ONT
````bash
display ont info F S P VPI
````

Cek Config ONT
````bash
display current-configuration ont x/y/z a
````

Cek Redaman ONT
````bash
config
interface gpon x/y
display ont optical-info z a
`````