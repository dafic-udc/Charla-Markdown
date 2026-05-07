---
aliases:
  - Intro a SO
tags:
  - teoría
  - tema/1
  - sistemas-operativos
estado: "terminado"
---

# Tema 1: Introducción a los Sistemas Operativos

## ¿Qué es un Sistema Operativo?

Un Sistema Operativo (SO) es un programa o conjunto de programas de un sistema informático que gestiona los recursos de hardware y provee servicios a los programas de aplicación de software. Funciona como un **intermediario** entre el usuario y el hardware.

> [!important] Objetivo Principal
> El objetivo principal de un SO es lograr que el sistema informático se use de manera **eficiente** y **cómoda**.

## Componentes Principales

1. **Gestión de Procesos:** (Ver [[Tema 2 - Gestión de Procesos]])
2. **Gestión de Memoria Principal:** Asignación y liberación de espacio.
3. **Gestión de Almacenamiento Secundario.**
4. **Sistema de Entrada/Salida (I/O).**
5. **Sistema de Archivos.**
6. **Sistemas de Protección y Seguridad.**

## Tipos de Sistemas

| Tipo | Descripción | Ejemplo |
| ---- | ----------- | ------- |
| **Monotarea** | Solo puede ejecutar un proceso a la vez. | MS-DOS |
| **Multitarea** | Permite ejecutar varios procesos concurrentemente. | Linux, Windows |
| **Multiusuario** | Permite a varios usuarios interactuar al mismo tiempo. | Unix |

## Arquitectura de Niveles (Anillos de Privilegio)

El hardware suele soportar al menos dos modos de operación para protegerse de errores del usuario:
- **Modo Usuario (User mode):** Privilegios restringidos.
- **Modo Kernel (Kernel mode):** Privilegios totales sobre el hardware.

La transición de modo usuario a kernel ocurre mediante una ==llamada al sistema== (System Call).
