---
status: Accepted.
date: 11-02-2023.
---
# ADD-0006-BDD-MongoDB.

## Context and Problem Statement

{Se necesita una base de datos para almacenar los datos de los sensores, las órdenes de trabajo y el registro de materiales.}

## Decision Drivers

* {RF01}.
* {RF05}.

## Considered Options

* {0006.1-BDD-DocumentDB}.

## Decision Outcome

Chosen option: "{MongoDB}", because
{Es una base de datos no relacional que permite manejar un gran volumen de datos con variedad de estructuras.}


### Consequences

* Good, because {Alta velocidad, implementa funciones de seguridad, es una base de datos de licencia libre y nor requiere de ningún servidor en la nube.}

## Pros and Cons of the Options

### {Pros}
* Es ideal para entornos con pocos recursos de computación.
* Es una herramienta con un coste bajo.
* Tiene una gran documentación.
* Es un complemento perfecto para JavaScript.


### {Cons}
* No es una base de datos adecuada para aplicaciones con transacciones complejas.
* Es una tecnología joven.
* No tiene Joins para consultas.


