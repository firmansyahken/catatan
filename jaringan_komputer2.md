# Jaringan Komputer 2

## Konfigurasi VLAN

### Konfigurasi VLAN pada Switch
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

Langkah ini mengonfigurasi port-range dari f0/11 hingga f0/17 agar menjadi port access yang terhubung ke VLAN 10 yang telah dibuat sebelumnya.

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

Langkah ini mengonfigurasi port gigabit Ethernet 0/1 sebagai trunk port, yang memungkinkan lalu lintas VLAN melalui port tersebut. VLAN 88 diatur sebagai VLAN asli (native VLAN) untuk port trunk ini.

- Mendisable semua port yang tak digunakan
```sh
S1(config)#interface range f0/1-5,g0/2
S1(config-if-range)#shutdown
```

Langkah ini menonaktifkan port-range f0/1 hingga f0/5 dan port g0/2, yang tidak akan digunakan untuk koneksi jaringan.


Catatan Sementara:

switchport mode trunk = digunakan untuk network device

channel-group 1 mode active/passive (LACP, active menerima | passive tidak)
channel-group 3 mode desirable/auto (PAGP)
