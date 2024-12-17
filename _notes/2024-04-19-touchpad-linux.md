---
layout: note
title: "Activar touchpad en i3wm"
author: Zetta Founder
date: 2024-04-19
tags: gnu-linux
---

## Activar tap del touchpad

Section "InputClass"
Identifier "touchpad"
Driver "libinput"
MatchIsTouchpad "on"
Option "Tapping" "on"
Option "TappingButtonMap" "lmr"
EndSection