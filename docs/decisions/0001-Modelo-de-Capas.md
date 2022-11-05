---
status: proposed.<br>
date: 05-11-2022.
---
# ADD-0001-Modelo-Capas

## Context and Problem Statement

{Se necesita una arquitectura software para crear una aplicación de gestión de Fábrica 4.0 y que sea capaz de mostrar los datos recogidos por sensores, notificar usuarios y gestionar los materiales y personal de la fábrica}

<!-- This is an optional element. Feel free to remove. -->
## Decision Drivers

* {RF01}
* {RF02}
* {RF03}
* {RF04}

## Considered Options

* {ADD-0001.1-Modelo-Vista-Controlador}


## Decision Outcome

Chosen option: "{Modelo-de-Capas}", because { Permite dividir el problema en diferentes modulos, que utilizan información y recursos de las capas inferiores, permitiendo resolver diferentes problemas abstrayendolos del problema general.
{justification. e.g., only option, which meets k.o. criterion decision driver | which resolves force {force} | … | comes out best (see below)}.

<!-- This is an optional element. Feel free to remove. -->
### Consequences

* Good, because {nos permite mudularizar mucho el software dividiendolo en diferentes capas por funcionalidad}
* Bad, because {no permite la navegacion entre capas que no sean contiguas y solo permite el uso de capas en una solo diercción}

<!-- This is an optional element. Feel free to remove. -->
## Pros and Cons of the Option

### {Pros}

* Ayuda en el diseño de protocolos, ya que los protocolos que operan en una capa específica tienen información definida según la cual actúan, y una interfaz definida para las capas superiores e inferiores.
* Fomenta la competencia, ya que los productos de distintos proveedores pueden trabajar en conjunto.
* Evita que los cambios en la tecnología o en las capacidades de una capa afecten otras capas superiores e inferiores.

### {Cons}

* Problemas con la sincrinización.
* instrumentaciones problemáticas.
* Las capas contienen demasiadas actividades redundantes.
* La gran cantidad de código que es necesario.
