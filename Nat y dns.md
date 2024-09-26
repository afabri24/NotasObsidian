
para el dns deslpues del default router:
dns-server 200.200.200.10



en
conf t
access-list 1 permit 192.168.0.0 0.0.0.255
ip nat inside source list 1 interface GigabitEthernet0/0 overload


