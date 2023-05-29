---
status: Accepted.
date: 25-02-2023.
---
# ADD-0007-Adapter.

## Context and Problem Statement

{Se necesita un patron que permita adaptar los sensores que pasan mensajes entre sí.}

## Decision Drivers

* {RF14.1}.

## Decision Outcome

Chosen option: "{Patrón Adapter}", because
{Al recibir una llamada, el adaptador pasa la solicitud al segundo objeto, pero en un formato y orden que ese segundo objeto espera.}


### Consequences

* Good, because {El adaptador obtiene una interfaz compatible con uno de los objetos existentes.
  Utilizando esta interfaz, el objeto existente puede invocar con seguridad los métodos del adaptador.}

## Pros and Cons of the Options

### {Pros}
* Principio de responsabilidad única.
* Principio de abierto/cerrado.


### {Cons}
* La complejidad general del código aumenta, ya que debes introducir un grupo de nuevas interfaces y clases.

