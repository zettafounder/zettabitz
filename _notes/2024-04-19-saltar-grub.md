---
layout: note
title: "Saltar selector de S.O. GRUB"
author: Jesús Peralta
date: 2024-04-19
tags: gnu-linux
---

1. nano /etc/default/grub
2. GRUB_TIMEOUT=0
3. Guardar cambios
4. sudo grub-mkconfig -o /boot/grub/grub.cfg