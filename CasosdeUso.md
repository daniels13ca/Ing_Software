# Casos de Uso

Un caso de uso representa la forma en que un cliente o clientes (Actor o Actores) interactua con el sistema para cumplir con un requerimiento, el sistema en si mismo representa un actor.

Se enfocan en los requerimientos funcionales y son una muy buena aproximación para comprender como debe funcionar el sistema.

### Buenas prácticas:

* El caso de uso debe describir qué debe hacer el sistema a desarrollar en su interacción con los actores y no cómo debe hacerlo. 
* El nombre del caso de uso debe ilustrar el objetivo que pretende alcanzar el actor al realizarlo.
* El caso de uso debe describir interacciones con los actores sin hacer referencias explícitas a elementos concretos de la interfaz de usuario del sistema a desarrollar.
* La invocación de unos casos de uso desde otros casos de uso (lo que se conoce como inclusión, o extensión si es condicional, en UML), sólo debe usarse como un mecanismo para evitar repetir una determinada secuencia de pasos que se repite en varios casos de uso. Nunca debe usarse para expresar posibles menús de la interfaz de usuario.
* Se debe intentar que todos los casos de uso estén descritos al mismo nivel de detalle.

![Ejemplo caso de uso](https://github.com/daniels13ca/Ing_Software/blob/master/images/Sprint.png "Ejemplo caso de uso")
*Fuente: http://www.juntadeandalucia.es/servicios/madeja/contenido/recurso/416*

## Diagrama de casos de uso

### Elementos

* Actores
* Caso de uso
* Relaciones de uso, herencia y comunicación

**Ejemplo**: Máquina Recicladores *(Fuente: http://stadium.unad.edu.co/ovas/10596_9839/diagramas_de_casos_de_uso.html)*

Se va a diseñar el sistema que controla una máquina recicladora de botellas, tarros y jabas (canastas plásticas), cuyo funcionamiento es el siguiente:

* Registrar el número de  items ingresados
* Imprimir un recibo cuando el cliente lo solicite (se solicita presionando un botón), el recibo:
	* Describe lo depositado
	* Muestra el valor de cada artículo
	* Valor total
* Existe un operador que desea saber lo siguiente:
	* Cuantos ítems han sido retornados por día
	* Al final del día, el resumen de todo lo depositado
* El operador puede modificar:
	* Información asociada a artículos
	* Crear alarmas cuando:
		* Un artículo se atora
		* No hay más papel

**Solución**:

Para comenzar se identifican los actores que interactuan con el sistema:

![Casos de uso 1](https://github.com/daniels13ca/Ing_Software/blob/master/images/Sprint.png "Casos de uso 1")

Luego, cada una de las interacciones individuales que realizan los actores:

![Casos de uso 2](https://github.com/daniels13ca/Ing_Software/blob/master/images/Sprint.png "Casos de uso 2")

Observamos que existen diferentes tipos de artículos a reciclar:

![Casos de uso 3](https://github.com/daniels13ca/Ing_Software/blob/master/images/Sprint.png "Casos de uso 3")

Ahora, para el caso de la impresión de recibos se puede dar a petición del operador o luego de terminar una transacción:

![Casos de uso 4](https://github.com/daniels13ca/Ing_Software/blob/master/images/Sprint.png "Casos de uso 4")

Al integrar todos estos elementos, el diagrama completo es el siguiente:

![Casos de uso 5](https://github.com/daniels13ca/Ing_Software/blob/master/images/Sprint.png "Casos de uso 5")

Observemos los diferentes tipos de relaciones que existen en el diagrama.

##### Tarea

Documentar los casos de uso con sus respectivos diagramas para los dos requerimientos funcionales más importantes según su priorización.


