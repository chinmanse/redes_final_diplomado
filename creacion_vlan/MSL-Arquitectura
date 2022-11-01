# Configuracion realizadas en el switch Muilti Capa MLS-Arquitectura
## Creacion de VLANs
```
enable
configure terminal
vlan 10
name LAB-A
vlan 20
name LAB-B
vlan 30
name LAB-C
vlan 40
name CRTP
vlan 50
name DECANATO
vlan 60
name INST-DOC
vlan 70
name ADMINISTRACION
vlan 80
name INVITADOS
vlan 90
name AULAS
vlan 100
name OFICINAS
vlan 110
name ADMIN
vlan 120
name NATIVA
end
show vlan brief

```
## Activar Enrutamiento IP
```
enable
configure terminal
ip routing
end

```
## Creacion de Troncales Trunk
```
enable
configure terminal
interface g1/0/1
switchport trunk encapsulation dot1q
switchport mode trunk
exit
end

enable
configure terminal
interface g1/0/2
switchport trunk encapsulation dot1q
switchport mode trunk
exit
end

enable
configure terminal
interface g1/0/3
switchport trunk encapsulation dot1q
switchport mode trunk
exit
end

enable
configure terminal
interface g1/0/4
switchport trunk encapsulation dot1q
switchport mode trunk
exit
end
```
## Asigancion de IP para enlace con la vlan de admin

```
enable
configure terminal
interface vlan 110
ip address 192.168.110.23 255.255.255.0
no shutdown
exit
ip default-gateway 192.168.110.1
end
```