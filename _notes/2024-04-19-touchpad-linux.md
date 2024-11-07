---
layout: note
title: "Activar touchpad en i3wm"
date: 2024-04-19
---

## Activar tap del touchpad

Section "InputClass"
Identifier "touchpad"
Driver "libinput"
MatchIsTouchpad "on"
Option "Tapping" "on"
Option "TappingButtonMap" "lmr"
EndSection