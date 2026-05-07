---
cssclasses:
  - dashboard
tags:
  - "#inicio"
  - "#dashboard"
created: 2026-05-06
updated: 2026-05-06
---

# 💻 Asignatura: Sistemas Operativos (SO)

> [!abstract] Resumen de la Asignatura
> Bienvenido al centro de control de **Sistemas Operativos**. Aquí encontrarás todos los recursos necesarios para dominar la gestión de recursos del hardware, la abstracción de procesos, y la sincronización. 

---

## 📚 Navegación Principal

- [[Tema 1 - Introducción a los Sistemas Operativos|📖 Tema 1: Introducción]]
- [[Tema 2 - Gestión de Procesos|⚙️ Tema 2: Gestión de Procesos]]
- [[Práctica 1 - Bash y Shell Scripting|💻 Práctica 1: Scripting]]

## 📌 Conceptos Clave Recientes
![[Deadlock#^definicion]]

*Revisa también:* [[Hilo (Thread)]]

---

## ✅ Tareas Pendientes

- [ ] Repasar el concepto de sección crítica.
- [ ] Entregar la [[Práctica 1 - Bash y Shell Scripting]] antes del viernes.
- [x] Configurar el vault de Obsidian.

---

## 📊 Progreso (Dataview)

> [!info] Tareas dinámicas
> *(Nota: Requiere el plugin Dataview para funcionar)*
> ```dataview
> TASK
> FROM "02 - Prácticas" OR "01 - Teoría"
> WHERE !completed
> GROUP BY file.folder
> ```

---

## 📈 Ecuación del Rendimiento

Para calcular la utilización de la CPU ($U$), usamos la fórmula:

$$
U = 1 - p^n
$$

Donde $p$ es la probabilidad de que un proceso esté esperando por I/O, y $n$ es el número de procesos en memoria. [^1]

[^1]: Extraído del libro *Sistemas Operativos Modernos*, Andrew S. Tanenbaum.
