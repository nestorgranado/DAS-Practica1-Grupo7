---

status: Accepted.
date: 19-11-2022.
---
# ADD-0007-Message-System.

## Context and Problem Statement

{Se necesita un sistema de mensagería que permita informar a los operarios de los cambios producidos.}

## Decision Drivers

* {RF07.1}.

## Decision Outcome

Chosen option: "{Apache Kafka}", because
{Puede verse como una cola de mensajes, bajo el patrón Publish Subscribe

## Pros and Cons of the Options

### {Pros}

* Permite desacoplar aplicaciones entre sí (útil en arquitecturas de microservicios).
* Sistema escalable horizontalmente, tolerante a fallos y con baja latencia (Big Data).
* Absorción de picos de carga que pueden ocurrir en el sistema.
* Permite construir aplicaciones que reaccionan a eventos en tiempo real.
* Referencia en la industria, lo usan las empresas más grandes del mundo.
* Garantías de entrega de mensajes exactly-once (exactamente una vez).
### {Cons}

* Kafka no es una tecnología que esté diseñada para manejar mensajes muy grandes (+ 1MB).
* Pocas opciones de monitorización potentes.
* Opciones en Stream processing más limitadas que otras opciones como Apache Flink.
* Operaciones de rebalanceo de datos en particiones a veces necesarias, lo que impacta en el rendimiento del sistema.

