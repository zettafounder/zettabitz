---
layout: post
title: "Cambiar el volumen desde la terminal"
author: Zetta Founder
date: 2024-04-19
---

Subir el volumen 10%: amixer sset Master 10%+
Bajar el volumen 5%: amixer sset Master 5%-
Activar silencio: amixer sset Master mute
Desactivar silencio: amixer sset Master unmute
Activar/desactivar silencio: amixer sset Master toggle

Nota: Si probamos el comando y nos aparece este error: amixer: Unable to find simple control 'Master',0 es porque no existe el control "Master" así que tenemos que ejecutar el comando amixer con otros argumentos para saber como se llama el control.

Así que ejecutamos amixer scontrols y nos saldrá una lista de controles, en mi caso, la línea que interesa es esta: Simple mixer control 'Master Front',0

Entonces reemplazo "Master Front" en los comandos anteriores y ahí funciona perfecto.