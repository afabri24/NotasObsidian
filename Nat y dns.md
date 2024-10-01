
para el dns deslpues del default router:
dns-server 200.200.200.10



en
conf t
access-list 1 permit 192.168.0.0 0.0.0.255
ip nat inside source list 1 interface GigabitEthernet0/0 overload

(La X la tienes que remplazar por lo que te pida)
1. configuracion basica(Router y switch)
enable 
configure terminal 
hostname (el nombre que se le va dar)
enable secret (la contrasena admin)
line con 0
 password (la contrasena usuario )
 login 
 exit 
banner motd # Mensaje de banner# 

2. configuracion de interfaz(Router y switch)

Para el Router:
interface (GigabitEthernet 0/x)
ip address 192.168.X.X 255.255.255.0
shutdown
exit

Para el Switch:
interface vlan 1
ip address 192.168.X.X 255.255.255.0
shutdown
exit


3. Configuracion SSH(Router y Switch)
 ip domain name (nombre del nominio)
crypto key generate rsa 
1024 
username (usuario) secret (contrasena)
line vty 0 15
transport input ssh
login local
exit
ip ssh version 2

4. Servicio DHCP (routers)
ip dhcp excluded-address x.x.x.x x.x.x.x
ip dhcp pool (nombre del pool) 
network 192.168.X.0 x.x.x.x
default-router x.x.x.x (Este es un comentario es para recordarte que x.x.x.x es la IP del router) 
dns-server x.x.x.x
exit

5. Configurar NAT (routers)
interface interface (GigabitEthernet 0/x)
ip nat inside
exit

interface interfaz-dos
ip nat outside
exit 

access-list 1 permit 192.168.X.0 0.0.0.255
ip nat inside source list 1 interface GigabitEthernet0/x (este es un comentario: o la interfaz que este conectado a la red interna) overload

6. Guardar configuracion
exit
write memory 
exit 

