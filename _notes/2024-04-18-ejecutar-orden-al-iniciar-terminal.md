---
layout: post
title: "Ejecutar una orden al iniciar la terminal"
author: Zetta Founder
date: 2024-04-18
---
Si al lanzar una terminal quieres que se ejecute un comando como por ejemplo `neofetch` lo que tenemos que hacer es editar el archivo de configuración de nuestra shell. Y añadir la orden que deseemos al final del archivo.

Este archivo se encuentra en la carpeta principal del usuario.

Para bash editaremos el archivo con la ruta `~/.bashrc`

Y para zsh es `~/.zshrc`

# Pasos en consola

```bash
#abrios el archivo con el editor nano
nano ~/.bashrc

#añadimos la linea `neofetch` al final del archivo (ver imagen siguiente)
```

![img](https://i.ibb.co/N7Jg6z7/image.png)
![Untitled](https://prnt.sc/32EKxoXBjIlN)

```bash
#guardamos con ctrl + s
#cerramos el editor con ctrl + x

#listo, lanza tu terminal y mira la magia
```