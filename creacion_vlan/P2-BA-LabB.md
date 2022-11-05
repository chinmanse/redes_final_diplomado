# Configuracion realizadas en el switch P2-BA-LabB
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
interface range fa0/3 - 22
switchport mode access
switchport access vlan 20
no shutdown
exit
end
show vlan brief
```
## Creacion del enlace troncal POR SI ACASO

```
enable
configure terminal
interface fa0/1
switchport mode trunk
no shutdown
exit
end
```
## Creacion de EtherChannel

```
enable
configure terminal
interface range fa0/1-2
channel-group 2 mode active
exit
interface port-channel 2
switchport mode trunk
switchport trunk allowed vlan 20
exit
end
show etherchannel summary
```
### Switch S-BA
```
enable 
configure terminal
interface range fa0/12-13
shutdown
channel-group 2 mode active
no shutdown
end
show etherchannel summary
```
## Asigancion de IP para enlace con la vlan de admin

```
enable
configure terminal
interface vlan 110
ip address 192.168.110.17 255.255.255.0
no shutdown
exit
ip default-gateway 192.168.110.1
end
```