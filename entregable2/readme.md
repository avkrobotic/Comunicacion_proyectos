Práctica día 10/03/2022

Iniciar sesión en Ubidots

Instalar en node-red paquete de ubidots

Poner token de ubidots en nodo "ubidots_out"

conectarlo para que envíe la info de openweather map          [captura node-red]

se muestra un máximo de 10 variables en el device creado "asdf" (máximo 2 devices) de todas las variables. Las 10 primeras en orden alfabético [captura varuables_ubidots]

add widget (metric) ... add variable (pressure del device "asdf") y se crea el primer widget.     [captura widget]

extra:

borramos las 3 primeras variables para que haya espacio

metemos 2 nuevas y presión especifixcando con function [captura node-red_function]

Se observan las nuevas variables y la otra actualizada [captura_variables_extra]

mostramos temperatura de Alicante en otro widget. FIN


Práctica día 17/03/2022

DOCUMENTACIÓN 

Esta sesión se ha dedicado íntegramente a la inicialización y conexión vía red local y vía WiFi del controlador de una instalación.

En primer lugar, el ordenador se ha conectado a la red local (del router o de shelly) (sin conexión WiFi) de la mencionada instalación, con la cual poder acceder a la configuración de Shelly por medio de su interfaz. 

Desde esta interfaz (192.168.33.1) se puede interactuar con aquellos dispositivos de la instalación conectados a ellos (ejecutar acciones como encender/apagar un switch, recibir información, etc.). En esta ocasión se ha indicado al Shelly que se conecte a la red WiFi "Cudy-081-c" indicando los siguientes valores:

{shelly_wifi_cudy}

La especificación de la IP se debe encontrar dentro de un rango de IPs disponibles (192.168.10.[0-255]). El uso de otra conexión fuera de este rango supondría encontrarse fuera de la red local.

Dado que shelly puede grabar esta configuración en su memoria, se puede salir de la conexión de Shelly y esta seguirá conectada a "Cudy-081-c".

Por último, se conecta nuevamente el ordenador a esta misma red del router, la cual sí ofrece al ordenador una conexión WiFi y se accede desde un navegador a la IP especificada. De esta manera, se ha logrado conectarse a la interfaz de Shelly vía WiFi, donde podemos acceder de igual manera al conjunto de la instalación. En este caso, se ha encendido y apagado el switch disponible.
