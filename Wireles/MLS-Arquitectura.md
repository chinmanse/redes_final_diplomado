## Configuracion de la interfaz g0/1 a troncal sobre la vlan 120
```
configure terminal
interface gigabitEthernet 1/0/1
switchport trunk native vlan 120
exit

interface gigabitEthernet 1/0/2
switchport trunk native vlan 120
exit

interface gigabitEthernet 1/0/3
switchport trunk native vlan 120
exit

interface gigabitEthernet 1/0/4
switchport trunk native vlan 120
exit
```