
![](https://github.com/Lperazo2/Fundamentos-de-Circuitos-Electricos/blob/754398f438566d25f4b7809930ac0c199aef01ba/1.PNG)


# Tema: 
# Diseño de circuitos mixtos y toma de mediciones en NGSPICE

2. Objetivo General
* Conocer la herramienta de simulación NGSPICE y desarrollar en ella un circuito eléctrico mixto, misma que nos otorgara todos los datos de corrientes presentes en los nodos del sistema, el presente trabajo se realizara mediante la búsqueda de información autónoma y los conocimientos adquiridos en el salón de clases, para de esta manera fortalecer los conocimientos y familiarizarnos con una nueva herramienta de simulación de circuitos eléctricos.

3. Objetivo específico:
* Instalar NGSPICE, desarrollar en ella el circuito eléctrico mixto planteado y recopilar los datos obtenidos.
* Resolver el ejercicio eléctrico empleando los conocimientos teóricos impartidos por el tutor y recopilar datos.
* Simular el circuito eléctrico en Multisim y comprar con los resultados anteriores.

3.	Marco teórico:

En la página oficial de ngspice, se nos indica que este es un simulador de código abierto para circuitos eléctricos y electrónicos. Informa sobre las cualidades y funcionalidades como JFET, transistores bipolares y MOS, elementos pasivos como R, L o C, diodos, líneas de transmisión y otros dispositivos, todos interconectados en una lista de conexiones.

4.	Datos a obtener:

* Caídas de voltajes de todos los elementos del circuito planteado
* Corriente de todas las mallas presentes en el circuito
* Corriente de todos los nodos existentes en el ejercicio
 
5.	Descripción del circuito eléctrico

![](https://github.com/Lperazo2/Fundamentos-de-Circuitos-Electricos/blob/905359004492d9fb63a6e7e166501856d2023510/2.PNG)

Características principales

•	Encontramos 4 resistencias y 2 fuentes de voltaje, una independiente y otra dependiente de la corriente i

6.	Resolución del ejercicio

I.- Aplicamos el método de mallas en el presente ejercicio

![](https://github.com/Lperazo2/Fundamentos-de-Circuitos-Electricos/blob/3429e41ba8365856527272557302cc631245e9f8/3.PNG)

II.- Generamos un sistema de ecuaciones considerando que I_2=i puesto a que es la corriente de esta malla.

![](https://github.com/Lperazo2/Fundamentos-de-Circuitos-Electricos/blob/3429e41ba8365856527272557302cc631245e9f8/4.PNG)

III.- Resolvemos el sistema de ecuaciones por medio de una calculadora virtual

![](https://github.com/Lperazo2/Fundamentos-de-Circuitos-Electricos/blob/3429e41ba8365856527272557302cc631245e9f8/5.PNG)

Esto nos indica que:

![](https://github.com/Lperazo2/Fundamentos-de-Circuitos-Electricos/blob/3429e41ba8365856527272557302cc631245e9f8/6.PNG)

Nota: El signo negativo solo indica que el sentido de la corriente es el contrario al estipulado al inicio.

IV.-	Encontramos el valor del voltaje 2i = 3.75v

V.-	Reestructuramos el ejercicio para poder resolverlo en ngspice

![](https://github.com/Lperazo2/Fundamentos-de-Circuitos-Electricos/blob/3429e41ba8365856527272557302cc631245e9f8/7.PNG)

VI.-	Este circuito será resuelto en el simulador ngspice para lo cual hay que entender lo siguiente

Para insertar los elementos hay que seguir el siguiente esquema

0 = Tierra

DC = Corriente directa

![](https://github.com/Lperazo2/Fundamentos-de-Circuitos-Electricos/blob/3429e41ba8365856527272557302cc631245e9f8/8.PNG)

![](https://github.com/Lperazo2/Fundamentos-de-Circuitos-Electricos/blob/3429e41ba8365856527272557302cc631245e9f8/9.PNG)

VII.-	Explicamos los resultados expuestos en el simulador

![](https://github.com/Lperazo2/Fundamentos-de-Circuitos-Electricos/blob/3429e41ba8365856527272557302cc631245e9f8/10.PNG)

VIII.-	Resultados de la simulación

![](https://github.com/Lperazo2/Fundamentos-de-Circuitos-Electricos/blob/3429e41ba8365856527272557302cc631245e9f8/11.PNG)

IX.-	Para comprobar estos todos resolvemos el circuito por el método de nodos y simularemos el circuito en Multisim.

![](https://github.com/Lperazo2/Fundamentos-de-Circuitos-Electricos/blob/3429e41ba8365856527272557302cc631245e9f8/12.PNG)

![](https://github.com/Lperazo2/Fundamentos-de-Circuitos-Electricos/blob/3429e41ba8365856527272557302cc631245e9f8/13.PNG)

Por lo tanto, las corrientes I1, I2 y I3:

![](https://github.com/Lperazo2/Fundamentos-de-Circuitos-Electricos/blob/3429e41ba8365856527272557302cc631245e9f8/14.PNG)

Ley de corrientes para el Nodo B:

![](https://github.com/Lperazo2/Fundamentos-de-Circuitos-Electricos/blob/3429e41ba8365856527272557302cc631245e9f8/15.PNG)

Por lo tanto, las corrientes I4, I5 y I6:

![](https://github.com/Lperazo2/Fundamentos-de-Circuitos-Electricos/blob/3429e41ba8365856527272557302cc631245e9f8/16.PNG)

Ley de corrientes para el Nodo C:

![](https://github.com/Lperazo2/Fundamentos-de-Circuitos-Electricos/blob/3429e41ba8365856527272557302cc631245e9f8/17.PNG)

Por lo tanto, las corrientes I7, I8 y I9:

![](https://github.com/Lperazo2/Fundamentos-de-Circuitos-Electricos/blob/3429e41ba8365856527272557302cc631245e9f8/18.PNG)

Representamos el circuito en Multisim

![](https://github.com/Lperazo2/Fundamentos-de-Circuitos-Electricos/blob/3429e41ba8365856527272557302cc631245e9f8/19.PNG)

7.	Tabla general de resultados

![](https://github.com/Lperazo2/Fundamentos-de-Circuitos-Electricos/blob/3429e41ba8365856527272557302cc631245e9f8/20.PNG)

8.	Conclusiones

* Los resultados obtenidos por el programa NGSPICE son confiables, puesto a que sus resultados son exactamente los mismos que los adquiridos en los datos teóricos y en la simulación realizada en Multisim.
* NGSPICE es un programa de simulación sencillo, pero para su utilización aparte de conocer los comandos, es indispensable saber cuántos nodos se encuentran dentro de un sistema eléctrico, lo cual permite fortalecer conocimientos identificando nodos fantasmas, principales y de referencia.  

9.	Recomendaciones

* Se debe evitar errores de sintaxis dentro del programa NGSPICE, puesto a que su interfaz puede confundir una letra mayúscula y minúscula, lo cual evita que el simulador procese correctamente los datos ingresados
* Al conocer los nodos en el simulador se debe considerar la dirección en la que está el polo positivo y negativo de los elementos a medir.
                            
                                               
# Tema: 
# Creación de una Aplicación móvil en App inventor para la resolución de ejercicios en serie, paralelo y ley de ohm

2. Objetivo General
* Conocer la herramienta de desarrollo de aplicaciones virtual MIT APP INVENTOR y desarrollar en ella una aplicación que permita la resolución de un circuito eléctrico en serie y en paralelo, el programa debe otorgara todos los datos de corrientes y caidas de voltajes presentes en cada circuito, asi como también ayude a resolver problemas relacionados con la Ley de Ohm, el presente trabajo se realizará mediante la búsqueda de información autónoma y los conocimientos adquiridos en el salón de clases, para de esta manera fortalecer los conocimientos y familiarizarnos con una nueva herramienta para crear aplicaciones y resolver circuitos eléctricos simples.

3. Objetivos específicos:
* Ingresar a MIT Inventor y familiarizarnos con la interfaz
* Diseñar un apartado sencillo para que el usuario pueda manejarlo de manera ágil.
* Generar un APK y compartirlo en github

3.	Marco teórico:

En la página oficial de MIT APP INVENTOR, se nos indica que esta es una página de sotfware libre en el cual se nos permite crear una gran variedad de aplicaciones compatibles con dispositivos android, al ser de código abierto el proyecto de crear una app para resolver circuitos eléctricos en serie y paralelo no representara ninguna dificultad y se permitirá al programador emitir todos los datos que se pueden extraer de un circuito eláctrico o de las leyes de Ohm.

4.	Datos a obtener:

* Caídas de voltajes de todos los elementos de los circuitos
* Corriente de todas las mallas presentes en los circuitos
* Resolver los diferentes problemas que pueden llegar a darse en la Ley de Ohm
 
5.	Descripción de los apartados de la aplicación 

![](https://github.com/Lperazo2/Ejercicios-Extras-FCE-P1/blob/68e4c69053dd9998d453c2fe5fce96a763b68b62/serie_1.png)

Al ser un circuito en serie con tres resistencias los datos a obtener son:
* It = Intensidad total
* VR1 = caidad de voltaje en la R1
* VR2 = caidad de voltaje en la R2
* VR3 = caidad de voltaje en la R3

![](https://github.com/Lperazo2/Ejercicios-Extras-FCE-P1/blob/68e4c69053dd9998d453c2fe5fce96a763b68b62/Paralelo_1.png)

Al ser un circuito en paralelo con tres resistencias los datos a obtener son:
* IR1 = Intensidad que para por R1
* IR2 = Intensidad que para por R2
* IR3 = Intensidad que para por R3
* It = Intensidad total
* VT = El voltaje que cae en cada resistencia

![](https://github.com/Lperazo2/Ejercicios-Extras-FCE-P1/blob/68e4c69053dd9998d453c2fe5fce96a763b68b62/Ley_Ohm.png)

La ley de Ohm permite obtener: la resistencia, el voltaje o la corriente de la siguiente manera:
* Conociendo el voltaje y la intencidad podemos determinar la resistecia
* Conociendo el voltaje y la resistencia podemos determinar la intensidad 
* Conociendo la resistencia y la intencidad podemos determinar el voltaje  

6.- Desarrollo de la Aplicación

# Interfaz de inicio

![](https://github.com/Lperazo2/Ejercicios-Extras-FCE-P1/blob/68e4c69053dd9998d453c2fe5fce96a763b68b62/31.PNG)

![](https://github.com/Lperazo2/Ejercicios-Extras-FCE-P1/blob/68e4c69053dd9998d453c2fe5fce96a763b68b62/32.PNG)

# Apartado para calcular un circuito en serie

![](https://github.com/Lperazo2/Ejercicios-Extras-FCE-P1/blob/68e4c69053dd9998d453c2fe5fce96a763b68b62/33.PNG)

![](https://github.com/Lperazo2/Ejercicios-Extras-FCE-P1/blob/68e4c69053dd9998d453c2fe5fce96a763b68b62/34.PNG)

# Apartado para calcular un circuito en paralelo

![](https://github.com/Lperazo2/Ejercicios-Extras-FCE-P1/blob/68e4c69053dd9998d453c2fe5fce96a763b68b62/35.PNG)

![](https://github.com/Lperazo2/Ejercicios-Extras-FCE-P1/blob/68e4c69053dd9998d453c2fe5fce96a763b68b62/36.PNG)

# Apartado para calcular la ley de Ohm

![](https://github.com/Lperazo2/Ejercicios-Extras-FCE-P1/blob/68e4c69053dd9998d453c2fe5fce96a763b68b62/37.PNG)

![](https://github.com/Lperazo2/Ejercicios-Extras-FCE-P1/blob/68e4c69053dd9998d453c2fe5fce96a763b68b62/38.PNG)

7.	Conclución
* La aplicación desarrollada cumple con lo planeado, su ejecución en un dispositivo android es correcta y los resultados obtenidos por medio de la misma no difieren de la realidad, podemos asegurar que la aplicación funciona y es fiable.


