# Reglas aplicadas

Antes de configurar las reglas como tal, haré las siguientes configuraciones.

- DHCP leases: Voy a reservar la ip 10.0.0.71 a mi sevidor web y la ip 172.16.0.60 al cliente desde el que estoy usando el administrador gráfico de pfSense.
 
 ![aplicado1](/imagenes/aplicado1.png)
 
 - Redes Internas: Ahora creo un grupo de interfaces que llamaré redes internas para especificar que me refiero tanto a LAN como DMZ.
 
 ![aplicado2](/imagenes/aplicado2.png)
 
 - Tráfico Web: Aquí creo un alias para referirme a los puertos 80 y 443 que sirven para HTTP y HTTPS.
 
 ![aplicado3](/imagenes/aplicado3.png)
 
 Ahora sí, creamos las reglas que voy a utilizar:
 
 - Redes Internas: Aqúi creamos una sola regla que permita las transferencia de paquetes ICMP dentro de las redes internas para así permitir el ping entre LAN y DMZ.
 
 ![aplicado4](/imagenes/aplicado4.png)
 
 - WAN: Creamos una regla que permit HTTP(s) a la red WAN con los paquetes TCP solo desde el cliente con la ip 10.0.0.71 y usando los puestos de tráfico web creados anteriormente. Creamos otra regla que bloquea todo tráfico desde la WAN.
 
 ![aplicado5](/imagenes/aplicado5.png)
 
 - LAN: Permitimos la conexión SSH desde el cliente con ip 172.16.0.60 solo los días de trabajo que se han configurado. Tenemos creada otra dos reglas más que se ven en la imagén a continuación, se puede ver su función en el apartado de descripción.
 
 ![aplicado6](/imagenes/aplicado6.png)
 
 -DMZ: Aquí solo creo dos reglas que permiten la conexión de los equipos de DMZ a internet y bloquea el tráfico proveniente de DMZ para que no vaya a LAN.
 
 ![aplicado7](/imagenes/aplicado7.png)
