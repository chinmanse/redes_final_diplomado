## Configuracion de router virtual

```
configure terminal
interface g 0/0/0.10
description VLAN LAB-A
encapsulation dot1Q 10
ip address 172.16.10.129 255.255.255.192
standby 2 ip 172.16.10.190
standby 2 priority 150
standby 2 preempt

configure terminal
interface g 0/0/0.20
description VLAN LAB-B
encapsulation dot1Q 20
ip address 172.16.20.193 255.255.255.224
standby 2 ip 172.16.20.222
standby 2 priority 150
standby 2 preempt

configure terminal
interface g 0/0/0.30
description VLAN LAB-C
encapsulation dot1Q 30
ip address 172.16.30.1 255.255.255.224
standby 2 ip 172.16.30.30
standby 2 priority 150
standby 2 preempt

configure terminal
interface g 0/0/0.40
description VLAN CRTP
encapsulation dot1Q 40
ip address 172.16.40.145 255.255.255.240
standby 2 ip 172.16.40.158
standby 2 priority 150
standby 2 preempt

configure terminal
interface g 0/0/0.50
description VLAN DECANATO
encapsulation dot1Q 50
ip address 172.16.50.97 255.255.255.224
standby 2 ip 172.16.50.126
standby 2 priority 150
standby 2 preempt

configure terminal
interface g 0/0/0.60
description VLAN INST-DOC
encapsulation dot1Q 60
ip address 172.16.60.33 255.255.255.224
standby 2 ip 172.16.60.62
standby 2 priority 150
standby 2 preempt

configure terminal
interface g 0/0/0.70
description VLAN ADMINISTRACION
encapsulation dot1Q 70
ip address 172.16.70.65 255.255.255.224
standby 2 ip 172.16.70.94
standby 2 priority 150
standby 2 preempt

configure terminal
interface g 0/0/0.80
description VLAN INVITADOS
encapsulation dot1Q 80
ip address 172.16.80.1 255.255.255.128
standby 2 ip 172.16.80.126
standby 2 priority 150
standby 2 preempt

configure terminal
interface g 0/0/0.90
description VLAN AULAS
encapsulation dot1Q 90
ip address 172.16.90.225 255.255.255.224
standby 2 ip 172.16.90.254
standby 2 priority 150
standby 2 preempt

configure terminal
interface g 0/0/0.100
description VLAN OFICINAS
encapsulation dot1Q 100
ip address 172.16.100.129 255.255.255.240
standby 2 ip 172.16.100.142
standby 2 priority 150
standby 2 preempt


```

