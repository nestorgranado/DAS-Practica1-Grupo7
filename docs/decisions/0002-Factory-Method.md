---

status: rejected.
date: 09-11-2022.
---
# ADD-0002-Factory-Method

## Context and Problem Statement

{Se necesita un patrón para crear una familias de sensores, que comparten parte de su funcionalidad.}

## Decision Drivers

* {RF03}

## Considered Options

* {ADD-0002.1-Abstract-Factory.}

## Decision Outcome

Chosen option: "{Factory-Method}", because
{Proporciona una interfaz para crear objetos en una superclase, mientras permite a las subclases alterar el tipo de objetos que se crearán.}

### Consequences

* Good, because {Permite mover la creacion de objetos a un methodo concreto.}
* Bad, because {Se usan metodos en vez de objetos.}



## Pros and Cons of the Options

### {Pros}

* Elimina la necesidad de instanciar de forma explícita los objetos que se van a utilizar.
* Permite encapsular en las clases factorías toda la lógica de creación de objetos.
* Es fácilmente extensible.
### {Cons}

* Puede ser que el código se complique, ya que debes incorporar una multitud de nuevas subclases para implementar el patrón.

