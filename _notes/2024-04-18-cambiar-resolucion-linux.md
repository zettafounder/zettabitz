---
layout: post
title: "Cambiar la resolución de pantalla desde la terminal en Linux"
author: Zetta Founder
date: 2024-04-18
---

Obtenemos las resoluciones disponibles de nuestro monitor ejecutado el comando `xrandr` y obtendremos la siguiente salida:

!https://i.ibb.co/HzSPyTG/resolucion.png

Ahora ejecutaremos el comando `xrandr -s #` remplazando # por el número de resolución que queramos poner empezando desde 0.

Por ejemplo, si queremos poner la resolución 800x600 el comando ejecutaríamos:

```bash
xrandr -s 3
```