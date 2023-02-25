---
status: accepted.
date: 05-02-2023.
---
# ADD-0002-Factory-Method

## Context and Problem Statement

{Se necesita un patrón para crear unas familias de sensores, que comparten parte de su funcionalidad.}

## Decision Drivers

* {RF02.1}

## Considered Options

* {ADD-0002.1-Abstract-Factory.}

## Decision Outcome

Chosen option: "{Factory-Method}", because
{Proporciona una interfaz para crear objetos en una superclase, mientras permite a las subclases alterar el tipo de objetos que se crearán.}

### Consequences

* Good, because {Permite mover la creación de objetos a un método concreto.}
* Bad, because {Se usan métodos en vez de objetos.}

## Pros and Cons of the Options

### {Pros}

* Elimina la necesidad de instanciar de forma explícita los objetos que se van a utilizar.
* Permite encapsular en las clases factorías toda la lógica de creación de objetos.
* Es fácilmente extensible.
### {Cons}

* Puede ser que el código se complique, ya que debes incorporar una multitud de nuevas subclases para implementar el patrón.

