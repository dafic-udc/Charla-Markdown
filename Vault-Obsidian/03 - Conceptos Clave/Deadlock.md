---
aliases:
  - Interbloqueo
  - Abrazo mortal
tags:
  - concepto
  - concurrencia
---

# Deadlock (Interbloqueo)

Un **deadlock** es una situación en la que un conjunto de procesos se bloquea permanentemente debido a que cada proceso retiene al menos un recurso y está esperando adquirir un recurso retenido por otro proceso del conjunto. ^definicion

## Condiciones de Coffman

Para que ocurra un deadlock, deben cumplirse **simultáneamente** las cuatro condiciones siguientes:

1. **Exclusión Mutua:** Al menos un recurso debe ser mantenido en modo no compartido.
2. **Retención y Espera (Hold and Wait):** Un proceso debe retener al menos un recurso y esperar adquirir recursos adicionales retenidos por otros.
3. **Sin Expropiación (No Preemption):** Los recursos no pueden ser expropiados; solo pueden ser liberados voluntariamente por el proceso.
4. **Espera Circular:** Debe existir un conjunto $\{P_0, P_1, ..., P_n\}$ de procesos en espera tal que $P_0$ espera por $P_1$, $P_1$ por $P_2$, ..., $P_n$ por $P_0$.

> [!tip] Prevención de Deadlocks
> La prevención busca asegurar que al menos una de las condiciones de Coffman nunca se cumpla. Frecuentemente se ataca la condición de *Espera Circular* estableciendo un orden estricto para solicitar recursos.
