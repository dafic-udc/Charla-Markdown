---
aliases:
  - Thread
  - Hilo de ejecución
tags:
  - concepto
  - procesos
---

# Hilo (Thread)

Un hilo, a veces llamado proceso ligero (LWP - Lightweight Process), es la unidad básica de utilización de la CPU. 

## Componentes

Comprende:
- Un ID de hilo.
- Un contador de programa (PC).
- Un conjunto de registros.
- Una pila (Stack).

## Relación con Procesos

Comparte con otros hilos que pertenecen al mismo [[Tema 2 - Gestión de Procesos|proceso]] la sección de código, la sección de datos y otros recursos del sistema operativo, como los archivos abiertos y las señales.

| Característica | Proceso | Hilo |
| :--- | :--- | :--- |
| **Aislamiento** | Alto (espacio de memoria propio) | Bajo (comparten memoria) |
| **Tiempo de Creación** | Alto | Bajo |
| **Comunicación** | IPC (Lenta, compleja) | Memoria compartida (Rápida) |

> [!bug] Riesgos de usar Hilos
> Dado que comparten la misma memoria, es muy fácil causar condiciones de carrera si dos hilos intentan escribir en la misma variable global al mismo tiempo. Aquí es donde entra la importancia de los mutex y semáforos.
