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
	* **Caja Negra:**
		* Particiones equivalencia
		* Analisis de valores limite
		* Tabla de decision
		* Pruebas de transicion de estado
		* Analisis de caso de uso 
		 	
	* **Caja Blanca:**
	
		* Cobertura de sentencia
		* Cobertura de Rama
		* Cobertura de condicion
		* Cobertura de camino