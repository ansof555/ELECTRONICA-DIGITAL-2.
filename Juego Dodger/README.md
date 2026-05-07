DODGER - Juego en ESP32 con OLED SSD1306

Descripción

El proyecto consiste en el diseño e implementación de un videojuego tipo dodger utilizando un microcontrolador ESP32 y una pantalla OLED SSD1306.

El sistema permite controlar un personaje mediante pulsadores para esquivar obstáculos generados dinámicamente. Además, cuenta con diferentes modos de juego, efectos de sonido y control de dificultad progresiva.

⸻

Componentes del Sistema

Entradas

3 Pulsadores

* Movimiento hacia arriba
* Movimiento hacia abajo
* Inicio / pausa del juego

⸻

Procesamiento

Microcontrolador ESP32

Funciones implementadas:

* Comunicación I2C
* Generación PWM
* Temporización en tiempo real
* Máquina de estados
* Debounce por software
* Generación aleatoria de obstáculos

⸻

Salidas

Pantalla OLED SSD1306

Visualización de:

* menú,
* jugador,
* obstáculos,
* disparos,
* puntaje,
* tiempo.

Buzzer

Generación de sonidos mediante PWM.

LED

Indicador de colisión y estados del juego.

⸻

Funcionamiento del Sistema

Menú Principal

El usuario puede seleccionar entre los diferentes modos de juego utilizando los pulsadores.

⸻

Modo Clásico

El jugador debe esquivar obstáculos mientras la dificultad aumenta progresivamente.

⸻

Modo Tiempo

El jugador debe sobrevivir durante 60 segundos para obtener la victoria.

⸻

Modo Hardcore

Se incrementa la dificultad del juego:

* mayor velocidad,
* más obstáculos,
* y sistema de disparos.

⸻

Código

El código principal del proyecto se encuentra en:

main.py

Incluye:

* lectura de botones,
* control PWM,
* manejo de estados,
* generación de obstáculos,
* detección de colisiones,
* y actualización gráfica.

⸻

Comunicación y Control

I2C

Utilizado para la comunicación con la pantalla OLED SSD1306.

PWM

Utilizado para generar sonidos mediante el buzzer.

Temporización

Implementada utilizando:

* ticks_ms()
* ticks_diff()
* ticks_add()

para evitar bloqueos durante la ejecución del juego.

⸻

Resultados

Se implementó un videojuego funcional en ESP32 con múltiples modos de juego, control en tiempo real y generación dinámica de obstáculos.

El sistema logró integrar correctamente:

* entradas digitales,
* comunicación I2C,
* señales PWM,
* y programación basada en estados.
