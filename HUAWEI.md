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

INDEX  TYPE  STATE   F /S /P   VPI  VCI   FLOWTYPE FLOWPARA   CVLAN
2310   gpon **up**   0 /1 /2   14   1     vlan     201        -        >> State UP, ONT UP.



display ont info **F S P VPI**