## Configuraciones para el DHCP

```
configure terminal
interface vlan 10
ip address 172.16.10.131 255.255.255.192
exit
ip dhcp excluded-address 172.16.10.129 172.16.10.131
ip dhcp excluded-address 172.16.10.190
ip dhcp pool LAB-A-10
network 172.16.10.128 255.255.255.192
default-router 172.16.10.190

configure terminal
interface vlan 20
ip address 172.16.20.195 255.255.255.224
exit
ip dhcp excluded-address 172.16.20.193 172.16.20.195
ip dhcp excluded-address 172.16.20.222
ip dhcp pool LAB-B-20
network 172.16.20.192 255.255.255.224
default-router 172.16.20.222

configure terminal
interface vlan 30
ip address 172.16.30.3 255.255.255.224
exit
ip dhcp excluded-address 172.16.30.1 172.16.30.3
ip dhcp excluded-address 172.16.30.30
ip dhcp pool LAB-C-30
network 172.16.30.0 255.255.255.224
default-router 172.16.30.30


configure terminal
interface vlan 40
ip address 172.16.40.147 255.255.255.240
exit
ip dhcp excluded-address 172.16.40.145 172.16.40.147
ip dhcp excluded-address 172.16.40.158
ip dhcp pool CRTP-40
network 172.16.40.144 255.255.255.240
default-router 172.16.40.158


configure terminal
interface vlan 50
ip address 172.16.50.99 255.255.255.224
exit
ip dhcp excluded-address 172.16.50.97 172.16.50.99
ip dhcp excluded-address 172.16.50.126
ip dhcp pool DECANATO-50
network 172.16.50.96 255.255.255.224
default-router 172.16.50.126

configure terminal
interface vlan 60
ip address 172.16.60.35 255.255.255.224
exit
ip dhcp excluded-address 172.16.60.33 172.16.60.35
ip dhcp excluded-address 172.16.60.62
ip dhcp pool INST-DOC-60
network 172.16.60.32 255.255.255.224
default-router 172.16.60.62


configure terminal
interface vlan 70
ip address 172.16.70.67 255.255.255.224
exit
ip dhcp excluded-address 172.16.70.65 172.16.70.67
ip dhcp excluded-address 172.16.70.94
ip dhcp pool ADMINISTRACION-70
network 172.16.70.64 255.255.255.224
default-router 172.16.70.94


configure terminal
interface vlan 80
ip address 172.16.80.3 255.255.255.128
exit
ip dhcp excluded-address 172.16.80.1 172.16.80.3
ip dhcp excluded-address 172.16.80.126
ip dhcp pool INVITADOS-80
network 172.16.80.0 255.255.255.128
default-router 172.16.80.126

configure terminal
interface vlan 90
ip address 172.16.90.227 255.255.255.224
exit
ip dhcp excluded-address 172.16.90.225 172.16.90.227
ip dhcp excluded-address 172.16.90.254
ip dhcp pool AULAS-90
network 172.16.90.224 255.255.255.224
default-router 172.16.90.254

configure terminal
interface vlan 100
ip address 172.16.100.131 255.255.255.240
exit
ip dhcp excluded-address 172.16.100.129 172.16.100.131
ip dhcp excluded-address 172.16.100.142
ip dhcp pool OFICINAS-100
network 172.16.100.128 255.255.255.240
default-router 172.16.100.142

```