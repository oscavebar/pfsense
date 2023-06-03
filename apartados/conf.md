# Configuración básica del sistema

Tenemos que tener las siguientes interfaces de red en nuestra máquina.

![conf0](/imagenes/conf0.png)
![conf0'5](/imagenes/conf0'5.png)
![conf0'75](/imagenes/conf0'75.png)

- Arrancamos la máquina no dará varias opciones, seleccionamos la primera para asignas la interfaces a cada red.
- Marcaremos que no queremos configurar las VLAN ahora.
- Ahora seleccionamos que interfaz pertenece a WAN, a LAN y la opcional si la queremos.
- Finalmente procedemos con el proceso.

![conf1](/imagenes/conf1.png)
![conf2](/imagenes/conf2.png)
![conf4](/imagenes/conf4.png)
![conf5](/imagenes/conf5.png)

Ahora vamos a la segunda opción para configurar la IP de nustra interfaz LAN dondé le daré la IP: 172.16.0.1/24 (Crearemos el acceso HTTP a el configurador WEB y no queremos que reciba la ip por DHCP)

![conf6](/imagenes/conf6.png)
![conf7](/imagenes/conf7.png)
![conf8](/imagenes/conf8.png)
![conf9](/imagenes/conf9.png)

Finalmente nos da una dirección para que cualquier equipo de la LAN pueda entrar al configurador WEB.
