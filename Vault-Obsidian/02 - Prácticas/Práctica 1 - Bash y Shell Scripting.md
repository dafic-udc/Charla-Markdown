---
tags:
  - práctica
  - bash
  - linux
fecha_entrega: 2026-05-15
nota: 
---

# Práctica 1: Bash y Shell Scripting

## Objetivos
- Aprender a moverse por el sistema de archivos mediante la terminal.
- Crear un script que automatice la creación de usuarios.

## Código de Ejemplo

A continuación, un ejemplo de cómo leer un archivo línea por línea en Bash:

```bash
#!/bin/bash
# Script para leer usuarios desde un archivo

ARCHIVO="usuarios.txt"

if [[ ! -f $ARCHIVO ]]; then
    echo "El archivo $ARCHIVO no existe."
    exit 1
fi

while IFS= read -r usuario; do
    echo "Creando al usuario: $usuario"
    useradd "$usuario"
done < "$ARCHIVO"
```

## Tareas

- [ ] Instalar máquina virtual con Ubuntu.
- [ ] Entender permisos en Linux (`chmod`, `chown`).
- [x] Escribir el script básico.

> [!warning] Cuidado con sudo
> Ejecutar scripts con `sudo` puede dañar el sistema si no controlas lo que hace cada comando. **Revisa tu código antes de ejecutarlo**.

## Enlaces externos útiles
- [Guía de Bash Scripting (Bash Guide)](https://mywiki.wooledge.org/BashGuide)
- [Explicación de permisos en Linux](https://wiki.archlinux.org/title/File_permissions_and_attributes)
