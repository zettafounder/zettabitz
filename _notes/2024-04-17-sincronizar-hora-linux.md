---
layout: post
title: "Sincronizar la hora en Linux"
author: Zetta Founder
date: 2024-04-17
tags: gnu-linux
---

Esta nota es más que nada para personas a las que se les cambia la hora por un error en la zona horaria por tener dual boot con windows.

Bastara con ejecutar estos comandos:

```bash
timedatectl
sudo timedatectl set-ntp true
timedatectl
```