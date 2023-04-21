# ARDUINO_UNO-ATLAS
Diseño de un recolocador para ARDUINO UNO en la I/O BOARD ATLAS.

Esquema básico ARDUINO UNO con la I/O BOARD ATLAS:

señales ATLAS | Patillaje izquierda | patilaje derecha | señales ATLAS
| ---: | ---: | ---: | :---: 




NC | NC | PC5 | 
NC | NC | PC4 |
NC | NC | AREF | 
NC | NC | GND | GND
NC  | PB5 | GND | GND
IOREF  | IOREF | PB4| GND
RESET  | PC6 | PB3 | 
+3V3| +3V3 | PB2 | 
+5V | +5V | PB1 | JOY_DOWN
GND | GND | PB0 | JOY_RIGHT
GND | GND | PD7  | JOY_LEFT
 | ADC0 | PD6 | HSYNC
EAR |  ADC1 | PD5 | AUDIO_R
SD_CS |  ADC2 | PD4  | AUDIO_L
SD_CLK |  ADC3 | PD3 | BLUE[1]
SD_MISO |  ADC4 | PD2| 
SD_MOSI |  ADC5 | PD1| GREEN[1]
NC| NC | PD0| 


SPI FILAS/COLUMNAS| C1  | C2| C3
| ---: | ---: |  ---: | :---: 
F1| PC6 | SD_CLK| SD_MISO
F2| GND | SD_MOSI| +5V






---

Integrado usado en el Arduino Uno:

![Integrado ARDUINO](https://github.com/AtlasFPGA/ARDUINO_UNO-ATLAS/blob/main/FOTOS/arduinobasico.png)

---

Señales del Arduino Uno:

![Placa ARDUINO UNO](https://github.com/AtlasFPGA/ARDUINO_UNO-ATLAS/blob/main/FOTOS/UNO_PINOUT.png)

