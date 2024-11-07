---
layout: note
title: "Crear lanzador en GNU/Linux"
date: 2024-04-19
---

Nos ubicamos en el directorio `/usr/share/applications` para añadir un lanzador en todo el sistema y en el directorio `/home/username/.local/share/applicatios/` para añadirlo solo al menú de un usuario en específico.

Una vez ubicados en este directorio crearemos un archivo con la siguiente estructura:

```bash
[Desktop Entry]
Name=
Type=
Categories=
Exec=
Icon=
Keywords=
```

Y rellenaremos los campos según lo necesitemos:

```bash
[Desktop Entry]
Name=VS Code
Type=Application
Categories=Programación
Exec=~/Programas/VSCode/bin/code
Icon=~/Iconos/vscode.png
Keywords=Programación;VS;Code;HTML;Python;
```

Guardamos el archivo con un nombre descriptivo, seguido de la extención `.desktop`, como por ejemplo: vscode.desktop y reiniciamos nuestra sesión grafica si es necesario y listo tendremos el lanzador que creamos en nuestro menu de aplicaciones.