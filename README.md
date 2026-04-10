# SOLEMNE-1-El-Lissitzky.js
## Solemne 1 Pensamiento computacional Maximiliano Piña
![imagen](https://www.meisterdrucke.com/kunstwerke/1000px/Eliezer_Markowich_Lissitzky_-_Proun_ca_1923_-_%28MeisterDrucke-724036%29.jpg)
[link]( https://www.meisterdrucke.com/kunstdrucke/Eliezer-Markowich-Lissitzky/724036/Proun,-um-1923.html )

La obra Proun, um forma parte de la serie Proun de El Lissitzky en 1923, cuyo nombre proviene del acrónimo ruso “Proyecto para la afirmación de lo nuevo”. En esta entrega, busco recrear la obra utilizando p5.js.
## Proceso
Con la obra seleccionada, la abro en la herramienta de Canva, donde marco cada vértice de las figuras utilizando guías, lo que permite visualizar sus coordenadas exactas dentro de la composición original.

Al marcar y detectar cada vértice, identifico en la obra la complejidad de sus profundidades y superposiciones. Por ello, procedo a numerar y ordenar las figuras, para definir el orden en que debo colocarlas dentro del programa.

Con el orden ya definido, antes de crear las figuras utilizo la herramienta de cuentagotas para identificar los colores presentes en la obra y luego los incorporo en el programa.

![image alt](https://github.com/Mppinax/SOLEMNE-1-El-Lissitzky.js/blob/10fc153894cba2e3a9322c5d49904ae2b9902dac/guias.png)

##Complicaciones 
- El tamaño original de la obra es de 788 × 1000 px. En el canvas usé la mitad de ese tamaño para que no quedara tan grande. El problema fue que las coordenadas de las guías ya no coincidían, así que al principio tuve que dividir todas por 2 para que encajaran. Hice gran parte del trabajo así, pero después busqué una forma más eficiente y encontré *scale(0.5)*, lo que me permitió eliminar todos los */2* y simplificar el proceso.
- Al principio, especialmente con los cuadrados, estaba ordenando mal los vértices. En vez de seguir el orden 1, 2, 3, 4, los colocaba como 1, 2, 4, 3. Por eso, en lugar de verse como un cuadrado, se formaban dos triángulos reflejados, como si la figura tuviera una torsión en el centro.
- El cuentagotas me entregaba los colores en formato hexadecimal, así que tenía que pasarlos por un conversor para obtenerlos en RGB y poder usarlos en el programa.
- En la obra original se aprecia el rastro de la brocha en la pintura, pero no logré replicar ese efecto en el programa, ya que los colores se ven demasiado homogéneos. Intenté bajar la opacidad en algunos tonos, pero no me convenció, porque la transparencia se aplica de forma uniforme y no de manera irregular, como ocurre con las pinceladas reales.
- No pude asistir a la clase del 27 de marzo, que fue cuando se explicó el uso de GitHub, así que hacer este documento me costó bastante. Aun así, con los slides de la clase y algunos tutoriales, logré entender lo básico. 
