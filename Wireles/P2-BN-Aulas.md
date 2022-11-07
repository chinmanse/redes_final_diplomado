## Configuracion de la interfaz g0/1 a troncal sobre la vlan 120
```
configure terminal
interface fastEthernet 0/1
switchport trunk native vlan 120
exit

```
## Configuracion de enlace troncal para el AP (Acces Point)
```
configure terminal 
interface gigabitEthernet 0/1
switchport mode trunk 
switchport trunk native vlan 120
exit

```