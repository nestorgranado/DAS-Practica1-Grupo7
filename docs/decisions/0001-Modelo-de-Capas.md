---
status: rejected.
date: 04-02-2023.
---
# ADD-0001-Modelo-Capas

## Context and Problem Statement

{Se necesita una arquitectura software para crear una aplicación de gestión de Fábrica 4.0 y que sea capaz de mostrar los datos recogidos por sensores, notificar usuarios y gestionar los materiales y personal de la fábrica}

## Decision Drivers

* {RF02}

## Considered Options

* {ADD-0001.1-Modelo-Vista-Controlador}
* {ADD-0001.2-Modelo-de-Eventos}.

## Decision Outcome

Chosen option: "{Modelo-de-Capas}", because { Permite dividir el problema en diferentes módulos, que utilizan información y recursos de las capas inferiores, permitiendo resolver diferentes problemas abstrayéndolos del problema general.

### Consequences

* Good, because {nos permite mudularizar mucho el software dividiéndolo en diferentes capas por funcionalidad}
* Bad, because {no permite la navegación entre capas que no sean contiguas y solo permite el uso de capas en una solo dirección}

## Pros and Cons of the Option

### {Pros}

* Ayuda en el diseño de protocolos, ya que los protocolos que operan en una capa específica tienen información definida según la cual actúan, y una interfaz definida para las capas superiores e inferiores.
* Fomenta la competencia, ya que los productos de distintos proveedores pueden trabajar en conjunto.
* Evita que los cambios en la tecnología o en las capacidades de una capa afecten otras capas superiores e inferiores.

### {Cons}

* Problemas con la sincronización.
* Instrumentaciones problemáticas.
* Las capas contienen demasiadas actividades redundantes.
* La gran cantidad de código que es necesario.