---
layout: post
title: "Iniciar XAMPP en Linux"
author: Jesús Peralta
date: 2024-04-18
tags: gnu-linux
---

Para iniciar XAMPP simplemente ejecuta este comando:

```bash
sudo /opt/lampp/lampp start
```

Para iniciar la herramienta gráfica ejecutar este comando:

```bash
cd /opt/lampp
sudo ./manager-linux.run (or manager-linux-x64.run)
```

O crear un alias en nuestra shell:

```bash
nano ~/.bashrc

#añadimos la linea
alias xampp='sudo /opt/lampp/manager-linux-x64.run'
```