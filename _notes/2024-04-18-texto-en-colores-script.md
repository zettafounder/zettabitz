---
layout: post
title: "Texto de colores en un Script para Linux"
author: Zetta Founder
date: 2024-04-18
---

Crea un script en bash colorido con este formato.

**El formato es el siguiente:**

```bash
echo -e "\e#mTexto"
```

**Donde # lo remplazamos por el número de color:**

| **Código** | **Color** |
| --- | --- |
| 30 | negro |
| 31 | rojo |
| 32 | verde |
| 33 | amarillo |
| 34 | azul |
| 35 | magenta |
| 36 | cyan |
| 37 | blanco |

**Ejemplo:**

```bash
echo -e "\e[34mScript \e[33mde \e[31mprueba \e[35mde \e[36mcolores \e[0m"
```

**Resultado:**

![img](https://i.ibb.co/5LzZQpw/texto-script-colores.png)