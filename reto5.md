Reto 5: Sistema de Inventario para una mini tienda

La mini tienda de Pepe vende diferentes productos, usualmente frutas, dulces y algunos tipos de carne. Con el propósito de mejorar el control sobre las ventas y el inventario de la tienda, Pepe decide construir una aplicación que le permita almacenar la información de los productos y realizar algunos cálculos sobre los datos.

En la primera parte del reto se debe construir una base de datos que almacene la información de los productos disponibles en la tienda. Debido a que Pepe no cuenta con un servidor de base de datos, solicita que temporalmente la base de datos sea representada mediante un diccionario de Python llamado productos que tendrán por llave el código del producto y por valor una lista formada por los atributos: precio e inventario. La Tabla 1 presenta los productos disponibles a la fecha.


código	nombre	   precio	 inventario
1	   Manzanas	   8000,0	 sesenta y cinco
2	   Limones	   2300.0	 15
3	   Granadilla  2500,0	 38
4	   Arandanos   9300.0	 55
5	   Tomates	   2100.0	 42
6	   Fresas	   4100.0	 3
7	   Helado	   4500.0	 41
8	   Galletas	   500,0	 8
9	   Chocolates  3500,0	 806
10	   Jamón	   15000,0	 10
Tabla 1: Productos disponibles en la tienda.

Para simular de una manera más realista la base de datos, es necesario construir 3 funciones que representan las operaciones de: AGREGAR, ACTUALIZAR y BORRAR los productos disponibles. Se debe implementar una función independiente por cada una de las acciones mencionadas. En este caso, para poder realizar las operaciones de ACTUALIZAR o BORRAR es necesario especificar todos los atributos del producto.

Además, Pepe está interesado en analizar los datos de los productos disponibles y conocer: el nombre del producto con el precio mayor; el nombre del producto con el precio menor; el promedio de precios de todos los productos y el valor total del inventario a la fecha. Este último se obtiene multiplicando el precio de cada producto por el inventario disponible y luego sumando todos los resultados. Por ejemplo, al calcular estos 4 valores para los datos disponibles en la Tabla 1 obtendríamos:
Producto precio mayor: Jamon
Producto precio menor: Galletas
Promedio de precios: 5180.0
Valor del inventario: 4421000.0

Entrada:
Cada uno de los casos de prueba estará compuesto por dos líneas.
La primera línea estará formada por una cadena de texto que identifica la operación a realizar. En este caso, las operaciones validas son:
ACTUALIZAR.
BORRAR.
AGREGAR.
La segunda línea estará formada por 4 valores (código, nombre, precio, inventario) que representan el producto sobre el cual se quiere realizar la operación.
En el caso de la operación ACTUALIZAR la segunda línea debe contener el código y los nuevos valores del producto.
En el caso de la operación BORRAR se deben especificar todos los atributos del caso de producto a eliminar.

Salida: 
La salida estará representada por una única línea formada por cuatro valores:
Nombre del producto con el precio mayor.
Nombre delproducto con el precio menor.
Promedio de precios.
Valor del inventario.
Estos 4 valores deben imprimirse después de realizar las operaciones solicitadas en la entrada de datos.
Los valores numéricos deben imprimirse con un número decimal.
En caso de solicitar ACTUALIZAR o BORRAR un producto que no existe (es decir, que el código del producto no se encuentra en la base de datos), se debe imprimir 'ERROR'.
En caso de solicitar AGREGAR un producto cuyo código ya existe en la base de datos se debe imprimir 'ERROR'.

Instrucciones
Instrucciones para la calificación automática

Antes de enviar la solución del reto, por favor tenga en cuenta los siguientes aspectos:
Cada caso de prueba se especifica con dos líneas.
Cada línea debe contener los valores de los parámetros requeridos separados por un espacio.
Es importante no utilizar ningún mensaje a la hora de capturar las entradas, es decir, utilizar la función input () no agregue ningún texto para capturar los datos.
Los resultados se muestran en una única línea. Los dos valores requeridos deben estar separados por un espacio.
Casos de prueba

Entrada	
AGREGAR
11 Melón 70 13
BORRAR
10 Jamón 15000 10
ACTUALIZAR
7 Helado 65000 11
BORRAR
14 Maíz 45000 12

Salida	
Jamón Melón 4715.5 4421910.0
Arandanos Galletas 4088.9 4271000.0
Helado Galletas 11230.0 4951500.0
ERROR