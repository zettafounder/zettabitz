---
layout: note
title: "Comandos básicos apt Debian"
author: Jesús Peralta
date: 2024-04-19
tags: gnu-linux
---

Listar paquetes instalados

```bash
apt list --installed | grep gddc
```

Eliminar paquete instalado

```bash
sudo apt --purge remove gddccontrol
```

Eliminar los juegos preinstalados de gnome

```bash
sudo apt --purge autoremove gnome-games
```