## Configuracion de la interfaz g0/1 a troncal sobre la vlan 120
```
configure terminal
interface fastEthernet 0/9
switchport trunk native vlan 120
exit

interface fastEthernet 0/16
switchport trunk native vlan 120
exit

interface fastEthernet 0/17
switchport trunk native vlan 120
exit

interface gigabitEthernet 0/1
switchport trunk native vlan 120
exit
```