# Configuracion realizadas en el switch P2-BN-Aulas
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
## Agrupacion de Puertos a vlans

```
enable
configure terminal
interface range fa0/2 - 13
switchport mode access
switchport access vlan 90
no shutdown
exit
end
```
## Creacion del enlace troncal

```
enable
configure terminal
interface fa0/1
switchport mode trunk
no shutdown
exit
end
```
### Switch S-BN
```
enable
configure terminal
interface fa0/10
switchport mode trunk
no shutdown
exit
end
```
## Asigancion de IP para enlace con la vlan de admin

```
enable
configure terminal
interface vlan 110
ip address 192.168.110.21 255.255.255.0
no shutdown
exit
ip default-gateway 192.168.110.1
end
```