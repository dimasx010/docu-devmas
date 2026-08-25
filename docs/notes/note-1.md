---
sidebar_position: 1

title: Nota I
date: 2026-08-24
status: exploring
---

# Nota I

Información del **Nota I**

**Objetivo:**  
Crear un script en Python que renombre archivos de forma masiva.

---

## 🧩 ¿Qué busco resolver?

Tenía una carpeta llena de archivos con nombres desordenados.  
Necesitaba renombrarlos rápido sin hacerlo uno por uno.

---

## 💡 Idea rápida

Usar `os.rename()` y recorrer la carpeta.  
Nada complejo, solo funcional.

---

## 🧪 Cómo funciona

```python
import os

for idx, file in enumerate(os.listdir(".")):
    if file.endswith(".txt"):
        nuevo_nombre = f"archivo_{idx}.txt"
        os.rename(file, nuevo_nombre)
