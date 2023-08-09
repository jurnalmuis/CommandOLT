=================== OLT ZTE ===================

Mencari Interface berdasarkan VLAN 
```bash
show vlan XXXX
```

Melihat Mac Address berdasarkan VLAN
````bash
show mac vlan XXXX
````

Melihat Mac Address berdasarkan interface 
````bash
show mac gpon onu gpon-onu_X/Y/Z:A
````

Melihat Detail ONT
```bash
show gpon onu detail-info gpon-onu_X/Y/Z:A
```

Melihat Config ONT
```bash
show onu running config gpon-onu_X/Y/Z:A
```

Melihat Redaman ONT
````bash
show pon power attenuation gpon-onu_X/Y/Z:A
````

Mencari Interface berdasarkan SN Modem
````bash
show gpon onu by sn ZTEXXXXXXXXX
````

