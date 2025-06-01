# control_tmp_ilum
Este proyecto (Actividad 2), se basa en Sistema de control y actuación en función del clima.

## Simulación en Wokwi
En el siguiente enlace se puede ver el código y probar el circuito: [https://wokwi.com/projects/432558575676350465](https://wokwi.com/projects/432573706929158145)

## Componentes Utilizados
- Arduino Uno
- Sensor de temperatura y humedad: `DHT22`
- Sensor de luz: `LDR`
- Actuador: `8 LEDs`
- Actuadores a añadir: `Servo motores` que simulan calefacción y refrigeración
- Pantalla `LCD 1602 I2C`

## Funcionalidad
### Actividad 1 - Medición y Presentación
- Lectura de temperatura, humedad, iluminación, viento y calidad del aire.
- Visualización en dos pantallas secuenciales en el LCD.
  
### Actividad 2 - Control y Actuación (nuevas funcionalidades)
- Algoritmos de control:
  - Temperatura: On-Off con zona muerta
  - Iluminación: On-Off puro (8 niveles)
- Mensajes informativos en el LCD que indican acciones tomadas.
