---
status: Accepted.
date: 11-02-2022.
---
# ADD-0005-Publish-Subscribe

## Context and Problem Statement

{Se necesita un patron de diseño para suscribirse a una serie de eventos y ser notificado cuando sucedan.}

## Decision Drivers

* {RF12}.
* {RF13}.

## Decision Outcome

Chosen option: "{Patrón Publish-Subscribe }", because
{Necesitamos notificar a nuestros usuarios cuando sucede un evento.}

### Consequences

* Good, because {Permite que los usuarios se subscriban a un evento para ser notificados cuando este suceda.}

## Pros and Cons of the Options

### {Pros}

* Perdida de acoplamiento de los subscriptores, ya que el programa no necesita saber nada sobre ellos.
* Alta escalabilidad.
### {Cons}

* Posibles problemas con la entrega de los mensajes.

