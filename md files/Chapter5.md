# Capitulo 5 - Gestion de pruebas

## Organizacion de pruebas

```
La gestion de pruebas debe verse como 
la gestion del proyecto de prueba
```

```
El proceso de pruebas es una actividad que 
cubre por completo el proceso de desarrollo 
de software
```


Actividad | Resultado del trabajo
--- | ---
Concepcion de pruebas | Plan de pruebas estatico
Planificacion de pruebas | Plan de pruebas dinamico
Control de pruebas | Informe de estao, accion de control
Pruebas de aceptacion | Entrega del producto de software

---

```
Los equipos de prueba deberian ser independientes

Ventajas 
    - Imparcialidad
    - Se pueden cuestionar hechos respecto de la base de pruebas
    
Desventajas
    - Mayor esfuerzo en la comunicacion
    - Los desarrolladores pierden el sentido de la responsabilidad

    
Conformacion de equipos
    - Los probadores prueban sus propios programas
    - Los probadores son miembros del equipo de desarrollo
    - Los probadores son miembros del equipo de proyecto o estructura de la organizacion 
    - Especialistas para tareas especificas
    - Equipos de prueba externos
```

### Perfiles del personal de pruebas

#### Jefe de pruebas o director de preubas (Test Manager)

* Planifica, realiza seguimiento y control del proyecto de prueba 
* Competencias necesarias
	* Gestion de pruebas y calidad de software
	* Planificacion y control de pruebas
	* Experiencia como jefe de proyecto
	* Habilidades de gestor

	
**Tareas del lider de prueba**	

* **Planificacion de pruebas**
	* Se realiza el plan maestro de pruebas
	* Se definen hitos, presupuesto y prioridades
	* Los riesgos
	* Se seleccionan las herramientas con respecto a la automatizacion
	* Si hay atrasos la planificacion de las pruebas debe ser modificada y adaptada
	* Se definen los recursos, personal y equipo
	* Se establecen metricas para el control de actividades de prueba
	* Se debe tener en cuenta pruebas anteriores para ser tomadas como base para la planificacion
	
	
* **Planificacion del ciclo de prueba**
	* El plan maestro de prueba es adaptado para describir cada una de los ciclos de prueba

* **Especificacion de pruebas**
	* El objetivo primordial es encontrar la mayor cantidad de defectos con el menor esfuerzo 
	
* **Estrategia de prueba**
* **Ejecucion, Medicion y control de pruebas**
	* Compraracion de resultados esperados contra resultados obtenidos
	* Todas las desviaciones deben ser informadas y tenidas en cuenta para tomar decisiones, ajustar las fechas de entrega, ajustar la cantidad de recursos
* **Introduccion de un sistema de gestion de incidencias adecuado**
* **Introduccion de un sistema de gestion de la configuracion **
* **Generacion de informes de resultado y progreso **
	* El uso de herramientas y plantillas aumentan la calidad y reducen la carga de trabajo
	* La gestion de prueba incluye la aceptacion de resultados, por lo que el producto debe cumplir con los requisitos y espeficaciones definidos. El jefe de proyecto y el jefe de pruebas deciden la aceptacion del objeto de prueba
* **Redaccion del plan de pruebas**
	
	
``` 
Tareas de un jefe de pruebas: Iniciacion, control y suspencion de 
pruebas y ciclos de prueba	
```
	

#### Diseñador de pruebas
* Disena casos de prueba y **establece el orden en el cual se ejecutaran los casos de prueba**
* Competencias necesarias
	* Conocimiento de desarrollo y de pruebas
	* Conocimiento de ingenieria de software
	* Conocimiento respecto a las especificaciones tecnicas
	* Conocimiento de requisito funcionales

#### Ingeniero en automatizacion de pruebas
* Evalua las posibilidades de la automatizacion de las pruebas y las implementa
* Competencias necesarias
	* Experiencia como probador
	* Conocimiento tecnico en el ambito de diseño y automatizacion de pruebas
	* Conocimientos en programacion 
	* Amplios conocimientos en el uso de las herramientas utilizadas

#### Administrador de prueba
* Prepara y opera el entorno de pruebas, es el responsable del cumplimiento de los requisitos del sistema de prueba
* Competencias necesarias
	* Administracion de sistemas
	* Conocimiento de herramientas de desarrollo y pruebas
	* Sistemas de bases de datos
	* Instalacion y operacion del software del sistema


#### Probador (Tester)
* Ejecuta las pruebas en base a las especificacion de los casos de prueba
* Competencias necesarias
	* Conocimiento basico de software
	* Conocimiento basico de pruebas
	* Operacion y uso de las herramientas de prueba
	* Experiencia en la ejecucion de pruebas
	* Conocimiento respecto a los objetos de pruebas

	
**Tareas del probador**

* **Asiste en la implementacion de la planificacion de actividades de prueba**
	* Revisa y comprueba planes de prueba
	* Analiza  bases de prueba

* **Desarrolla los diseños de los casos de prueba y ejecucion de prueba**
	* Desarrolla especificaciones de prueba
	* Formula y selecciona casos de prueba
	* Formula resultados esperados
	* Prepara, configura y administra el entorno de prueba junto con el administrador de sistema
* **Revisa casos de prueba de otros probadores**
* **Asiste en la implementacion de la automatizacion de pruebas**
* **Ejecucion de casos de prueba**
	* Ejecuta pruebas y registra resultados
	* Evalua los resultados de las pruebas

#### Experto tecnico
* Asiste al equipo de pruebas
* Competencias necesarias
	*	Administracion y Diseño de bases de datos 
	* Experto en Interfaz de usuario
	* Experto en redes
	* Exporto en seguridad

---
	
```
Competencias No tecnicas (Soft Skills) 

    - Instinto politico y diplomatico
    - Disposicion a preguntar sobre hechos aparentemente obvios
    - Persistencia, fuerte personalidad
    - Meticulosidad y creatividad
    - Capacidad para tratar situaciones complejas
    - Capacidad de aprender rapidamente

```


---
## Planificacion y estimacion del proceso de prueba

```La planificacion de las pruebas es planificacion de proyectos ```

```La planificacion de las pruebas es parte importante del aseguramiento de la calidad ```

Todas las tareas y actividades deben ser planificadas con antelacion, se deben asignar recursos(personal, herramientas, presupuesto, ambientes), se debe contar con un plan maestro de pruebas, se debe definir el nivel de calidad.

Esta planificacion es continua y debe ser controlada de forma constante, permitiendo asi hacer ajustes al plan maestro de pruebas para mitigar los riegos produciodos por los cambios.

Se debe contar con un **Plan de aseguramiento de calidad**, el cual debe tener:

* Organizacion del proyecto
* Documentos que cubren el ciclo de vida del desarrollo
* Estandares, metodos y convenciones para el desarrollo
* Revisiones y auditorias 
* Proceso de prueba
* Documentacion de errores y acciones correctivas



###Plan maestro de prueba - Master Test Plan
Es el primer paso en la planificacion de pruebas, cubre todas las fases del proceso de prueba, se fijan reglas de acuerdo a objetivos de prueba, recursos, actividades e hitos.

#### Estructura del Plan Maestro de Prueba - IEEE 829

1. Introduccion
2. Suposiciones
3. Elementos de prueba
4. Caracteristicas/prestaciones sujetas a pruebas
5. Caracteristicas/prestaciones **NO** sujetas a pruebas
6. Enfoque
7. Criterios de paso/fallo
8. Criterios de suspencion/renudacion
9. Entregables de prueba
10. Tareas de pruebas
11. Necesidades relativas al entorno
12. Responsabilidades
13. Personal y formacon 
14. Calendario
15. Riesgos y contingencias
16. Aprobacion


Actividades a realizar durante la planificacion  y estimacion del proceso de prueb

- Estrategia de prueba - Test Strategy
- Planificacion de recursos
- Soporte de herramientas

### Estrategia de prueba - Test Strategy
- Describe los niveles de prueba a desarrollar 
- Determina los criterios de entrada y salida, si como las metricas para evaluar estos criterios
- Evaluacion del riesgo, con el fin de enfocarse en las areas con mayor riesgo

#### Criterios de entrada

Definen cuando comenzar a probar. Ejemplos de criterios de entrada

- Inicio de un nivel de prueba
- Cuando un conjunto de pruebas estan listas para la ejecucion
- Entorno de prueba disponible
- Herramientas de prueba listas
- Disponibilidad de codigo
- Disponibilidad de recursos humanos
- Tester preparados 

#### Criterios de salida

Indican la finalizacion de una fase de prueba. Ejemplos:

- % Cobertura de codigo
- % Cobertura de riesgo 
- Razones de tiempo, costos o calidad
- Tasa de deteccion de errores


#### Enfoques de prueba

El enfoque de pruebas es la implementacion de la estrategia de pruebas para un proyecto en especifico.

-  **Enfoque preventivo:** Las pruebas son diseñadas tan pronto como sea posible
-  **Enfoque Reactivo:** Primero el desarrollo y luego el diseño de las pruebas
-  **Enfoque analisto:** Se basa en el analisis previo a las pruebas, ejemplo evaluando el riesgo 
-  **Enfoque heuristico:** Son pruebas reactivas, ejemplo pruebas exploratorias.

### Planificacion de recursos
- Objetivo principal es estimar el esfuerzo de los miembros del equipo(Tiempo, tareas, herramientas)
- Las estimacione forman parte del plan maestro de prueba dinamico
- Por medio del calendario se gestionan la ejecucion de pruebas.


### Estimacion de pruebas

Factores para realizar la estimacion

- Caracteristicas del producto
- Calidad de la base de pruebas
- Requisitos de fiabilidad  y seguridad
- Complejidad del desarrollo
- Estabilidad de la organizacion, madurez de proceso utilizado
- Personal involucrado

#### Estimacion experta

**Metodo**

1. Identificar todas las tareas
2. Obtener las estimaciones por parte de los responsables
3. Sumar todas las estimaciones
4. Incluir amortiguadores como colchon ante eventualidades


**Ventajas**

1. Las actividades estan relacionadas con la planeacion del proyecto
2. A medida que avanza el proyecto, las estimaciones se pueden modificar 
3. Los miembros del equipo son los que en grupos pueden determinar las estimaciones


**Desventajas**

1. Proceso largo y caro
2. No se estima los tiempos correctamente y por lo general se estima a la baja
3. Los errores en cuanto a la planeacion son heredados

#### Estimacion basada en analogias
**Metodo**

1. Clasificar las tareas de prueba
2. Buscar un proyecto **anterior** que tenga una tarea similar
3. Utilizar el esfuerzo real de ella como base de estimacion 
4. Usar metricas(lineas de codigo, modulos,etc) para la estimacion total
5. Incluir amortiguadores para considerar las correciones


**Ventajas**

1. Simple y efectivo
2. Se logran valores muy precisos en la estimacion 

**Desventajas**

1. Se requiere personal con experiencia
2. En ocaciones se debate la validez de la estimacion 
3. Los proyectos con que se compara no son iguales.

#### Estimacion basada en porcentajes
**Metodo**
1. El esfuerzo de las tareas de prueba se estima con un porcentaje de la totalidad de las actividades del proyecto

``` 
La estimacion basada en porcentajes no tiene en cuenta el esfuerzo de 
las pruebas de regresion, que pueden ser una parte sustancial de las 
pruebas de mantenimiento y asociadas al cambio
```

**Ventajas**

1. Es muy simple
2. No requiere mucha informacion 

**Desventajas**

1. No es precisa
2. No se tiene claro el tiempo necesario por lo que genera debates dificiles
3. Los porcentajes pueden variar de proyecto en proyecto


---
## Seguimiento y control del estado de pruebas
El seguimiento debe ser basado en consideraciones medibles

- **Metricas a base de errores:** Tasa de deteccion de errores, defectos, resultados de repeticion de pruebas
- **Metricas en base a casos de prueba:** cobertura de los casos de prueba, cobertura de codigo, cobertura de riesgo
- **Metricas en base a costos:** Costo de deteccion de errores, costo de pruebas de regression, costo de recursos externos


```
Los resultados deben ser informados de manera regular a los miembros del 
equipo
```

### Informacion de prueba
Toda la informacion de las actividades de prueba se consigna en los efectos de informacion de prueba (Test Reporting)

#### Informe de estado de pruebas (IEEE-829)
- Objecto(s) de prueba
- Nivel de prueba, ciclo de prueba, periodo de informe
- Avance de las pruebas, basadas en las metricas
- Recursos utilizados / Presupuesto consumido
- Hitos alcanzados
- Informe de defectos
- Evaluacion de riesgo
- Pronostico: Actividades planificadas para el proximo periodo de informe
- Evaluacion del estado general

La frecuencia de los informes dependera de las fases del proyecto, al inicio puede ser cada 15 dias / mes, sin embargo en las fases criticas tiene que ser diaria / semanal

Ademas al finalizar todas las pruebas se debe entregar el informe final 

```
Evaluacion de los informes - Como evaluar el estado general 

- La evolucion es apropiada?
- La ejecucion de pruebas es eficaz y eficientes? 
- Las actividades estan alineadas con los objetivos de prueba?
- Estan siendo alcanzados los objetivos de pruebas?
- Cual es el estado de confianza con respecto al producto 
en el estado actual progreso/evolucion/desarrollo?
```

###Control de pruebas
El control de pruebas es una tarea de gestion, por lo tanto es responsabilidad del jefe de prueba


Se deben tomar las medidas correctivas como respuestas a desviaciones del plan

```
Evalucion y cierre de pruebas
- Los criterios de salida son registrados como metricas de progreso en el avance de las pruebas
- los criterios de salida son documentados en el informe de prueba para 
su aprobacion 

```

### Medidas de control de pruebas
- Provision de resursos adicionales (Personas, presupuestos)
- Reduccion del esfuerzo aplicado al trabajo
	- Exclusion de variaciones de casos de prueba
	- Simplificacion de objetos de prueba
	- Reduccion de datos prueba
	- Omision de casos de prueba

---
## Gestion de la configuracion 

---
## Riesgo y proceso de prueba

---
## Gestion de incidencias