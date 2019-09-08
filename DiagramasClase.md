# Diagramas de clases

## ¿Qué es un diagrama de clases?

En el Lenguaje Unificado de Modelado (UML), el diagramas de clases es un tipo de diagrama de estructura estática que describe la estructura de un sistema mostrando las clases del sistema, sus atributos, operaciones (o métodos), y las relaciones entre los objetos.

Son un tipo de diagrama de estructura porque describen lo que debe estar presente en el sistema que se está modelando. 

El UML se estableció como un modelo estandarizado para describir un enfoque de programación orientada a objetos (POO), de esta forma estos diagramas (de clases) se pueden considerar entre los más importantes.

## Beneficios

* Ilustrar modelos de datos para sistemas de información, sin importar qué tan simples o complejos sean.

* Comprender mejor la visión general de los esquemas de una aplicación.

* Expresar visualmente cualesquier necesidades específicas de un sistema y divulgar esa información en toda la empresa.

* Crear diagramas detallados que resalten cualquier código específico que será necesario programar e implementar en la estructura descrita.

* Ofrecer una descripción independiente de la implementación sobre los tipos empleados en un sistema que son posteriormente transferidos entre sus componentes.

## Clase

**Sección superior:** Contiene el nombre de la clase. Esta sección siempre es necesaria, ya sea que estés hablando del clasificador o de un objeto.

**Sección central:** Contiene los atributos de la clase. Usa esta sección para describir cualidades de la clase. Esto solo es necesario al describir una instancia específica de una clase.

**Sección inferior:** Incluye operaciones de clases (métodos). Esto está organizado en un formato de lista. Cada operación requiere su propia línea. Las operaciones describen cómo una clase puede interactuar con los datos.

IMAGEN DE UNA CLASE 

Modificadores de acceso a miembros
Todas las clases poseen diferentes niveles de acceso en función del modificador de acceso (visibilidad). A continuación te mostramos los niveles de acceso con sus símbolos correspondientes:

Público (+)
Privado (-)
Protegido (#)

Interacciones
El término "interacciones" se refiere a múltiples relaciones y enlaces que pueden existir en diagramas de objetos y de clases. Algunas de las interacciones más comunes incluyen:

Herencia: El proceso en el que una subclase o clase derivada recibe la funcionalidad de una superclase o clase principal, también se conoce como "generalización". Se simboliza mediante una línea de conexión recta con una punta de flecha cerrada que señala a la superclase.

IMAGEN HERENCIA DE LA REFERENCIA

En este ejemplo, el objeto "Auto" heredaría todos los atributos (velocidad, números de pasajeros, combustible) y los métodos (arrancar(), frenar(), cambiarDirección()) de la clase principal ("Vehículo"), además de los atributos específicos (tipo de modelo, número de puertas, fabricante del auto) y métodos de su propia clase (Radio(), limpiaparabrisas(), aireacondicionado/calefacción()). La herencia se muestra en un diagrama de clases por medio de una línea continua con una flecha cerrada y vacía.

Asociación bidireccional: La relación predeterminada entre dos clases. Ambas clases están conscientes una de la otra y de la relación que tienen entre sí. Esta asociación se representa mediante una línea recta entre dos clases.

asociación bidireccional en diagrama de clases
En el ejemplo anterior, la clase Auto y la clase Viaje están interrelacionadas. En un extremo de la línea, el Auto recibe la asociación de "autoAsignado" con el valor de multiplicidad de 0..1, de modo que cuando la instancia de Viaje existe, puede tener una instancia de Auto asociada a ella o no tener instancias de Autos asociadas a ella. En este caso, una clase CasaRodante separada con un valor de multiplicidad de 0..* es necesaria para demostrar que un Viaje puede tener múltiples instancias de Autos asociadas a ella. Dado que una instancia de Auto podría tener múltiples asociaciones "iniciarViaje", en otras palabras, un auto podría realizar múltiples viajes, el valor de multiplicidad se establece en 0..*

Asociación unidireccional: Una relación un poco menos común entre dos clases. Una clase está consciente de la otra e interactúa con ella. La asociación unidireccional se dibuja con una línea de conexión recta que señala una punta de flecha abierta desde la clase "knowing" a la clase "known".

asociación unidireccional en diagrama de clases
Como ejemplo, en tu viaje por Arizona, podrías encontrarte con una trampa de velocidad donde un radar de tráfico registra la velocidad a la que conducías, pero no lo sabrás hasta que recibas la notificación por correo. Esto no está dibujado en la imagen, pero en este caso, el valor de multiplicidad sería 0..* en función de cuántas veces hayas conducido frente al radar de tráfico.

Ejemplo:

Diagrama de clases para un sistema de cajero automático ATM
Los ATM son aparentemente simples. Aunque los clientes solo necesitan oprimir algunos botones para recibir efectivo, hay muchas capas de seguridad que un ATM seguro y efectivo debe pasar para evitar fraude y brindar valor a los clientes bancarios. Las diversas partes humanas e inanimadas de un sistema de ATM son ilustradas por este diagrama sencillo de leer. Cada clase tiene su título y los atributos se detallan debajo. Puedes editar, guardar y compartir este diagrama abriendo el documento y registrándote a una cuenta gratuita de Lucidchart.

*Fuentes*:

* https://www.lucidchart.com/pages/es/tutorial-de-diagrama-de-clases-uml
* https://es.wikipedia.org/wiki/Diagrama_de_clases

