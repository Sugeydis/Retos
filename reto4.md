Reto 4: Detectando nombres de yogurt iguales

Un trabajador en una línea de producción de empaque de yogurt está comenzando a perder su memoria. Hace algún tiempo, cuando comenzó a trabajar en la empresa, no únicamente conocía perfectamente todos los nombres de los distintos sabores de yogurt, sino que además contaba con una habilidad increíble para detectar nombres iguales en las cajas que se empacaban durante su turno de trabajo.

La habilidad del trabajador se basa en su memoria fotográfica. Cuando el trabajador revisaba las cajas que empacaba con el yogurt era capaz de recordar a la perfección si había visto un yogurt con el mismo nombre o no, y si los pudimos saber en que caja estaba el nombre duplicado. Lamentablemente, durante los últimos meses su memoria fotográfica ya no funciona como antes y ahora solo recuerda algunas de las últimas cajas que ha revisado.

Debido a estas circunstancias, el trabajador ha decidido solicitar ayuda para construir un programa en Python que le permita comprobar si la perdida de su memoria fotográfica podría tener como consecuencia una disminución en la cantidad de nombres de yogurt que se detectan durante la revisión de las cajas .

Entrada:
La entrada estará formada por dos líneas:
La primera línea aparecerán dos números P: indican el número de cajas a revisar y Q: el número de cajas de yogurt que el trabajador es capaz de recordar (1≤P≤1000,1≤Q≤1000).
La segunda línea contiene N números (entre 1 y 10) separados por espacios que representan los nombres de cada uno de los yogures empacados.
Dos yogures se consideran duplicados si están representados por el mismo número.

Salida:	
El programa imprimirá dos números separados por un espacio.

El primero representará el número total de yogures con nombres iguales.
El segundo representará la cantidad de nombres de yogures detectados por el trabajador considerando que al revisar una caja solo es capaz de recordar las Q cajas anteriores.

Instrucciones
Instrucciones para la calificación automática

Antes de enviar la solución del reto, por favor tenga en cuenta los siguientes aspectos:
Cada caso de prueba se especifica con dos líneas.
Cada línea debe contener los valores de los parámetros requeridos separados por un espacio.
Es importante no utilizar ningún mensaje a la hora de capturar las entradas, es decir, utilizar la función input () no agregue ningún texto para capturar los datos.
Los resultados se muestran en una única línea. Los dos valores requeridos deben estar separados por un espacio.
Casos de prueba

Entrada	5 1
1 2 3 1 2 1 1
5 2
1 2 3 1 2
5 3
1 2 3 1 2
5 1
1 1 1 1 1 1 1 1
Salida	4 1
2 0
2 2
7 7

