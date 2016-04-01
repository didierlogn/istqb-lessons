# Capitulo 2

## Modelos de desarrollo de software

Cada etapa del ciclo de desarrollo del software tiene relacionadas sus actividades de prueba

### Modelo V 


Tareas Dev  | Tareas QA
:------------- | :-------------:
Definicion de Requisitos | Pruebas de aceptacion
Diseño funcional | Pruebas de sistema
Diseño tecnico del sistema | Pruebas de integracion
Especificacion de componentes | Pruebas de componente
Programacion |

> **Verificacion**
> > Comprobar la conformidad de los requisitos establecidos.
> > `Se hizo lo q realmente se pidio`
> > `Es verificar los resultados obtenidos con respecto a los requerimientos`
> 
> **Validacion**
> >Comprobacion de la ideoneidad para el uso esperado
> > `Lo que se hizo es realmente lo que se esperaba`
> > `Comprueba si los requerimientos son los correctos`

---
### Modelo W
Es una extencion del modelo V, pone en manifiesto que las actividades de pruebas se desarrollan en paralelo con las actividades de desarrollo


Tareas Dev  | Tareas QA |  | Tareas QA | Tareas de dev
:------------- | :-------------: | ---- | :------------- | :-------------:
Requisitos funcionales | Planificar actividades de prueba |  | Ejecucion de prueba de acceptacion | Depuracion y correccion de errores
Diseño funcional del sistema | Planificar prueba de sistema |  | Ejecucion de prueba de sistema | Depuracion y correccion de errores
Diseño funcional tecnico | Planificar pruebas de integracion |  | Ejecucion de prueba de integracion | Depuracion y correccion de errores 
Especificacion de componentes | Planificacion de pruebas de componentes |  | Ejecucion de pruebas de componentes | Depuracion y correccion de errores

---
### Modelos iterativos

#### Tipos
* Modelo prototipado
* Desarrollo rapido de aplicaciones - Rapid application Developement - RAD
* Proceso unificado - Rational Unified Process - RUP
* Programacion Extrama
* Scrum

#### Caracteristicas

* Cada liberacion es una carateristica adicional al producto
* Cada iteracion puede ser probada por separado
* El regression y automatizacion son una parte clave en las pruebas
* La verificacion y validacion se pueden efectuar por separado

### Principios de los modelos de desarrollo

* Cada actividad de desarrollo debe ser probada por separado
* Cada nivel de pruebo debe ser probado de forma especifica
* El proceso de pruebas debe comenzar mucho antes que la ejecucion de las pruebas

## Niveles de prueba

### Pruebas de componentes
Se pueba cada componente individualmente, los casos de prueba se obtienen de las especificaciones de componente, diseño de software y modelo de datos

Base de pruebas: Requisitos de componente, Diseño detallado, codigo
Objetos de prueba: Componentes, clases modulos, programas, conversion de datos, modulos de bases de datos


Nombre	 | Lenguaje
---------------- | ---
Prueba de clase  | Java C++
Prueba de modulo | C
Prueba de unidad | Pascal

Las pruebas de componente podran comprobar caracteristicas funcionales y no funcionales de un sistema

**Arnes de prueba**
Se requiere para la prueba de componente e integracion 

* Controlador - Driver: Simulan datos de entrada, registran datos de salida, se utilizan herramientas de programacion.
* Stub: Reemplaza o simula un componente que aun no se encuentra disponible o no es parte del objecto de prueba


### Pruebas de integracion - pruebas de interfaz

Comprueban las funciones externas tras las pruebas de componente y la interaccion entre componentes o subsistemas

* Base de pruebas: Diseño de software y sistema, Arquitectura, flujos de trabajo(workflow), casos de uso
* Objectos de pruebas: Implementacion de subsistema de BD, interfaces, infraestructura, configuracion de datos

#### Estrategias de pruebas de integracion

* Big Bang
* Ascendente (bottom-up)
* Descendiente (top-down)
* Ad Hoc


### Pruebas de Sistema

Las pruebas de sistema comprueban el comportamiento del sistema completo.
El alcance esta definido por el plan maestro de pruebas  o plan del nivel de prueba
La calidad del software es obsevada desde el punto de vista del usuario

No son necesarios los drivers o stubs, dado que se prueba la totalidad del sistema

* Bases de prueba: Casos de uso, especificaciones de requisitos de software y sistema, especificacion funcional, manueales de sistema, informes de analisis de riesgos, configuracion del sistema
* Datos de configuracion 

### Pruebas de aceptacion

* **Pruebas de acceptacion contractual y aceptacion de regulacion**: Se cumplen todos los hitos legales? esta todo de acuerdo con el contrato, las pruebas de aceptacion toman en cuenta normas y reglamentos gubernamentales, industriales
* **Pruebas de aceptacion de usuario:**: Son llevadas acabo por los usuarios del sistema, en el entorno del cliente
* **Pruebas de aceptacion operativa:** Son las pruebas llevadas a cabo por los administradores del sistemas del cliente que verifican que el sistema cumple con los requisitos tecnicos correctos

* **Pruebas aceptacion alpha**: Son llevadas a cabo en el entorno del desarrollador
* **Pruebas de aceptacion beta:** Son llevadas a cabo en el entorno propio del cliente

> **Ventajas de pruebas alpha y beta**
>> Reduce el costo de las pruebas de aceptacion
>> Se utilizan distintos entornos de prueba
>> Involucran a un alto numero de usuarios

* Bases de prueba: requisitos de usuario, de sistema, casos de uso, procesos de negocios informes analisis de riesgos
* Objectos de prueba: Procesos de negocios, procedimientos de negocio, procedimientos de usuario

## Tipos de prueba

* **Pruebas funcionales**:  objetivo probar la funcionalidad
Se utilizan los metodos de caja negra.
Estas pruebas se pueden llevar a cabo en todos los niveles de prueba

> Pruebas de seguridad
> > Tipo de prueba funcional q abora amenazas externas
> > Ataques maliciosos podrian dañar programas o datos


* **Pruebas no funcionales:** Objetivo probar las caracteristicas del producto(Fiabilidad, usabilidad, eficiencia, mantenibilidad y portabilidad)

Pruebas de carga: Sistema expuesto a una carga de usuarios 
Pruebas de rendimiento: Rapidez con que el sistema ejecuta una funcion
Pruebas de volumen: Tiempo de procesamiento de grandes cantidades de datos/ficheros
Pruebas de estres: Sobrecarga/recuperacion al entorno a una carga normal

* **Pruebas Estructurales:** Objectivo probar la estructura/arquitectura del sistema
Son las pruebas que se utilizan metodos de caja blanca para su ejecucion.
Tiene como objetivo saber cuanto % de la estructura del objeto de prueba (codigo del sistema) ha sido cubierto por los test cases.

* **Pruebas asociadas al cambio:** Objetivo probar despues de un cambio, dado que luego q el objeto de pruebas a sido modificado es necesario repetir las pruebas con el fin de validar que los requerimientos han sido correctamente cumplidos.
Estas se ejecutan luego de una Extencion funcional del sistema o luego de la correccion de errores.
Se pueden llevar a cabo en cualquier nivel de prueba

Razon del cambio	 | Tipo de pruebas |  |  Final 
---------------- | --- | ---------------- | --- 
Correccion de errores | Pruebas de confirmacion |  |  
 |  | Pruebas de Regression |  
 |  |  |  Release 
 |  | Pruebas de Regression |  
Extension funcional | Nuevos casos de prueba |  |  


Criterios  para la seleccion de casos de prueba de regresion

* Casos con mas alta prioridad
* Funcionalidad estandar, no casos especiales o variaciones
* Probar la configuracion utilizada con mayor frecuencia
* Probar solamente sistemas/zonas seleccionadas para ser tomadas en las pruebas

## Pruebas de mantenimiento

Son las pruebas q se ejecutan luego de que el sistema a sido puesto en producion
Se realizan cuando hay una extension funcional, cuando hay hotfixes o cuando el sistema se va a sacar de produccion.
Es necesario la ejeccion de pruebas de regression por lo que el analisis de impacto ayudara a juzgar los cambios asociacidos con el riesgo y asi establecer el set de pruebas necesarios.
Las pruebas de migracion de datos son importantes 