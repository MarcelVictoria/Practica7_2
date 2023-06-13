## PRACTICA 7
En el ejercicio 1 hemos reproducido un audio desde la memoria interna de la ESP32.
## EJERCICIO 2: Reproducción de música desde una SD
Ahora el audio lo tenemos guardado en formato .mp3 en la microSD. Hemos conectado el lector de tarjetas y el altavoz de la siguiente manera:
```cpp
#define SD_CS 5
#define SPI_MOSI 23
#define SPI_MISO 19
#define SPI_SCK 18
#define I2S_DIN 25
#define I2S_BCLK 27
#define I2S_LRC 26
```
En el puerto MISO hemos puesto una resistencia en serie. El lector de SD está conectado a 5V mientras que el altavoz está conectado a 3.3V.

Hemos cogido el proyecto que nos proporciona la práctica: [Proyecto](https://github.com/schreibfaul1/ESP32-audioI2S). Hemos cambiado la línea de código donde se indica la ubicación del audio:
```cpp
audio.connecttoFS(SD, "Ensoniq-ZR-76-01-Dope-77.wav");
```
Después de varios intentos y tratando de modificar código y archivos de carpetas varias no hemos conseguido que funcionara.
En las siguientes imagenes mostramos el montaje de la practica:

[Imagen montaje](https://drive.google.com/file/d/1h1Csu99i50zItmCq6e60xiG2hL6dXFbS/view?usp=sharing)
[Imagen montaje](https://drive.google.com/file/d/1vjk8YkMSucTQ2aBK3kYj5b-6_lVw1mlK/view?usp=sharing)
[Imagen montaje](https://drive.google.com/file/d/1kKQuKayC2UA3azZbJwADz33UbG60JiE1/view?usp=sharing)
[Imagen montaje](https://drive.google.com/file/d/1JfcRzdaOgAc9kTMMKElZFbev7ZAZh09q/view?usp=sharing)