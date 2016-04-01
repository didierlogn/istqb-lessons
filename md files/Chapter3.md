#Capitulo 3

## Tecnicas estaticas y procesos de prueba

## Proceso de revisiones

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

