#Capitulo 4

## Proceso de desarrollo de pruebas
Los casos de prueba deben ser tomados de los requerimientos 
> **Trazabilidad**
> > Las pruebas deben ser trazables -> Que requisitos han sido cubiertos por cuales casos de prueba?
> > Permite definir la cobertura de requisitos
> > Si hay un cambio se puede determinar cuales casos de prueba son afectados 


>**Objeto de pruebas**
> > Elemento a ser revisado (Documento, codigo , programa)
>
> **Condicion de pruebas**
> > Elemento o evento de un componente o sistema que deveria ser verificado or uno o mas casos de prueba
>
>**Criterios de prueba**
> > El objeto de pruebas debe cumplir los criterios de prueba con el objeto de superar la preuba
>
>
>**Calendario de ejecucion de pruebas**
> > Esquema de ejecucion de las pruebas
>
>
>**Especificacion de diseño de pruebas**
> > Documento que especifica las condiciones de prueba, el enfoque de preuba de forma detallada e identifica los casos de prueba a alto nivel
>
>**Especificacion de casos de prueba**
>> Documentacion que especifica un conjunto de casos de prueba para un elemento 




####**Caso de prueba**
* **Precondiciones**
* **Valores de entrada**
* **Resultados esperados**
* **Postcondiciones**
*  **Dependencias**
*  **Identificador**
* **Requisitos**

---

Los casos de prueba se pueden combinar en juegos de prueba y escenarios de prueba. 

Ademas los juegos de pruebas  pueden ser automatizados con herramientas apropiadas

El calendario de pruebas define el orden de la ejecucion de los procedimeintos de prueba y la automatizacion de pruebas

## Categorias de tecnicas de diseño de prueba

### Metodos basados en la especificaion - Caja Negra
Los casos de prueba se obtienen a partir del analisis de la especificion funcional y no funcional del objeto de pruebas

La funcionalidad es el foco de las pruebas

### Metodos basados en la estructura - Caja Blanca - Prueba basada en el flujo de control
El foco de atencion es la estructura del codigo/sistema y su estructura

### Metodos basados en la experiencia
La fuente para el diseño de los casos de prueba son el conocimiento y la experiencia del objeto de pruebas

Se detectan posible puntos debiles, posibles errores o errores detectados anteriormente

## Tecnicas de Caja Negra o basadas en la especificacion

Tienen como finalidad la verificacion de la correcion y completitud de una funcion.

``` Se cubrieron todas las funcionalidades, todos los resultados son los correctos ```

### Tipos
* **Particiones de equivalencia**
* **Análisis de Valores Limite**
* **Tablas de Desición**
* **Pruebas de Transición de Estado**
* **Pruebas de caso de uso**
* **Pruebas de humo**
* **Pruebas estadisticas**



#### **Particiones de equivalencia**

<iframe width="560" height="315" src="https://www.youtube.com/embed/Uo2xvx7zhwo" frameborder="0" allowfullscreen></iframe>

```
Coberutura(CE)  =   

   Numero de CE Probadas 

   _____________________  * 100

   Numero de CE Definidas
```
#### **Análisis de Valores Limite**

<iframe width="560" height="315" src="https://www.youtube.com/embed/7FMFXLmu-sw" frameborder="0" allowfullscreen></iframe>

#### **Tablas de Desición**

<iframe width="560" height="315" src="https://www.youtube.com/embed/6g9cYF0_J7Q" frameborder="0" allowfullscreen></iframe>

#### **Pruebas de Transición de Estado**

<iframe width="560" height="315" src="https://www.youtube.com/embed/98LWGvhVSpE" frameborder="0" allowfullscreen></iframe>

#### **Pruebas de caso de uso**
Los casos de prueba se obtienen directamente de los casos de uso creados, cada caso de uso tiene un caso de prueba, cada alternativa del caso de uso debe tner tambien un caso de prueba.

Estos casos de uso se definen como la interaccion de un usuario con el sistema generalmente se utiliza el diagrama de casos de uso UML.

Contienen: 

* Precondiciones
* Resultados esperados / Comportamiento del sistema
* Post condiciones

Se utilizan en las pruebas de sistema y las pruebas de aceptacion.

Su principal desventaja es que no se pueden obtener casos de prueba adicionales directo del caso de uso sino que hay que recurir a otros documentos para obtener mas contexto acerca del sistema.



## Tecnicas de caja Blanca o basadas en a estructura - Prueba basada en el flujo de control

Son tecnicas q se ejecutan en los niveles de prueba de componente, integracion y de sistema, se utilizan herramientas para una mejor calidad de pruebas


### Cobertura de sentencia

Se basa en el porcentaje de sentencias ejecutables que son ejecutados por las pruebas. Se utiliza el grafo de flujo de control.

**El objetivo de prueba es lograr la cobertura de un porcentaje especifico de todas las sentencias**

```
Cobertura de sentencia = 

   Numero de sentencias ejecutadas 
   
   ------------------------------- * 100%
   
   Numero total de sentencias

```

Con este metodo se pueden encontar sentencias q nunca se ejecutan en el sistema, ademas si una funcionalidad no esta implementada este metodo no podra determinarlo dado que el mismo se basa solo en lo que esta escrito en el codido y sus sentencias

<iframe width="854" height="480" src="https://www.youtube.com/embed/9tJbunCrOmE" frameborder="0" allowfullscreen></iframe>


### Cobertura  de decision

Se basa en el porcentaje de resultados de decision que son ejecutados por las pruebas

Se trata de cubrir con casos de prueba cada arista del grafo de flujo de control al menos una vez.

**El objetivo de prueba es lograr la cobertura de un porcentaje especifico de todas las desiciones**


```
Cobertura de decision = 

   Numero de decisiones ejecutadas 
   
   ------------------------------- * 100%
   
   Numero total de decisiones

```

Lograr una cobertura de 100% de condicion al menos necesita los mismos casos de prueba que se requieren para una cobertura de 100% de sentencia


### Cobertura de de condicion
Se basa en el porcentaje  de todos los resultados individuales de condicion que afectan los resultados 

Se tienen en cuenta la complejidad de una condision que este constituida por varias condiciones individuales. Ejemplo  

`If ((a>2) Or (b<8))`

Se toma cada una de las condiciones individuales de la condicion y a partir de ellos se generan casos de prueba.



#### Cobertura de condicion simple

Para generar los casos de prueba cada condicion individual **debe tomar al menos una vez** los valores de verdadero y falso.

Ejemplo

```

If ((a>2) Or (b<8))

```

 a  | b | Resultado de la condicion  
------------- | -------------  | -------------
a = 6 => True | b = 9 => False | (a=6) OR (b = 9) => **True**
a = 1 => False | b = 2  => True| (a=1) OR (b = 2) => **True**

En este caso solo se esta tomando 1 vez cada valor y se esta evaluando la condicion.


####Cobertura de condicion multiple

Para generar los casos de prueba cada condicion individual debe tomar **TODOS** los valores de verdadero y falso.



Ejemplo

```

If ((a>2) Or (b<8))

```

 a  | b | Resultado de la condicion  
------------- | -------------  | -------------
a = 6 => True | b = 9 => False | (a=6) OR (b = 9) => **True**
a = 6 => True | b = 2 => True | (a=6) OR (b = 2) => **True**
a = 1 => False | b = 2  => True| (a=1) OR (b = 2) => **True**
a = 1 => False | b = 9  => False| (a=1) OR (b = 9) => **False**



En este caso solo se esta tomando Todos los posibles valores y se esta evaluando la condicion, lo que genera 4 casos de prueba no solo dos como en condicion simple.

En este tipo de prueba los casos de prueba crecen de manera exponencial, en la formula 2N [^math]

#### Minima Cobertura de condicion multiple


### Cobertura de camino

Se basa en el porcentaje de caminos del programa que han sido ejecutados por las pruebas, incluye todos los caminos dentro de un bucle, por lo que cada camino del bucle es un caso de prueba separado, lo que ademas genereraria una explocion de casos de prueba.

Esta es brinda una cobertura aun mas exhaustiva que la cobertura de sentencia y de condicion.


**El objetivo de prueba es lograr la cobertura de un porcentaje especifico de todos los caminos**


```
Cobertura de caminio = 

   Numero de caminos cubiertos
   
   ------------------------------- * 100%
   
   Numero total de caminos

```

## Tecnicas basadas en la experiencia - Pruebas intuitivas

Se basan en la intuicion y experiencia del probador, ya sea como usuario del sistema, o experiencias con un sistema similar en el pasado o conocimiento de que algun miembro del equipo puede generar defectos debido a su poca experiencia.

Lo que le permite tener la intucion de saber donde pueden estar los defectos, la experiencia de saber cuales y donde han sido detectados anteriormente los defectos y donde hay mas probabilidades por la complejidad del proyecto que existan mas defectos.

```Donde se han acumulado los errrores en el pasado? ```

``` Donde falla este software normalmente? ```

Son un complemento ideal para las pruebas sistematicas por lo que se deberia tratar como una tarea adicional en el proceso de pruebas. Tienen el beneficion que estos pueden detectar defectos q no se detectarian con las pruebas sistematicas.


Estaa incluyen **prediccion de errores** y **pruebas exploratorias**

**La predicionn de defectos** se basa en comprobar la lista de defectos, que han sido enumerados y documentados con anterioridad, por lo que se generan nuevos casos de prueba en base a esta lista con el fin de tratar de reproducir los defectos que estan en la lista. Un factor muy importante es que si se encuentra un nuevo defecto este debe ser añadido a la lista con el fin de ser tomado en cuenta en futuros proyectos 


**Las pruebas exploratorias** son apropiadas cuando la base de prueba es poco estructurada y cuando el tiempo de prueba es poco.
Su procedimiento es 

* Revisar partes del objecto de prueba
* Ejecutar un # reducido de casos de prueba
* Analisar los resultados 
* Repetir las acciones anteriores expandiendo los casos de prueba en base a lo aprendido en la iteracion anterior


> **Carta de pruebas**
> > Contiene los objetivos de las pruebas y los tiempos de ejecucion de las mismas

<iframe width="560" height="315" src="https://www.youtube.com/embed/RQRkRLYujWA" frameborder="0" allowfullscreen></iframe>


##Seleccion de las tecnicas de prueba

La seleccion de tecnicas de prueba dependen de varios factores

* Estado del la informacion del objeto de pruebas 
	* Tengo el codigo para realizar pruebas de caja blanca? 
	*  la documentacion esta completa para poder realizar pruebas de caja negra?
* Objectivos de la prueba predominantes
	* Se ha solicitado explicitamente un tipo de prueba (Funcionales, Stress, Automatizadas)
* Riesgos 	 
	* El sistema sera utilizado con una alta frecuencia
	* Hay estandares legales/ contracturales que me permitan realizar la prueba
* El proyecto
	* Tengo el tiempo necesario para realizar las pruebas
	* Que pasa si no tengo finalizado todo el juego de pruebas segun lo planeado
* Caracteristicas del objeto de pruebas
	* Esta el objeto de pruebas disponible
	* Esta el ambiente de pruebas listo
* Requisitos contracturales
	* Hay alguna norma que determine el objetivo especifico de las pruebas
	* Estan todos los documentos listos cuando se requirieron
* Mejores practicas
	* Que enfoques se han ejecutado en sistemas similares
	* Que experiencia se han obtenido de estas estructuras anteriormente
* Niveles de prueba
	* Que niveles de prueba seran ejecutados con las pruebas

Los diferentes miembros del equipo tienen enfoques distintos al momento de plantear el diseño de pruebas

El jefe de proyecto velara porque el sistema tenga la calidad requerida y ademas se cumplan con el tiempo y presupuesto del proyecto

El cliente velara por recibir un producto con la mas alta calidad y que ademas no se sobrepase ni el tiempo ni el presupuesto

El jefe de pruebas velara por ejecutar las pruebas necesarias para evaluar la calidad del sistema, que se tengan los recursos necesarios para ejecutar todas las tareas de prueba, ademas de evaluar y analizar la calidad alcanzada por el sistema. 	 	    	    	 