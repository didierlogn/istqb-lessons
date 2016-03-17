## Capitulo 1

### Terminos
Bug  |  Defecto  |  Error  |  Fallo  |  Calidad  |  Riesgo
---  |  -------  |  -----  |  -----  |  -------  |  ------

---

```	
Error: Accion Humana que produce un resultado incorrecto ( IEEE 610 )
========================================
```
```
Defecto: Componente que puede causar el fallo en el desempeño de las funciones requeridas
========================================
```
```	
Fallo: Manifestacion fisica o funcional de un defecto
========================================
```
---
### Papel del proceso de pruebas
* Mejora la calidad del producto de Software
* Reduce el riesgo de detectar errores
* Permite satisfacer compromisos
	* Dado que puede ser requisito obligatorio por parte del cliente

> *La deteccion de defectos en etapas tempranas permite minimizar el costo de los mismos* 
---

---
```
Software: Programa de ordenador, procedimientos, documentacion y datos de un sistema basado en un ordenador. (IEEE 610)
```
```
Calidad de software: La totalidad de la funcionalidad y prestaciones de un producto software que contribuyen con su capacidad de satiscacer necesidades explicitas o implicitas.(ISO/IEC 9126)
```
```
Calidad: Grado en el cual un componente, sisetma o porceso satisface requisitos especificados o necesidades y expectativas del usuario. (IEEE Std 610)
```

---
### Tipos de pruebas ( *ISO 9126* )
* **Funcionales**
	* Funcionalidad 	
* **No Funcionales**
	* Fiabilidad
	* Usabilidad
	* Eficiencia
	* Mantenibilidad
	* Portabilidad 	

---

La norma **ISO 2501** añade dos atributos mas:

* Compatibilidad
* Seguridad
	* Integridad
	* Disponibilidad
	* Accesibilidad

---
## Tipos de Aseguramiento de la calidad

### QA Constructivo - Gestion de calidad
> Tiene como objetivo prevenir defectos

**Consigna del QA constructivo**

* Los defectos evitados no requieren ser reparados
* Los defectos introducidos en el pasado no deben ser repetidos
* Prevenir defectos


	* **Organizacion**
		* Guias 
		* Estandares
		* Listas de comprobación
		* Reglas de procesos y normas
		* Requisitos legales

	* **Técnico**
		* Metodos 
		* Herramientas
		* Lenguages
		* Listas / plantillas
		* Entornos de Desarrollo Integrado (IDE)


### QA Analitico - Verificacion y pruebas
> Tiene como objectivo detectar defectos

**Consigna del QA analitco**

* Los defectos deben ser detectados tan pronto como sea posible

#### Tipos de QA analitico
* **Estatico**: Son llevadas a cabo sin la ejecucion del programa
	* Revisiones / revisiones guidadas
	* Analisis del flujo de control
	* Analisis del fluoj de datos
	* Metricas de compilador / analizador 		

* **Dinamico**: Se necesita la ejecucion del programa.
	* **Caja Negra - Pruebas de Especificación**
		* Particiones equivalencia
		* Analisis de valores limite
		* Tabla de decision
		* Pruebas de transicion de estado
		* Analisis de caso de uso 
		 	
	* **Caja Blanca - Pruebas estructurales - Pruebas basadas en el flujo de control**
	
		* Cobertura de sentencia
		* Cobertura de Rama
		* Cobertura de condicion
		* Cobertura de camino

---

## Objectivos de las pruebas

* Generar confianza con respecto a la calidad
* Generar informacion para la toma de decisiones
* Detectar defectos - Adquirir conocimientos sobre los defectos del objeto de prueba
* Confirmacion de la funcionalidad
* Prevencion de Defectos

---
### Criterios de salida
* No encontrar mas defectos
* Pruebas basadas en riesgos
* Pruebas basadas en tiempo y presupuesto

### Casos de prueba
Un buen caso de prueba debe contener las siguientes secciones(**Estandar IEEE 829**)

* Precondiciones
* Valores de entrada
* Resultados Esperados
* Poscondiciones
* Un Identificador
* Dependencias con otros test cases
* Referencia al requisito probado
* Prioridad
* Forma de ejecutar la prueba, pasos para ejecutarla

### Base de Pruebas
Conjunto de documentos que definen los requisitos del objeto de prueba


## Actividades de Proceso de pruebas
```
Cada fase del proceso de pruebas es concurrente con las fases del proceso de desarrollo
```

---
* Planeacion y control
* Seleccion de condiciones de prueba
* Diseño y ejecucion de pruebas
* Comprobacion de resultados
* Generacion de informes
* Finalizacion y actividades de cierre

---
* Planeacion y control 
* Analisis y diseño de pruebas
* Implementacion y ejecucion de pruebas
* Evaluacion de resultados y genracion de informes - Evaluacion de criterios de salida e informes
* Actividades de cierre de pruebas

---
### Planeacion y control
#### Planeacion
Define los objectivos de las pruebas y la especificacion de las actividades de prueba

**Objetivos**

* Determinar el alcance
* Identificar los objectivos de las pruebas y criterios de salida
* Determinar el enfoque de la prueba
* Implementar el metodo de prueba / Estrategia de pruebas 
* Manejar los recursos necesarios para las pruebas. personal, entorno de prueba, presupuestos

#### Control
Es una actividad constante que verifica el avance real con respecto a lo planeado, informa sobre desviaciones e implica la adopcion de medidas para cumplir los objetivos planeados.
Dado al control se puede cambiar el **plan maestro de pruebas ( Master Test Plan - Test Plan)** para adecuarlo a las necesidades

> **Plan maestro de pruebas - Master Test Plan - Test Plan**
>>Documento que define los alcances, el enfoque, los recursos, el calendario de actividades, los items que se van a probar y los que no se van a probar 

> **Estrategia de pruebas - Test Strategy**
> > Escripcion a alto nivel de los **niveles de prueba** y las pruebas asociadas a ellos

> **Enfoque de Pruebas - Test approach**
> >Es la implementacion de de la estrategia de pruebas para un proyecto en especifico. Contiene las decisiones tomadas para cada objectivo, analisis del riesgo, puntos de inicio del proceso de prueba, tecnicas del diseño de prueba, criterios de salida y tipo de prueba a ejecutar

> **Criterios de salida**
> > Conjunto de condiciones definidas que permiten establecer que una tarea en especifico esta concluida

### Analisis y diseño de pruebas
Tiene como finalidad convertir los objectivos de las pruebas en casos de prueba

**Tareas principales**

* Analizar la base de prueba
* Analizar la testeabilidad 
* Identificar y priorizar las condiciones de prueba
* Disenar y priorizar casos de prueba y condiciones de prueba a alto nivel
* Identificar los datos de prueba para los casos de prueba - (test data)
* Diseñar la configuracion del entorno de pruebas (ambiente de pruebas - cama de pruebas (test-bed)) - Infraestructura, herramientas de prueba
* Crear la trazabiidad entre los casos de prueba y la base de prueba (requerimientos) 

> **Datos de prueba**
> > Datos que necesita una prueba para ser ejecutada
> 
> **Datos de entrada**
> >Parametro de entrada que toma una componente para ejecutarse
> 
> **Cobertura de pruebas**
> > Porcentaje de codigo probado por el set de pruebas
> 
> **Oraculo de pruebas - Test oracle**
> > Fuente que permite comprarar resultados anteriores con los obtenidos durante las pruebas

---
> # - ---------Voy por aca --------

---
## Terminos de desarrollo de software
* Depuracion
	* Proceso de encontrar,analizar y solucionar el defecto  
* Requisito
	* Condicion o capacidad necesario sistema cumpla con lo establecido
* Revision
	* Evaluacion de un producto o estado de un proyecto para detectar diferencias con los resultados planificados.

# Depuracion
La depuracion consiste en:

* Encontrar la raiz del defecto
* Corregir el defecto 	

Las pruebas y depuracion tienen el siguiente flujo:

```
Prueba -> Depuracion[Encontrar la causa raiz - Corregir defecto] -> Re Test 
```

---
## Principios del proceso de prueba

* **El proceso de pruebas demuestra la presencia de defectos**
	*  No detecta la ausencia de los mismos
* **Las pruebas exaustivas no existen**
	* Solo en casos triviales, por lo que se debe realizar un analisis de riesgo y prioridades
	* Genera una explocion de casos de prueba
	* Por lo que se toma una **Prueba de Muestra(Sample Test)**,que es un subconjunto de todos los posibles valores de entrada
* **Pruebas Tempranas**
	* Cuanto mas rapido se encuentre un defecto menor es el costo de correccion. 
	* La preparacion de la prueba tambien consume tiempo
* **Agrupacion de defectos** 
	*	 Donde se encontro un defecto es muy probable que si se sigue probando se contraran mas defectos
* **Paradoja del Pesticida**
	* La repeticon de las mismas pruebas con los mismos valores de entrada no van a encontrar mas errores
	* Las pruebas deben ser evaluadas constantemente
* **Las pruebas dependen del contexto** 
	* Todo depende de lo que se vaya a probar, no es lo mismo probar un software bancario a probar un sitio web
* **La falasia de aunsencia de errores**
	* El proceso de prueba encontrara los fallos mas importantes del objeto de prueba, pero talvez no los encuentre todos	 















