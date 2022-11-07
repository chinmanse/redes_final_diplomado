## Configuracion de la interfaz g0/1 a troncal sobre la vlan 120
```
configure terminal
interface fastEthernet 0/1
switchport trunk native vlan 120
exit

interface gigabitEthernet  0/1
switchport mode trunk 
switchport trunk native vlan 120
```

## Asignacion de IP a la interfaz de la VLAN
```
interface vlan 120
ip address 172.16.120.134 255.255.255.240
```