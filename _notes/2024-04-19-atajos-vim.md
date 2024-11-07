---
layout: note
title: "Navegación y atajos VIM"
date: 2024-04-19
---

## Navegación

| H | J | K | L |
| --- | --- | --- | --- |
| ← | ↓ | ↑ | → |

## Atajos

| Teclas | Descripción |
| --- | --- |
| w | Siguiente palabra |
| b | Anterior palabra |
| e | Final de la palabra |
| i | Modo Insertar |
| Esc | Modo normal |
| a | Insertar despues de la letra |
| A | Insertar al final de la linea |
| x | Eliminar 'Del' |
| dd | Eliminar linea |
| d + $ | Limpiar desde el cursor al final de la linea |
| g + d | Ir a la declaración de la función |
| g + f | Ir al archivo |
| Ctrl + o | Bufer anterior |
| Ctrl + i | Bufer siguiente |
| d + w | Eliminar palabra |
| d + b | Eliminar palabra anterior |
| d + e | Eliminar hasta el final de la palbra |
| x, [operador] | Repite en operador o movimiento x número de veces |
| 4, d +w | Equivale a eliminar 4 palabras (ejemplo) |
| u | Desacer |
| Ctrl + r | Rehacer |
| p | Pegar lo eliminado anteriormente (linea, palabra) |
| P | Pegar en la linea de arriba (reordenar lineas) |
| x, dd | Cortar x lineas (8, dd = cortar 8 lineas) |
| r | Reemplazar caracter |
| c + w | Cambiar palabra o resto de palabra |
| c + i + w | Cambia el objeto de la palabra |
| gg | Ir al principio del archivo |
| G | Ir al final de archivo |
| x, G | Ir a la linea x (16, G = Ir a la linea 16) |
| / | Buscar siguiente (Enter y moverse entre resultados con n) |
| ? | Buscar anterior |
| % | Moverse entre parentesis correspondientes ((),[],{}) |
| o | Insertar nueva linea |
| O | Insertar nueva linea sobre el cursor |
| R | Modo reemplazar |
| V | Modo visualizar (sirve para seleccionar) |
| x | En modo visualizar borra lo seleccionado |
| y | Copiar lo seleccionado |

## Comandos
| Comando | Descripción |
| --- | --- |
| :q | Salir de Vim |
| :q! | Forzar salir sin guardar |
| :w | Guardar cambios |
| :wq | Guardar cambios y salir |
| :s/x/x/g | Remplaza una palabra en una linea |
| :%s/x/x/gc | Remplaza una palabra en todo el archivo |