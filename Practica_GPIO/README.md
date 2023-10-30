<h2><FONT COLOR="red">Utilizando charlieplexing para ahorrar pines en el control de leds</FONT></h2>

Utilizamos charlieplexing en una barra de 10 leds, para mostrar un contador en formato binario, se utilizan 4 pines (pb12,pb13,pb14,pb15) para controlar 10 leds pero se pueden controlar hasta 12 leds. Con este metodo se pueden controlar n(n+1) siendo "n" el numero de pines utilizados, tambien se emplea un metodo similar a la multiplexacion para dar el efecto de que varios leds estan prendidos en el mismo momento. Se utiliza el systick timer ya que este metodo requiere que siempre se este visualizando los leds ,con retardos minimos, si desea prender un solo led a la vez, no es necesario ser tan extricto en los tiempos. En la imagen del repositorio se puede ver el funcionamiento simple de charlieplexing

![charlieplexing](https://github.com/ericksm248/Curso_STM32_proyectos/assets/147954327/38dc1d2b-b08f-4e1b-b4fc-6de974bf666f)

