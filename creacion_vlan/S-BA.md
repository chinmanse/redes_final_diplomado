# Switch S-BA
## Modo truncol del puerto G0/1
```
enable
configure terminal
interface g0/1
switchport mode trunk
end
show interfaces trunk
```
## Restringir VLAN
```
enable
configure terminal
interface g0/1
switchport trunk allowed vlan 10,20,30,40,50,60,70,80,90,110
end
```