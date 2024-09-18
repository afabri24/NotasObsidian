enable

configure terminal

hostname R1

banner motd # texto#
end
write
enable password ulagos
secret password ulagos2024




1 - Agregar configuraciones básicas:
Hostname R1
        Hostname SW1
        Banner motd "Acceso restringido por sunombre"
clave usuario: ulagos
clave admin: ulagos.2024

2 - Configuración de interfaces
    IP Router: 192.168.0.254 máscara de de red 255.255.255.0
    IP Switch: 192.168.0.99/24

3 - Agregar SSH versión 2 a cada dispositivo(Router y Switch)
nombre: admin clave: admin.2024
(Para ambos dispositivos y accesible desde todos los PCs)
 
4 - Agregar Servicio DHCP para Router ISP y Router de Red interna
    Nombre de Pool red Externa ISP: "redISP". Excluir desde la IP        200.200.200.1-9
  - Agregar DNS server 200.200.200.10

    Nombre de Pool red Interna: "redInterna" y excluir las IPs del 192.168.0.1 al 192.168.0.99 y del 192.168.0.151 al 192.168.0.254

5 - Configurar NAT
    IP Exterior  e IP Interior
 (Explicación al final de la clase)


E


