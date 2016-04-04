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


## Tecnicas de caja Blanca o basadas en a estructura - Prueba basada en el flujo de control

## Tecnicas basadas en la experiencia

##Seleccion de las tecnicas de prueba
