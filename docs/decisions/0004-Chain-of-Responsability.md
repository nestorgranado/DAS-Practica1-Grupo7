---

status: Accepted.
date: 12-11-2022.
---
# ADD-0004-Chain-of-Responsability.

## Context and Problem Statement

{Se necesita un patrón para el paso de información entre diferentes sensores de la misma familia.}

## Decision Drivers

* {RF09}.

## Decision Outcome

Chosen option: "{Patron Chain of Responsability}", because
{Permite pasar solicitudes a lo largo de una cadena de manejadores. Al recibir una solicitud, cada manejador decide si la procesa o si la pasa al siguiente manejador de la cadena.}

### Consequences

* Good, because {Permite pasar solicitudes a lo largo de una cadena de manejadores. Al recibir una solicitud, cada manejador decide si la procesa o si la pasa al siguiente manejador de la cadena.}

## Pros and Cons of the Options

### {Pros}

* Puedes controlar el orden de control de solicitudes.
* Principio de responsabilidad única. Puedes desacoplar las clases que invoquen operaciones de las que realicen operaciones.
* Principio de abierto/cerrado. Puedes introducir nuevos manejadores en la aplicación sin descomponer el código cliente existente.

### {Cons}

* Algunas solicitudes pueden acabar sin ser gestionadas.
