---
# These are optional elements. Feel free to remove any of them.
Estado: { rejected }
Fecha: { 2023-06-18 }
Decisores: { Juan Carlos Peñaranda, Kevin Acuña, Jorge Franco, Sergio Silva }
Consultores: { Juan Carlos Peñaranda, Kevin Acuña }
Informados: { Jesús Barrios }
---

# Fabrica 4.0: Selección de base de datos

## Contexto y planteamiento del problema

Se pretende diseñar el software de una factoría inteligente compuesta por tres líneas de producción y más de 10 sensores IoT que proporcionan datos sobre el estado de los dispositivos físicos de una factoría inteligente 4.0. Los datos de los sensores se almacenan en una base de datos SQL. Además, se desea tener el inventario de la fábrica almacenado.

## Drivers de decisión

- RF3 - Almacenar inventario
- RF10 - Almacenamiento de informacion de sensores

## Opciones consideradas

- SQLLite

## Decisión final

Opción seleccionada: MySQL porque es más robusto y se desea implementar en un servidor.

### Consecuencias

- Bueno, porque se pueden hacer implementaciones de servidor
- Malo, porque si la fabrica crece y se necesitan bases de datos serverless no se podría

## Validation

Se hizo una revisión con benchmarks

## Pros and Cons de la opción

### SQLLite

- Bueno, porque es un motor de base de datos abierto lo que aumenta la seguridad
- Malo, porque al ser codigo abierto no hay soporte más que el que presta la comunidad
- Neutral, porque permite estructuras bidimensionales
- Bueno, porque permite integridad de la información
- malo, porque no permite flexibilidad de la información
- Neutral, porque es serverless
