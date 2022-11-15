---

status: Accepted.
date: 12-11-2022.
---
# ADD-0003-Strategy

## Context and Problem Statement

{Se necesita un patrón para la decisión de selección de los algoritmos.}

## Decision Drivers

* {RF05}.
* {RF06}.

## Considered Options

* {ADD-0003.1-State.}

## Decision Outcome

Chosen option: "{Patron Strategy}", because
{Permite encapsular los algoritmos y, delegar la toma de decisión en la selección del mismo a la clase que lo implementa.}

### Consequences

* Good, because {Extraer la toma de la decisión a las clases que lo utilizan.}

## Pros and Cons of the Options

### {Pros}

* Puedes intercambiar algoritmos usados dentro de un objeto durante el tiempo de ejecución.
* Puedes aislar los detalles de implementación de un algoritmo del código que lo utiliza.
* Puedes sustituir la herencia por composición.
* Principio de abierto/cerrado. Puedes introducir nuevas estrategias sin tener que cambiar el contexto.
### {Cons}

*  Los clientes deben conocer las diferencias entre estrategias para poder seleccionar la adecuada.

