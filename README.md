# Introducción

Mosquitto es un servidor de mensajería de código abierto que implementa el protocolo MQTT (Message Queuing Telemetry Transport). MQTT es un protocolo de comunicación de mensajería leve diseñado para la conectividad en dispositivos IoT y redes de área amplia.

MQTT se utiliza para enviar y recibir pequeños mensajes entre dispositivos conectados, permitiendo una comunicación eficiente y confiable en redes con limitaciones de ancho de banda y energía. Es un protocolo public-subscriber, lo que significa que los dispositivos pueden "publicar" mensajes en un "tema" específico, y otros dispositivos pueden "suscribirse" a ese tema para recibir los mensajes publicados.

Mosquitto es uno de los servidores de mensajería MQTT más populares y ampliamente utilizado. Es compatible con diferentes sistemas operativos, incluyendo Windows, MacOS y Linux, y es fácil de configurar y utilizar. Puedes usar Mosquitto para conectar dispositivos IoT a una red y comunicarse entre ellos de manera eficiente y segura.

# Material Necesario

- [VirtualBox](https://github.com/RaulToribio/01-Instalar-VirtualBox)
- [Ubuntu 22.04.1 LTS](https://github.com/RaulToribio/02-Descargar-Ubuntu)
- [Crear Máquina Virtual](https://github.com/RaulToribio/03-Crear-Maquina-Virtual)
- [Configurar Máquina Virtual](https://github.com/RaulToribio/04-Configurar-Maquina-Virtual)
- [Instalar Ubuntu](https://github.com/RaulToribio/05-Instalar-Ubuntu)
- [Instalar Guest Additions](https://github.com/RaulToribio/06-Instalar-Guest-Additions)
- [Comandos Linux](https://github.com/RaulToribio/07-Comandos-Linux)

# Material de Referencia

- [Instalación de Mosquitto en Ubuntu 20.04](https://edu.codigoiot.com/course/view.php?id=818)

# Instrucciones

![https://raw.githubusercontent.com/RaulToribio/15-Instalar-Mosquitto/main/Im%C3%A1genes/Instalar%20Mosquitto%20(1).png](https://raw.githubusercontent.com/RaulToribio/15-Instalar-Mosquitto/main/Im%C3%A1genes/Instalar%20Mosquitto%20(1).png)

Acceder a la sección de Ubuntu en la página de descargas de [Mosquitto](https://mosquitto.org/download/).

![https://raw.githubusercontent.com/RaulToribio/15-Instalar-Mosquitto/main/Im%C3%A1genes/Instalar%20Mosquitto%20(2).png](https://raw.githubusercontent.com/RaulToribio/15-Instalar-Mosquitto/main/Im%C3%A1genes/Instalar%20Mosquitto%20(2).png)

Usar la línea de comando `sudo apt-add-repository ppa:mosquitto-dev/mosquitto-ppa` para agregar el repositorio de Mosquitto.

![https://raw.githubusercontent.com/RaulToribio/15-Instalar-Mosquitto/main/Im%C3%A1genes/Instalar%20Mosquitto%20(3).png](https://raw.githubusercontent.com/RaulToribio/15-Instalar-Mosquitto/main/Im%C3%A1genes/Instalar%20Mosquitto%20(3).png)

Ingresar contraseña.

![https://raw.githubusercontent.com/RaulToribio/15-Instalar-Mosquitto/main/Im%C3%A1genes/Instalar%20Mosquitto%20(4).png](https://raw.githubusercontent.com/RaulToribio/15-Instalar-Mosquitto/main/Im%C3%A1genes/Instalar%20Mosquitto%20(4).png)

Presionar “Enter”.

![https://raw.githubusercontent.com/RaulToribio/15-Instalar-Mosquitto/main/Im%C3%A1genes/Instalar%20Mosquitto%20(5).png](https://raw.githubusercontent.com/RaulToribio/15-Instalar-Mosquitto/main/Im%C3%A1genes/Instalar%20Mosquitto%20(5).png)

Se habrá agregado el repositorio de Mosquito a la lista de paquetes.

![https://raw.githubusercontent.com/RaulToribio/15-Instalar-Mosquitto/main/Im%C3%A1genes/Instalar%20Mosquitto%20(6).png](https://raw.githubusercontent.com/RaulToribio/15-Instalar-Mosquitto/main/Im%C3%A1genes/Instalar%20Mosquitto%20(6).png)

Actualizar el sistema.

![https://raw.githubusercontent.com/RaulToribio/15-Instalar-Mosquitto/main/Im%C3%A1genes/Instalar%20Mosquitto%20(7).png](https://raw.githubusercontent.com/RaulToribio/15-Instalar-Mosquitto/main/Im%C3%A1genes/Instalar%20Mosquitto%20(7).png)

Se habrá actualizado el sistema.

![https://raw.githubusercontent.com/RaulToribio/15-Instalar-Mosquitto/main/Im%C3%A1genes/Instalar%20Mosquitto%20(8).png](https://raw.githubusercontent.com/RaulToribio/15-Instalar-Mosquitto/main/Im%C3%A1genes/Instalar%20Mosquitto%20(8).png)

Usar la línea de comando `sudo apt-get install mosquitto` para instalar Mosquitto.

![https://raw.githubusercontent.com/RaulToribio/15-Instalar-Mosquitto/main/Im%C3%A1genes/Instalar%20Mosquitto%20(9).png](https://raw.githubusercontent.com/RaulToribio/15-Instalar-Mosquitto/main/Im%C3%A1genes/Instalar%20Mosquitto%20(9).png)

Confirmar la operación escribiendo “*Y*”.

![https://raw.githubusercontent.com/RaulToribio/15-Instalar-Mosquitto/main/Im%C3%A1genes/Instalar%20Mosquitto%20(10).png](https://raw.githubusercontent.com/RaulToribio/15-Instalar-Mosquitto/main/Im%C3%A1genes/Instalar%20Mosquitto%20(10).png)

Se habrá instalado Mosquitto.

![https://raw.githubusercontent.com/RaulToribio/15-Instalar-Mosquitto/main/Im%C3%A1genes/Instalar%20Mosquitto%20(11).png](https://raw.githubusercontent.com/RaulToribio/15-Instalar-Mosquitto/main/Im%C3%A1genes/Instalar%20Mosquitto%20(11).png)

Utilizar la línea de comando `sudo apt indtall net-tools` para instalar las net-tools.

Los net-tools son un conjunto de herramientas de red para Linux que incluye una serie de comandos para configurar y monitorear interfaces de red, configuraciones de red y protocolos de red.

El conjunto de herramientas incluye comandos como:

- ifconfig: Es una herramienta que se utiliza para configurar y verificar la configuración de las interfaces de red, como la dirección IP, la máscara de subred y la dirección MAC.
- route: Comando que se utiliza para verificar y configurar la tabla de enrutamiento del sistema.
- netstat: Es una herramienta que se utiliza para verificar el estado de las conexiones de red, las estadísticas de protocolo y las tablas de enrutamiento.
- arp: Es una herramienta que se utiliza para verificar y configurar la tabla de asociación de direcciones de protocolo de Internet (IP) y direcciones de hardware de interface de red.

Los net-tools son un paquete que ha sido ampliamente utilizado en versiones anteriores de Linux, pero actualmente se recomienda usar iproute2, un conjunto de herramientas que incluye las mismas funciones pero con un enfoque en el diseño de sistemas modernos, con una interfaz de línea de comandos coherente y una interfaz de programación de aplicaciones (API) consistente.

![https://raw.githubusercontent.com/RaulToribio/15-Instalar-Mosquitto/main/Im%C3%A1genes/Instalar%20Mosquitto%20(12).png](https://raw.githubusercontent.com/RaulToribio/15-Instalar-Mosquitto/main/Im%C3%A1genes/Instalar%20Mosquitto%20(12).png)

Se habrán instalado los net-tools.

![https://raw.githubusercontent.com/RaulToribio/15-Instalar-Mosquitto/main/Im%C3%A1genes/Instalar%20Mosquitto%20(13).png](https://raw.githubusercontent.com/RaulToribio/15-Instalar-Mosquitto/main/Im%C3%A1genes/Instalar%20Mosquitto%20(13).png)

Utilizar la línea de comando `net-statan` para verificar el estado de las conexiones de red, las estadísticas de protocolo y las tablas de enrutamiento.

![https://raw.githubusercontent.com/RaulToribio/15-Instalar-Mosquitto/main/Im%C3%A1genes/Instalar%20Mosquitto%20(14).png](https://raw.githubusercontent.com/RaulToribio/15-Instalar-Mosquitto/main/Im%C3%A1genes/Instalar%20Mosquitto%20(14).png)

Mosquitto estará habilitado en la dirección 127.0.0.1 con puerto 1883 y configuración Foreing Address como 0.0.0.0* que permite que todos los dispositivos envíen información.

# Créditos

> [José Raúl Toribio Gabriel](https://github.com/RaulToribio)
> 

> [Codigo IoT](https://github.com/codigo-iot)
>
