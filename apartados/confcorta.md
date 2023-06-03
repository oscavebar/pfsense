# Configuración del cortafuegos

## Reglas

Para configurar las reglas de nuestro cortafuegos iremos al apartado de firewall y le damos donde dice 'rules'.

Aquí podremos configurar todas las reglas que queramos para nuestras interfaces.

- Dependiendo de la interfaz que veamos, podemos comprobar que tenemos reglas por defecto que ya están creadas.
- Tenemos dos botones para añadir regla nuevas, con la flecha arriba significa que crearemos las reglas encima de las otras que se han creado, tieniendo esta prioridad sobre las de abajo en caso de se contradictorias. Igualmente se puede modificar la posición con posterioridad arrastándo la regla creada.
 
 IMAGEN
 
 Cuando empezamos a crear una regla podemos ver las siguientes opciones:
 
 - Action: Especificaremos la función de la regla si es permisiva, si bloquea o hace reject. Esta última también bloquea, pero notificará al usuario la causa del bloqueo.
 - Disabled: Sirve para desactivar la regla en caso de que no la queremos usar temporalmente.
 - Interface: Por defecto saldrá la interfaz que estábamos configurando, pero en caso de haberte equivocado, puedes rectificar aquí.
 - Addres Family: Aquí elegimos si queremos editar esta regla para las IPv4 o IPv6.
 - Protocol: Esta opcíon es importante, aquí decidimos si queremos que esta regla aplique en un protocolo de red específico o todos los protocolos.
 
 IMAGEN
 
 IMAGEN
 
 - Source: Indicamos desde donde se aplica la regla, donde podemos elegir entre varias opciones. Podemos elegir una red entera, una zona, alguna ip en concreto, etc...
  IMAGEN
 -Destination: Ahora toca decidir a donde se aplica la regla, tenemos varias opciones al igual que en source y específiacmos en que puerto va a actuar esta regla.

 IMAGEN
 
 - Opciones extra: Aquí podemos hacer una descripción de la regla que siempre recomiendo hacer para poder localizar la regla fácilmente después. Además contamos con la opción de entrar a las configuraciones avanzadas de las que adelante especifíco las más usadas.

 IMAGEN
 
 Opciones avanzadas:
 
 - Source OS: Esta solo aplica para las reglas TCP, donede podemos especificar además cuál ha de ser el SO del equipo
 - Límites: En la opciónes siguientes podremos ver que se puede establecer un máximo de conexiones por host, por ejemplo.
 IMAGEN
 - Schedule: En esta podemos usar una schedule creada con anterioridad, que lo enseñaré en el siguiente apartado.
 - Gateway: Aquí también puedes especificar la puerta de enlace configurada del cliente.

IMAGEN

## Interface Groups
Aquí podemos configurar un grupo de interfaces para que a la hora de crear una regla puedas ahorrarte crear reglas repetitivas. En el siguiente apartado hay un ejemplo de como se usa.

IMAGEN

## Aliases
Este es otro apartado para ahorrar tiempo en la creación de reglas si creamos un alias podremos actuar sobre un grupo de IP, puertos y/o URLs.

IMAGEN
