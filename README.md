# ARDUINO_UNO-ATLAS
Diseño de un recolocador para ARDUINO UNO en la I/O BOARD ATLAS.
Vionado del diseño:
https://www.youtube.com/watch?v=ql8l04nuYEk
---

Visualización superior

![Visualización inferior](https://github.com/AtlasFPGA/ARDUINO_UNO-ATLAS/blob/main/FOTOS/ARDUINO_UNO-ATLAS-3D-CARA-SUPERIOR-RAY.jpg)


Visualización inferior

![Visualización superior](https://github.com/AtlasFPGA/ARDUINO_UNO-ATLAS/blob/main/FOTOS/ARDUINO_UNO-ATLAS-3D-CARA-INFERIOR-RAY.jpg)

---


Esquema básico ARDUINO UNO con la I/O BOARD ATLAS:

Teniendo como base el pong realizado en ARDUINO UNO y expandiendo las señales todo lo posible con la I/O BOARD ATLAS:

https://blog.arduino.cc/2015/09/24/yet-another-cool-pong-with-arduino-uno/

También del ejemplo de pineado VGA con 8 colores:
https://forum.arduino.cc/t/turn-your-uno-into-a-vga-output-device/99969/9

---

Avance 22 Abril del 2023 Esquemático:

![Avance 22 Abril del 2023 Esquemático](https://github.com/AtlasFPGA/ARDUINO_UNO-ATLAS/blob/main/FOTOS/Esquem%C3%A1tico%20en%20desarrollo%20para%20ARDUINO%20UNO.png)

Avance 22 Abril del 2023 PCB:

![Avance 22 Abril del 2023 PCB](https://github.com/AtlasFPGA/ARDUINO_UNO-ATLAS/blob/main/FOTOS/Placa_PCB_ARDUINO_UNO_ATLAS.png)

---

1[ARDUINO UNO VGA8](https://github.com/AtlasFPGA/ARDUINO_UNO-ATLAS/blob/main/FOTOS/ARDUINO_UNO_VGA_8COLORES.jpeg)

señales ATLAS | Patillaje izquierda | patilaje derecha | señales ATLAS
| ---: | ---: | ---: | :---: 
NC | NC | PC5 R3*| PI_TX -> PI_I2C_SCL
NC | NC | PC4 R3*| PI_RX -> PI_I2C_SDA
NC | NC | AREF | AREF
NC*  | NC* | GND | GND
VAVIO | VACIO | 13 | M_DATA
IOREF  | IOREF R3*| PB4| Key_DATA
RESET  | PC6 | PB3 | Key_CLK
+3V3| +3V3 | PB2 | SD_CS
+5V | +5V | PB1 | Joy_FIRE1
GND | GND | PB0 | M_CLK
GND | GND | PD7  | DELTASIGMA_L
EAR | ADC0 | PD6 | BLUE[1] -> TMDS_0_P
VIDEO_COMPOSITE[1] |  ADC1 | PD5 | GREEN[1] -> TMDS_1_P
JOY_UP_ANALOG |  ADC2 | PD4  | RED[1] -> TMDS_2_P
JOY_DOWN_ANALOG |  ADC3 | PD3 | HSYNC -> TMDSC_N
JOY_RIGHT_ANALOG |  ADC4 | PD2| VSYNC -> TMDSC_P
JOY_LEFT_ANALOG |  ADC5 | PD1| DELTASIGMA_R
NC| NC | PD0| VIDEO_COMPOSITE[0]



SPI FILAS/COLUMNAS| C1  | C2| C3
| ---: | ---: |  ---: | :---: 
F1| PC6 *RESET| SD_CLK| SD_MISO
F2| GND | SD_MOSI| +5V






---

Integrado usado en el Arduino Uno:

![Integrado ARDUINO](https://github.com/AtlasFPGA/ARDUINO_UNO-ATLAS/blob/main/FOTOS/arduinobasico.png)

---

Señales del Arduino Uno:

![Placa ARDUINO UNO](https://github.com/AtlasFPGA/ARDUINO_UNO-ATLAS/blob/main/FOTOS/UNO_PINOUT.png)

