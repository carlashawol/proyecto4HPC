# proyecto4HPC






**Problema o caso de estudio a resolver**

Se plantea abordar el problema que enfrentan muchas compañías y empresas actualmente al momento de adquirir mercancías, 
productos y servicios. La problemática aborda la gran cantidad de proveedores, marcas y empresas prestadoras de servicios que hay 
disponibles en el mercado; todas ellas con amplia variedad de calidad, precio y disponibilidad.
El problema que buscamos resolver es satisfacer la necesidad de estas mercancías, productos o servicios que requieren las empresas
para su operación. Para ellos tenemos en cuenta que las empresas tienen una lista de productos a adquirir y buscan que estos se 
puedan obtener en su totalidad por medio de una sola compañía; con el objetivo de reducir costos en impuestos, envíos, etc. 
Y con el fin de fidelizar sus proveedores para obtener descuentos o beneficios.

**Solución**

Para la solución de este problema decidimos realizar la implementación de un código en C con el cual llevaremos a cabo una multiplicación
de matrices haciendo uso de OpenMP y paralelización la cual nos dará el resultado de una matriz con la cual se puede realizar el análisis
al momento de decidir cuál proveedor se elegirá para realizar una compra de productos. 

Para este problema tendremos en cuenta el concepto de curva de indiferencia; el cual supone que para cierta compra de bienes o servicios
se tiene la misma satisfacción independientemente de las cantidades de los mismos. Teniendo como resultado que para una compañía puede
significar el mismo nivel de satisfacción adquirir 10 unidades del producto 1 y 2 unidades del producto 2; que 7 unidades del producto 1
y 3 unidades del producto 2.

Para nuestro problema planteamos las siguientes matrices. La primera matriz tiene por columnas los diferentes productos que una
determinada compañía desea adquirir; por columnas tiene las diferentes compras que desea realizar las cuales se supone aportan la misma
satisfacción para la empresa. La matriz contiene las cantidades de cada producto dependiendo de la compra.

La segunda matriz tiene por columnas los diferentes proveedores con los cuales la compañía podría llevar a cabo la compra. Y por columnas
contiene los productos que ofrece cada proveedor, los cuales coinciden con los que desea adquirir la compañía. La matriz contiene los
precios de cada proveedor para cada producto.
![alt text](https://github.com/carlashawol/proyecto4HPC/blob/master/Captura%20de%20pantalla%20(597).png)

Con el resultado de la ejecución podemos deducir que sumando todos los campos de cada una de las columnas de la matriz resultante podemos obtener el total del costo de la compra de la compañía con cada uno de los proveedores. El proveedor a elegir será con el cual el costo total de la compra sea menor.

![alt text](https://github.com/carlashawol/proyecto4HPC/blob/master/Captura%20de%20pantalla%20(598).png)

![alt text](https://github.com/carlashawol/proyecto4HPC/blob/master/Captura%20de%20pantalla%20(596).png)

De los datos capturados y cálculo de speedUp y eficiencia podemos concluir lo siguiente:

Deducimos que el tiempo de ejecución disminuye al implementar paralelización en el código y al aumentar el número de procesadores.
A su vez observamos un aumento en el speedUp cuando aplicamos paralelización y aumentamos el número de procesadores. Con dos procesadores tenemos que el speedUp es de 2.66, con 3 procesadores el speedUp aumenta a 4 y con 4 procesadores el speedUp aumenta a 12. Mientras mayor sea el speedUp, mayor será la eficiencia del algoritmo, con respecto al algoritmo secuencial.
Observamos que al aplicar paralelización y aumentar el número de procesadores, aumenta a su vez la eficiencia, ya que se reduce la complejidad del algoritmo.


**Declaración**

Juan Diego: Declaro que el proyecto es original. Mi aporte dentro del desarrollo del proyecto fue el siguiente:

--Aporte en la realización del código paralelizado y secuencial.

--Aporte en la toma de datos contundentes y análisis de los mismos.

--Aporte en el diseño de la métodología PCAM para el proyecto.

Carla Rendón:Declaro que el proyecto es original. Mi aporte dentro del desarrollo del proyecto fue el siguiente:

--Aporte en la realización del código paralelizado y secuencial.

--Aporte en la toma de datos contundentes y análisis de los mismos.

--Aporte en el diseño de la métodología PCAM para el proyecto.
