Monitoreo de Temperatura, Humedad y Movimiento con ESP32

Descripción del proyecto


El proyecto consiste en el desarrollo de un sistema IoT basado en ESP32 capaz de monitorear variables ambientales y detectar movimiento mediante sensores electrónicos.

El sistema permite medir temperatura, humedad relativa y estado de movimiento utilizando sensores conectados al microcontrolador. Además, incorpora monitoreo remoto mediante Telegram y visualización en tiempo real a través de un servidor web.

También se implementó un sistema de alertas visuales, sonoras y remotas para notificar condiciones anormales del entorno.


Componentes utilizados

ESP32
Sensor DHT11/DHT22
Sensor MPU6050
Buzzer
Pulsador
Protoboard
Jumpers
Red Wi-Fi
Celular con Telegram


Funcionamiento del sistema

El ESP32 se conecta automáticamente a la red Wi-Fi.
Se inicializan los sensores DHT y MPU6050.
El sistema comienza el monitoreo continuo.
Las variables son mostradas en el servidor web.
El usuario puede consultar datos mediante Telegram.
Si ocurre una condición anormal, el sistema activa alertas.


Variables monitoreadas

Temperatura
Humedad relativa
Movimiento
Estado de alarmas


Sistema de alertas
El sistema implementa alertas multimodales:

Alertas visuales
Mostradas en el servidor web.

Alertas sonoras
Generadas mediante buzzer.

Alertas remotas
Enviadas automáticamente mediante Telegram.


Comunicación

Comunicación Wi-Fi
El ESP32 utiliza conexión Wi-Fi para habilitar el servidor web y la comunicación remota.

Comunicación mediante Telegram
El bot de Telegram permite:
Consultar temperatura
Consultar humedad
Consultar movimiento
Recibir notificaciones automáticas
Servidor web

La interfaz web muestra:
Temperatura
Humedad
Estado de movimiento
Estado de alarmas


Interfaz de usuario
La interfaz fue diseñada para facilitar el monitoreo en tiempo real.
El usuario puede acceder al sistema mediante:
Navegador web
Aplicación Telegram


Estructura del código
El programa está dividido en módulos encargados de:

Configuración Wi-Fi
Lectura de sensores
Manejo de alertas
Comunicación Telegram
Servidor web
Control del buzzer
Procesamiento de movimiento
