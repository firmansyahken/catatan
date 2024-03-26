# Jaringan Komputer 2

## Konfigurasi VLan 

### Konfigurasi Switch VLan
- Konfigurasi nama vlan berdasarkan id vlan
```sh
S1(config)#vlan 10
S1(config-vlan)#name Faculty/Staff
```
- Konfigurasi interface vlan
```sh
S1(config-vlan)#interface range f0/11 - 17
S1(config-if-range)#switchport mode access
```
- Contoh swit mode access
```sh
S1(config-if-range)#switchport access vlan 10
```
- Contoh swit mode trunk
```sh
S1(config)#interface g0/1
S1(config-if)#switchport mode trunk
S1(config-if)#switchport trunk native vlan 88
```
- Mendisable semua port yang tak digunakan
```sh
S1(config)#interface range f0/1-5,g0/2
S1(config-if-range)#shutdown
```
