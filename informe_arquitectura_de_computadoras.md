# Informe de Investigación Sobre Arquitectura de Computadoras

Electronica IV - TP - Arquitectura de Computadora

Lucas Ahumada Checa Casquero.

## Introducción

-Segun William Stallings en "Computer Organization and Architecture: Designing for Perfomance"(10ma edición, 2016) define una computadora de la siguiente manera:
  Una computadora es una máquina electrónica que opera bajo el control de un conjunto de instrucciones almacenadas llamado programa y que recibe datos, procesa los datos según las instrucciones especificadas y proporciona los resultados como información.
- Siguiendo con la misma bibliografia citada, se define arquitectura de computadora de la siguiente manera:
  La arquitectura de computadoras es la estructura de una computadora, que abarca todo, desde la disposición de los diversos componentes de hardware hasta los detalles específicos de las operaciones del sistema.
- La microarquitectura esta referida en los complicados detalles del diseño interno de los componentes de hardware, como los procesadores, describiendo cómo se materializa la arquitectura en un nivel más detallado. Como lo expresan Patterson y Hennessy, "La microarquitectura se ocupa de los detalles del diseño del procesador" (Patterson & Hennessy, "Computer Organization and Design: The Hardware/Software Interface", 5ta edición, 2013).
Despues, la arquitectura de computadoras abarca tanto el hardware como el software en su diseño conceptual y estructural fundamental, definiendo la estructura y el comportamiento del sistema informático. Tanenbaum destaca este punto al afirmar que "La arquitectura de computadoras es el diseño conceptual y estructural fundamental de un sistema informático" (Tanenbaum, "Structured Computer Organization", 6ta edición, 2012).
Por último, el software comprende el conjunto de instrucciones, programas y datos que dirigen las operaciones de la computadora, transformando las instrucciones en acciones automatizadas. Stallings lo describe de esta manera: "El software es una secuencia de instrucciones que se ejecutan en una computadora" (Stallings, "Computer Organization and Architecture: Designing for Performance", 10ma edición, 2016).

## Clases de arquitectura de computadora

La arquitectura de computadoras abarca una variedad de enfoques que han evolucionado a lo largo del tiempo. Entre los principales tipos encontrados en la bibliografía se destacan la máquina de pila, la máquina de registros y la máquina de acumulador. Además, se discuten las arquitecturas RISC y CISC, así como los modelos Von Neumann y Harvard.

La máquina de pila se caracteriza por utilizar una estructura de pila para almacenar y manipular datos. Según Patterson y Hennessy, "En una máquina de pila, el tope de la pila es donde se realizan todas las operaciones aritméticas y lógicas" (Patterson & Hennessy, "Computer Organization and Design: The Hardware/Software Interface", 5ta edición, 2013). Sus ventajas incluyen una implementación más simple y eficiente para ciertas operaciones, pero puede ser menos intuitiva para los programadores y puede requerir más instrucciones para realizar algunas operaciones.

La máquina de registros se centra en el uso de un conjunto de registros para almacenar y manipular datos. Según Tanenbaum, "En una máquina de registros, los operandos de las instrucciones provienen de los registros de la CPU" (Tanenbaum, "Structured Computer Organization", 6ta edición, 2012). Sus ventajas radican en un acceso rápido a los datos y la posibilidad de optimizar el rendimiento a través de técnicas como el registro renombramiento. Sin embargo, puede requerir un hardware más complejo y costoso para implementar un gran número de registros.

La máquina de acumulador utiliza un único registro acumulador para realizar operaciones aritméticas y lógicas. Según Stallings, "En una máquina de acumulador, el resultado de una operación se almacena en el acumulador" (Stallings, "Computer Organization and Architecture: Designing for Performance", 10ma edición, 2016). Su principal ventaja es la simplicidad de su diseño, pero puede resultar en un código menos eficiente y requiere instrucciones adicionales para transferir datos entre registros y memoria.

En cuanto a las arquitecturas RISC y CISC, la primera se caracteriza por un conjunto de instrucciones reducido y simple, mientras que la segunda presenta un conjunto de instrucciones más complejo y variado. Según Patterson y Hennessy, "Los diseñadores de RISC creen que la simplicidad de las instrucciones lleva a una mayor velocidad de ejecución" (Patterson & Hennessy, "Computer Organization and Design: The Hardware/Software Interface", 5ta edición, 2013). Las ventajas de RISC incluyen una decodificación más simple y un potencial para un rendimiento más rápido, mientras que CISC puede ofrecer una mayor flexibilidad y eficiencia en la programación.

Los modelos Von Neumann y Harvard representan enfoques diferentes para la organización de la memoria y las instrucciones. En la arquitectura Von Neumann, tanto las instrucciones como los datos se almacenan en la misma memoria, mientras que en la arquitectura Harvard se utilizan memorias físicamente separadas para instrucciones y datos. Según Tanenbaum, "La arquitectura de computadoras es el diseño conceptual y estructural fundamental de un sistema informático" (Tanenbaum, "Structured Computer Organization", 6ta edición, 2012). Las ventajas de la arquitectura Harvard incluyen un acceso más rápido a los datos, pero puede requerir hardware adicional para implementar la separación de memorias.

En este contexto, la arquitectura ARMv7M se destaca como una versión de la familia ARM diseñada específicamente para sistemas embebidos y de baja potencia. Con un conjunto de instrucciones RISC, ofrece eficiencia energética y es adecuada para dispositivos móviles y sistemas embebidos. Sin embargo, su enfoque podría limitar su rendimiento en comparación con arquitecturas más potentes en aplicaciones que requieren un cómputo intensivo.

## Partes de una arquitectura de computadora

Explicación de las distintas partes de una arquitectura de computadora:

Unidad Central de Procesamiento (CPU): La CPU es el componente principal de una arquitectura de computadora, responsable de ejecutar instrucciones y coordinar todas las operaciones del sistema. Como afirman Patterson y Hennessy, "La CPU interpreta las instrucciones almacenadas en la memoria y ejecuta las operaciones necesarias" (Patterson & Hennessy, "Computer Organization and Design: The Hardware/Software Interface", 5ta edición, 2013).

Memoria: La memoria es donde se almacenan los datos y las instrucciones que la CPU necesita para operar. Según Tanenbaum, "La memoria es uno de los componentes clave de una arquitectura de computadora, donde se almacenan tanto los programas como los datos" (Tanenbaum, "Structured Computer Organization", 6ta edición, 2012).

Unidades de Entrada/Salida (E/S): Las unidades de E/S facilitan la comunicación entre la computadora y los dispositivos externos, como teclados, monitores y unidades de almacenamiento. Stallings señala que "Las unidades de entrada/salida permiten que la computadora interactúe con el mundo exterior" (Stallings, "Computer Organization and Architecture: Designing for Performance", 10ma edición, 2016).

Buses: Los buses de datos, direcciones y control son los canales de comunicación que conectan la CPU, la memoria y las unidades de E/S. Patterson y Hennessy explican que "Los buses coordinan la transferencia de datos entre los distintos componentes del sistema" (Patterson & Hennessy, "Computer Organization and Design: The Hardware/Software Interface", 5ta edición, 2013).

Análisis de la arquitectura ARMv7M:

La arquitectura ARMv7M, perteneciente a la familia ARM, está diseñada para sistemas embebidos y de baja potencia. Con un conjunto de instrucciones RISC, ofrece eficiencia energética y es adecuada para dispositivos móviles y sistemas embebidos. Según ARM, "ARMv7-M es una arquitectura RISC de 32 bits ampliamente utilizada en sistemas embebidos y de baja potencia" (ARM, "ARM Architecture Reference Manual ARMv7-A and ARMv7-R edition", 2014).

La arquitectura ARMv7M incluye los componentes estándar de una arquitectura de computadora, como CPU, memoria, unidades de E/S y buses. Sin embargo, su diseño y conjunto de instrucciones están optimizados para aplicaciones embebidas, priorizando la eficiencia energética y el rendimiento en entornos con recursos limitados.


## Conclusiones

- ¿Qué es, para tí, una arquitectura de computadoras?
- Si descomponemos un sistema de cómputo en capas ¿Qué posición ocupa la arquitectura?
- ¿Cuál es la función que cumple una arquitectura de computadora?
- ¿Qué considerarías a la hora de elegir una arquitectura de computadora?

*Nota:* El contenido de este capítulo expone lo que aprendiste durante la investigación para desarrollar este práctico. Es un espacio para tu propia reflexión. Intenta exponer tus propias ideas, tal vez sea bueno hacerlo luego de apartarte unas horas del material de referencia para evitar seguir demasiado de cerca una fuente particular.

## Bibliografía

> Aquí listarás todas las fuentes bibliográficas citadas. Sigue para tus citas y referencias las [normas de la APA](https://normas-apa.org/citas/), usando *citas parrafraseadas* en el texto.
