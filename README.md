# comedero-inteligente-EL1200
Comedero automático para gatos con ESP32, sensor PIR y servomotor

Proyecto del curso EL-1200 Introducción a la Electrónica, TEC, II semestre 2026

## Descripción

Comedero automático que dispensa alimento solo cuando detecta al gato y evita servir de más si el gato se queda frente al plato.

## Funcionamiento

- El sensor PIR detecta la presencia del gato.
- El servomotor abre la compuerta durante 1,5 segundos y la vuelve a cerrar.
- El LED indica que se está sirviendo.
- Una variable booleana (dispensado) evita que se sirva otra vez mientras el gato sigue ahí.

## Conexiones

| Componente | Pin del ESP32 |
|---|---|
| Sensor PIR | GPIO 2 |
| Servomotor | GPIO 13 |
| LED (con 220 Ω) | GPIO 5 |
| Alimentación | 3V3 y GND |

## Simulación

Proyecto en Wokwi: https://wokwi.com/projects/481345822057182209

## Código

El código del ESP32 se encuentra en el archivo sketch.ino.

La biblioteca utilizada se encuentra en el archivo bibliotecas.

## Evidencia

![Simulación](media/capturacomedero.png)
