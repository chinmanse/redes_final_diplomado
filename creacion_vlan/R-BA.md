### Switch S-BA
# Configuracion de Sub Interfaces
```
enable
configure terminal
interface g0/0/0.110
description VLAN ADMIN
encapsulation dot1Q 110
ip address 192.168.110.1 255.255.255.0
exit
end

enable
configure terminal
interface g0/0/0.10
description VLAN LAB-A
encapsulation dot1Q 10
ip address 192.168.10.1 255.255.255.0
exit
end

enable
configure terminal
interface g0/0/0.20
description VLAN LAB-B
encapsulation dot1Q 20
ip address 192.168.20.1 255.255.255.0
exit
end

enable
configure terminal
interface g0/0/0.30
description VLAN LAB-C
encapsulation dot1Q 30
ip address 192.168.30.1 255.255.255.0
exit
end

enable
configure terminal
interface g0/0/0.40
description VLAN CRTP
encapsulation dot1Q 40
ip address 192.168.40.1 255.255.255.0
exit
end


enable
configure terminal
interface g0/0/0.50
description VLAN DECANATO
encapsulation dot1Q 50
ip address 192.168.50.1 255.255.255.0
exit
end


enable
configure terminal
interface g0/0/0.60
description VLAN INST-DOC
encapsulation dot1Q 60
ip address 192.168.60.1 255.255.255.0
exit
end


enable
configure terminal
interface g0/0/0.70
description VLAN ADMINISTRACION
encapsulation dot1Q 70
ip address 192.168.70.1 255.255.255.0
exit
end


enable
configure terminal
interface g0/0/0.80
description VLAN INVITADOS
encapsulation dot1Q 80
ip address 192.168.80.1 255.255.255.0
exit
end


enable
configure terminal
interface g0/0/0.90
description VLAN AULAS
encapsulation dot1Q 90
ip address 192.168.90.1 255.255.255.0
exit
end


enable
configure terminal
interface g0/0/0.100
description VLAN OFICINAS
encapsulation dot1Q 100
ip address 192.168.100.1 255.255.255.0
exit
end
```

### Encender el puerto G0/0/0
```
enable
configure terminal
interface g0/0/0
no shutdown
end
```
### Ver las configuraciones
```
show ip interface brief
```