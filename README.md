# control_tmp_ilum
Este proyecto (Actividad 2), se basa en Sistema de control y actuación en función del clima.

## Simulación en Wokwi
En el siguiente enlace se puede ver el código y probar el circuito: [https://wokwi.com/projects/432558575676350465](https://wokwi.com/projects/432573706929158145)

## Componentes Utilizados
- Arduino Uno
- Actuador: `8 LEDs`
- Actuadores a añadir: `Relés` que simulan calefacción y refrigeración
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

#### Lógica
Para el control de Tª: Setpoint de 25°C y zona muerta de ±3 °C. Si la tmeperatura se encuentra por encima de 25+3 se activa el enfriador (relé 1). Si esta por debajo de 25-3 se activa el calentador (relé 2); y si estuviera entre esos valores ambos apagados.

Para el control de la iluminación: el valor puede estar en el rango 0-1023 (actividad 1) y se escala a 8 leds. De tal forma que si hay luz baja más leds se encienden y si hay mucha luz pues menos leds.

LCD: En la primera línea de la primera pantalla se ve el valor de la temperatura y en la segunda el nivel de luz. En la siguiente pantalla se indica si es necesario activar alguno de los relés (para enfriar o calentar).

En esta actividad en vez de medir la temperatura y la luz con sensores se crean dos arrays, de esta forma se puede simular cambios en la temperatura (más frio o calor) y en la iluminación (día-noche).
