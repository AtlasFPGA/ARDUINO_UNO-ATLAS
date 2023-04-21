# ARDUINO_UNO-ATLAS
Diseño de un recolocador para ARDUINO UNO en la I/O BOARD ATLAS.

Esquema básico ARDUINO UNO con la I/O BOARD ATLAS:

señales ATLAS | Patillaje izquierda | patilaje derecha | señales ATLAS
| ---: | ---: | ---: | :---: 
NC | NC | PC5 R3*| PI_TX -> PI_I2C_SCL
NC | NC | PC4 R3*| PI_RX -> PI_I2C_SDA
NC | NC | AREF | AREF
NC | NC | GND | GND
NC*  | NC* | GND | GND
IOREF  | IOREF R3*| PB4| KB_DATA
RESET  | PC6 | PB3 | KB_CLK
+3V3| +3V3 | PB2 | SD_CSS
+5V | +5V | PB1 | JOY_P1
GND | GND | PB0 | JOY_P2
GND | GND | PD7  | AUDIO_MONO
EAR | ADC0 | PD6 | BLUE[1]
VIDEO_COMPOSITE[1] |  ADC1 | PD5 | GREEN[1]
JOY_UP_ANALOG |  ADC2 | PD4  | RED[1]
JOY_DOWN_ANALOG |  ADC3 | PD3 | HSYNC
JOY_RIGHT_ANALOG |  ADC4 | PD2| VSYNC
JOY_LEFT_ANALOG |  ADC5 | PD1| EAR
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

