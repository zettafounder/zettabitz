---
layout: note
title: "Ejecutar una orden al iniciar la terminal"
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

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/2d649050-51c0-44ef-aba5-a9611375d6a2/bc5942ca-2aa8-4540-a1fe-5b23c4df970c/Untitled.png)
![Untitled](./../assets/Untitled.png)

```bash
#guardamos con ctrl + s
#cerramos el editor con ctrl + x

#listo, lanza tu terminal y mira la magia
```