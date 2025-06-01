# control_tmp_ilum
Este proyecto (Actividad 2), se basa en Sistema de control y actuación en función del clima.

## Simulación en Wokwi
En el siguiente enlace se puede ver el código y probar el circuito: https://wokwi.com/projects/432558575676350465

## Componentes Utilizados
- Arduino Uno
- Sensor de temperatura y humedad: `DHT22`
- Sensor de luz: `LDR`
- Sensor de calidad del aire: `Potenciómetro`
- Sensor de viento: `Joystick` (para velocidad y dirección)
- Actuador: `LED rojo` (indica mala calidad del aire)
- Actuadores a añadir: `LEDs o mensajes` que simulan ventilador y humidificador
- Pantalla `LCD 1602 I2C`

## Funcionalidad
### Actividad 1 - Medición y Presentación
- Lectura de temperatura, humedad, iluminación, viento y calidad del aire.
- Visualización en dos pantallas secuenciales en el LCD.
  
### Actividad 2 - Control y Actuación (nuevas funcionalidades)
- Activación de actuadores simulados:
  - 💨 Ventilador si temperatura > 25 °C
  - 💧 Humidificador si humedad < 80%
- Mensajes informativos en el LCD que indican acciones tomadas.
- Control automático basado en algoritmos simples.
- El sistema busca mantenerse cerca de los parámetros:
  - Temperatura: 25 °C
  - Humedad: 80%
