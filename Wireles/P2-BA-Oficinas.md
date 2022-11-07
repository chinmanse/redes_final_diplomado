## Configuracion de la interfaz g0/1 a troncal sobre la vlan 120
```
configure terminal
interface gigabitEthernet 0/1
switchport mode trunk 
switchport trunk native vlan 120
exit
interface fastEthernet 0/1
switchport trunk native vlan 120
```
## Para habilitar la vlan 120, en la interfaz correcta
```
switchport trunk allowed vlan 10,20,30,40,50,60,70,80,90,110,120
```
## Creacion del interfaz de la vlan nativa para permitir el trafico hacia el WLC
```
interface vlan 120

```

# PARA EL MLS
```
configure terminal
interface vlan 120
ip address 172.16.120.131 255.255.255.240
exit
ip dhcp excluded-address 172.16.120.129 172.16.120.139
ip dhcp pool NATIVA-120
network 172.16.120.144 255.255.255.240
default-router 172.16.120.129
```
