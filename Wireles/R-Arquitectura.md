## Configuracion de la subinterfaz para la vlan nativa
```
configure terminal
interface GigabitEthernet0/0/0.120
description VLAN NATIVA
encapsulation dot1Q 120 native
ip address 172.16.120.129 255.255.255.240
```