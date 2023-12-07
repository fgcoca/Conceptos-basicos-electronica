# <FONT COLOR=#8B008B>Conversión ADC y DAC</font>
En un sistema microcontrolado existe la necesidad de poder trabajar con señales que no sean digitales, como lo son la mayoría de las variables que nos rodean, por lo tanto se hace necesario implementar una conversión de la información de entrada analógica a digital y el dispositivo se encargará también de convertir al contrario.

* La conversión analógica a digital la realiza el dispositivo ADC (Analog to Digital Converter)
* La conversión digital a analógica la realiza un dispositivo DAC (Digital to Analog Converter)

Ya hemos visto anteriormente como una señal analógica se representa mediante valores discretos y cambian continuamente con el tiempo mientras que una señal digital se representa mediante valores discretos.

Un conversor ADC se utiliza para convertir señales analógicas, como tensiones, en señales digitales o binarias formada por unos y ceros.

El rango del módulo ADC que lleva el dispositivo tendrá un determinado número de bits de resolución. A continuación indicamos el dato para diferentes dispositivos:

* Pi Pico y ESP32: resolución = 12 bits, lo que significa que su resolución es de $2^{12}=4096 \space bits$, por lo que su rango (a 3,3V) se dividirá en 4096 partes iguales.
* Arduino y micro:bit: resolución = 10 bits, lo que significa que su resolución es de $2^{10}=1024 \space bits$, por lo que su rango (a 3,3V) se dividirá en 1024 partes iguales.

Cualquier valor analógico puede ser mapeado a un valor digital usando la resolución del conversor. Por tanto, cuantos más bits tenga el ADC, de más precisión será el muestreo del analógico y mayor la precisión de la conversión resultante.
