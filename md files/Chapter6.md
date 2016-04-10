#Capitulo 6  - Herramientas de prueba

## Tipos de Herramientas


Las  herramientas dan soporte a las actividades de prueba descritas en el Capitulo 1, tambien hay herramientas para cada nivel del proceso de prueba, por ejemploo herramientas para la ejecucion de prueba, generacion de datos, que permites la exploracion del objeto de prueba, en fin cualquier herramienta que ayude al proceso de prueba, ejemplo una hojo de calculo.

**Objetivos del uso de herramientas**

* Mejorar la eficiencia a travez de la automatizacion de tares repetitivas 
* Automatizar actividades que requiren mucho esfuerzo si se hicieran de manera manual
* Mejorar la fiabilidad de las pruebas



> **Test Framework - Marco de prueba**
> > Librerias de pruebas reutilizables y extendibles usadas para contruir herramientas de prueba
> > Tipo de diseño de automatizacion de pruebas
> > Proceso global de ejecucion de pruebas

### Clasificacion de herramientas de prueba

* Herramientas  unitarias (Single Tools) dan soporte a una sola tarea o actividad

* Paquete de herramientas (Test tools suite) cubren varas tareas e integran herramientas unitarias

* Herramientas intrusivas que interfieren en la ejecucion del objeto de prueba y pueden generar comportamientos diferentes a los posibles resultados obtenidos en el entorno real, ejemplo los depuradores que introducen breakpoints y alteran la ejecucion

* Herramientas que no afectan la ejecucion del objeto de prueba
* Se pueden clasificar bajo otros criterios
	*	Comerciales, gratuitas, codigo libre
	* Por la actividad que soportan
	* Herramientas desarrolladas de forma interna(In House), como Hojas de calculo, scripts de sql, bases de datos.
 

#### Herramientas para el soporte de la gestion de pruebas
* **Herramientas para gestion de pruebas**
	* Se encarga de la administracion de los casos de prueba
	* Permiten establecer metricas
	* Permiten la planificacion de recursos y tiempo para las pruebas 

*	 **Herramientas para gestion de requerimientos**
	*	 Repilacion de requerimientos
	*	 Asignacion de prioridades a los requerimientos
	*	 Establece la relacion entre caso de prueba y requerimientos
	*	 Identificacion de requisitos inconsistentes

	
	
*	 **Herramientas para gestion de incidentes / defectos**
	*	 Registro seguimiento de incidencias, defectos, anomalias
	*	 Almacen de solicitud de cambio
	*	 Permiten la priorizacion de los defectos
	*	 Permiten la evalucacion del progreso de los defectos
	*	 Determinal el ciclo de vida de los defectos
	 
*	 **Herramientas para gestion de la configuracion**	*	 Seguimiento de las distintas versiones de los objetos de prueba
	*	 Gestion del versionamiento de los productos de soporte de prueba, configuraciones y otras herramientas
	*	 Administracion del codigo fuente y del codigo del objeto

	
####  Herramientas para el soporte de pruebas estaticas
* **Herramientas para el analisis estatico**
	*	Cumpliento de estandares de programacion
	* Analisis de la estructura del codigo
	* Analisis del flujo de datos
	* Analisis de metricas de complejidad del codigo


* **Herramientas de revision**
	* Apoyo a la revision con listas de comprobacion, guias y cometarios de revision
	* Documentacion de los resultados de la revision
	* Evaluacion de los resultados de la revision
	* Apoya la trazabilidad entre documentos y codigo fuente

* **Herramientas de modelado**
	* Analisis de modelos de datos
	* Analisis de documentos de especificacion/modelo de objetos y diagramas de estados
	* Generar casos de prueba a base de dagrama


####  Herramientas para el soporte de la especificacion de pruebas 

* **Herramientas de diseño de prueba**
* **Herramientas de preparacion de datos de prueba**
* **Generadores de datos asociados a la base de datos**
* **Generadores de datos de prueba en base en el codigo**
* **Generadores de datos de prueba asociados a la interfaz**
* **Generadores de datos de prueba en basados en la especificacion**
	
####  Herramientas para el soporte de la ejecucion y registro de prueba
Apoyan a la ejecucion de pruebas en todos los nivels de prueba.

* Entrega de datos
* Registro del comportamiento de la salida


Ejemplos de herramientas

* **Robots de prueba**
	* Compara los resultados obtenidos contra los esperados
	* Permiten la repeticion automatica de la secuencia de prueba utilizando el script de prueba
	* Son apropiadas para pruebas de regresio y pruebas exploratorias
* **Depurador**
	* Herramientas para la deteccion de errores en el codigo mediante la comprobacion de sentencias unitarias y condidciones

* **Comprobadores de prueba**
	*   Comparan los resultados obtenidos con los esperados

* **Arnes de prueba o marco de trabajo para pruebas unitarias**
	* Simulan el entorno del objeto(Mock objects)
* **Controladores de prueba (Test Drivers)**
	* Permite acceder al objeto de prueba cuando las interfaces no han sido creadas 
* **Stubs**
	* Simulan la funcionalidad de un componente **INVOCADO**  
* **Herramientas de medicion de cobertura**
	* Miden el porcentaje de un tipo de estructura de codigo especificada que ha sido ejecutada por un conjunto de pruebas
*** Herramientas de prueba de seguridad**
	* Evaluan las caracteristicas de seguridad del software

####  Herramientas para el soporte de monitoreo y rendimiento
* **Herramientas de analisis dinamico**
	*  	Detectan defectos cuando el software esta en ejecucion ejemplo fugas de memoria, asignacion de punteros, etc.
* **Herramientas de pruebas de rendimiento/carga/estres**
	* Permiten medir el sistema bajo condiciones de cantidad de usuarios o transacciones durante un periodo determinado
* **Herramientas de monitoreo**
	*   Analiza de forma continua los recursos del sistema y advierte de posbiles problemas del servicio


####  Herramientas para necesidades especificas de  prueba
* **Evalucion de la calidad de datos**
	* Se enfocan en los datos, permiten revisar y verificar la conversion de los datos en base  a las reglas de migracion

	
	
	
##Uso efectivo de herramientas de prueba

El uso de herramientas implica costes y esfuerzos, como por ejemplo instalacion de la herramienta, adaptando la herramienta en la organizacion, el tiempo de transicion y esfuerzo en el uso de la herramienta. 

```Las ventajas del suo de herramientas deben superar los costes. ```

**Beneficios**

* Reduccion del trabajo repetitivo 
* Iteracion de actividades identicas
* Mayor consistencia 
* Facilidad de acceso a la informacion
* Mejor informacion a la toma de decisiones

**Riesgos** 
* La funcionalidad de la herramienta no cumple las expectativas
* La usabilidad de la herramienta no cumple las expectativas
* Se han subestimado el tiempo y esfuerzo necesarios para lograr beneficios
* Otros requisitos de calidad no han sido alcanzado
* Se han subestimado los beneficios
* Los costes se han subestimado
* Excesiva dependencia de la herramienta
* Desatencion del contol de versiones de los activos de prueba enla herramienta
* Riesgo que el fabrican suspenda el desarrollo de la herramienta
* Riesgo de pobre soporte, actualizacion y correccion de defectos
* Expectativa que la herramienta resolvera todos los problemas de prueba


``` Una herramienta nunca reemplazara un proceso inexiste o compensara un procediento mal diseñado ``` 



##Introduccion de herramientas de prueba en una organizacion

``` Es un proceso exigente que debe ser controlado y gestionado ```

**Pasos para la introduccion de herramientas**

* Evalucacion
	* Identificacion de las debilidades del proceso de prueba donde las herramientas 
* Definicion de requisitos
	* Definicion de las necesidades respecto a la herramienta

* Evaluacion
	* Examinar una lista corta de herramientas, comprobando la conformidad con la funcionalidad requerida

* Prueba de concepto
	* Probar y evaluar las herramientas bajo condiciones que se necesitan
* Evaluacion del fabricante
	* Enumerar los posibles candidatos, caracteristicas, revisar el resultado y tomar la desicion de cual herramienta usar.
* El uso de la herramienta
	* Identificar los requisitos internos para la preparacion
* Evaluacion de formacion - Training
	* Validar las necesidades del equipo y realizar entrenamientos
* Relacion Coste-Beneficio




#### Ventajas de un proyecto piloto
* Llegar a conocer los puntos fuertes y debilidades de la herramienta
* Establecimiento de interfaces con otras herramientas
* Definir informes
* Evaluar si se cumple conlos beneficios esperados
* Estimar el costo

```
No se debe introducir una herramienta sin el desarrollo de un piloto.
De lo contrario esperar/contar con problemas de aceptacion
```
#### Factores de exito en el despliegue de software
* Introducion paso a paso en la totalidad de la organizacion
* Hacer obligatorio el uso de la herramienta
* Son necesarias guias de usuario
* Los usuarios deben tener acceso a la formacion adecuada
* La experiencia adquirida debe estar disponible para todos los usuarios
* La herramienta debe ser sujeta de seguimiento para mejorar su aceptacion
* Reunir/recoger las lecciones aprendidas de todos los proyectos



















