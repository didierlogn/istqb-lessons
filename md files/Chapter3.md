#Capitulo 3

## Tecnicas estaticas y procesos de prueba
Estas comprenden tecnicas en las cuales no se ejecuta el objeto de prueba
Las pruebas estaticas son:

* **Revisiones**
* **Analisis Estatico**

Estan detectan la causa de los fallos -> **Defectos**, Ademas pueden encontrar defectos que las pruebas dinamicas no podrian, los documentos de calidad producen productos de calidad.

### Objetivos de la revision
* Se utilizan para corroborar la correcta transicion entre las distintas fases del modelo V.
* Detectan errores de forma temprana
* Ejemplo de defectos
	* 	Defectos en las especificaciones
	*  Defectos en el diseño o arquitectura
	*  Defecto en la especificaciones de interfaces
	*  Mala Mantenibilidad del codigo
	*  Desviaciones con respecto a los estandares
	
**Ventajas**

* Permite tener costos mas bajos dado que encuentran errores en etapas tempranas
* Los documentos de calidad mejoran el desarrollo
* Mejoran la comunicacion y el intercambio de conocimiento del sistema entre los miembros del sistema

**Desventajas**
* Se pueden dar enfrentamientos con el autor
* Los expertos necesitan adquirir el conocimiento requerido para participar en la revision
* Es necesario impertir tiempo y por ende dinero 
* El Moderador y los participantes influyen en la calidad de la revision

## Proceso de revisiones

### Actividades de una revision formal


Actividad  | Tareas
:---------- | -------------
**Planificar** | Definir los criterios de revision
           | Selecionar el personal
           | Asignar funciones y tareas
           | Definir el calendario
**Definicion de criterios de entrada y salida** | Seleccionar que partes seran revisadas (dependiendo de la importancia y complejidad)
**Inicio/Lansamiento/Kickoff** | Se reparten los documentos
           | Se explican los objetivos de la revision
**Comprobacion de criterios de entrada** | (Esto para revisiones formales)
**Preparacion individual** | Se revisan los documentos por parte de cada miembro del equipo revisor           
**Identificar posibles defectos, preguntas, comentarios** |  Los revisores detectan los defectos
**Reunion de revision** | Los revisores prsentan sus resultados 
           | Debatir, registrar los resultados
            | Identificar defectos  y presentar recomendaciones
**Examen/Evaluacion/Registro** | Reuniones o comunicaciones electronicas del grupo
**Recontruccion / Adaptacion** | El autor corrige los errores detectados y mantiene actualizados el estado del defecto
**Seguimiento** | Comprobacion de que los defectos han sido tratados
 | Se recopilan metricas
  | Se decide realizar otra revision si fuera necesario
**Comprobacion de criterios de salida**

### Roles y responsabilidades

* **Jefe**              
	* Incia la revision
	* Determina si los objetivos se han cumplido
	* Asigna el tiempo en el calendario del proyecto 	
* **Moderador**              
	*	Dirige la reunion
	* Es el mediador 
	* Concluye resultados
	* Planifica la revision, su ejecucion y el seguimiento

* **Autor**              
	* Redactor del objecto de revision
	* Expone su trabajo en la revision

* **Revisor**              	
	* Detectan  defectos, desviaciones  o problemas
	* Presentan consejos
	* Representan los distintos perspectivas y roles de la revision
	* Tienen el conocimiento tecnico o del negocio para participar	 
* **Escriba**              
	* Documenta todos los puntos durante la revision

	
#### Tipos de Revisiones

Inspeccion | Revision Guiada | Revision Tecnica | Informal
---------- | --------------- | ---------------- | --------
Se realiza con listas de comprobacion y metricas | Revision guidados de documentos, diseño de interfaz o modelos de bases de datos | Uso  listas de comprobacion |  Es la revision mas simple |  
Se necesita un moderador | La reunion es dirigida por el autor, no es necesario el moderador |  Se necesita un moderador entrenado | 
Es necesario criterios de entrada espeficados previamente |  |  | 
Es un proceso formal | Son secciones abiertas |  | 
Preparacion previa a la reunion | No necesita preparacion previa  | Preparacion previa a la reunion | Iniciada por un compañero de trabajo
Se tiene una lista de hayazgos |  | Se tiene una lista de hayazgos | Listas de accion
Se necesitan roles definidos |  |  | 
Actividades intencivas de preparacion y seguimiento| Son secciones con notificaciones con poco antelacion |  |
Es un metodo estructurado |  |  | No requiere protocolo, facil de ejecutar y rentable
Se realiza como un examen entre pares | Participacion grupal de parees, son escenarios, ejecucion simulada  | Se realiza como un examen entre pares | 
**Objetivo principal:** Identificar defectos | **Objetivo principal:** Identificar defectos, aprender y entender el objeto de pruebas | **Objetivo principal:** Toma de decision, evaluar alternativas, detectar defectos, resolver problemas tecnicos, comprobar estandares |  

#### Factores de exito de revisiones

* Hay un enfasis de aprendizaje y mejoras de proceso
* Debe haber un ambiente de confianza
* Deben ser enfocadas al logro de objetivos
* El autor debe sr motivado de forma positiva, nunca con el motivo de criticar su trabajo
* Uso de herramientas y plantillas
* Uso de listas de comprobacion (checklist)
* Presupuesto correcto

## Analisis estatico con herramientas
> **Analisis Estatico**
> ---
> > Consiste en analizar un objeto de prueba (codigo fuente, script, requerimiento) sin ejecutar el sistema.
---

Durante el analisis estatico se comprueban los siguientes aspectos

* Reglas y estandares de programacion
* Diseño de programa - Analisis del flujo de control
* Uso de datos - Analisis del flujo de datos
* Complejidad de la estructura del programa

El analisis estatico usando herramientas se realiza con un menor esfuerzo que con las revisiones, lo que permite detectar logica ausente o erronea, construcciones muy complicadas, vulnerables a fallos de seguridad, por lo que se ejecuta de antes que las inspecciones.
Ademas permite comprobar la mantenibilidad del codigo o diseño o inclusive diferencias con el diseño

### Herramientas 
#### Compilador
* Dectecta errores de sintaxis en el codigo
* Comprueba consistencia entre los tipo de datos de las variables
* Detecta variables no declaradas o codigo inaccesible

#### Analizador
* Convenciones y Estandares
* Metricas de complejidad
* Acoplamiento de objectos

### Analisis de flujo de control
Permite detectar cdefectos causados por un desarrollo incorrecto(ramas muertas o codigo muerto)
Se utiliza un grafo dirigido donde

* Los nodos representan sentencias o grupos de sentencias
* Las aristas representan condicionales o blucles

Esto permite tener una visualizacion mas clara de como esta la estructura del programa.

#### Como hacer el grafico de control flujo a partir del codigo
Este es un ejemplo de como realizar el grafico de control de flujo a partir del codigo. [Link](https://drive.google.com/file/d/0B0r0vOZR85sfemxUTmxUZUExQkE/view?usp=sharing).

**Codigo**

![Codigo](https://cldup.com/TuSxSK7hRi.thumb.png)

**Identificar sentencias y condicionales**

![Sentencias y condicionales ](https://cldup.com/WWuQISUbUZ.thumb.png)

**Diagrama de flujo**

![Diagrama de flujo](https://cldup.com/CtjOveo2u--3000x3000.png)

**Diagrama de control de flujo**

![Diagrama de control de flujo](https://cldup.com/0m96b-szyU-2000x2000.png)

Tomado de [http://cursos.tecmilenio.edu.mx/cursos/at8q3ozr5p/prof/sa/sa09002/anexos/grafo_java](http://cursos.tecmilenio.edu.mx/cursos/at8q3ozr5p/prof/sa/sa09002/anexos/grafo_java)



### Analisis de flujo de datos
Este permite detectar errores en el flujo de datos, es decir valida los datos q puede tener una variable durante todo el ciclo del programa con el fin de encontrar algun error durante el proceso


### Metricas
Tratan distintos aspectos del programa: Tamaño de programa (Total de lineas de codigo), Estructuras de control (numero cliclomatico), Estructuras de control de datos(metrca de Halstead)

**Numero ciclomatico** mide la complejidad estatica de un programa utilizando el grafo de control de flujo.

> v(G) = e - n +2p
---




































