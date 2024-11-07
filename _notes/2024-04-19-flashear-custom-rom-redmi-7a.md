---
layout: post
title: "Flashear custom rom en redmi 7a"
author: Jesús Peralta
date: 2024-04-19
tags: android
---

## Metodo 1

Una vez tienes el custom recovery (y flasheaste el vbmeta para que no se quite), haz backup de lo que tengas importante porque borraras todo.

1. Vas a wipe o advanced wipe y borras system/cache/dalvik/data/vendor.
Formateas data (ten la rom y demás en una tarjeta externa o copia los archivos luego de borrar todo).
2. Instalas la rom, luego las gapps y haces format data. Después el kernel cherry y magisk si quieres root. Iniciar.
Importante tener telegram abierto en otro lado por si no encuentras una opción o falla algo.

Cuando digo de instalar es ir a la pantalla principal del recovery, tocar instalar y seleccionar los archivos zip.

## Metodo 2

[Reenviado de Rose]
📌 Instalar Custom ROM

🎮 Requisitos para instalar Custom ROM de 64bits:

💻 #adb (si es primera vez para recovery).
🎯 #recovery (64bits).
🧩 #customs_roms64 (la ROM que elijas).
📦 #gapps (GApps64 de tu preferencia).

👇🏻 Instrucciones para instalar:

1. Reinicia en modo recovery
⚡️ Power + Vol ⬆️
2. Format DATA
wipe > format data > escribe yes
3. Wipes
wipe todo excepto SD y OTG
4. Flas5OM 🤑
5. Instalar Gapps
install > select storage > gapps > swipe
6. Format DATA por segunda vez
wipe > format data > escribe yes
7*. Reiniciar y disfrutar 😎*

📆 Actualizado 04-08-2021.

## Metodo 3

[Reenviado de Rose]
Si ya has desbloqueado el bootloader e instalado un #recovery estos son los pasos:

1. Realizar una copia de seguridad de todos tus archivos de la memoria interna
2. Formatear data: Esto desencriptará el dispositivo y permitirá el acceso a la carpeta data, la cual luego podrá ser modificada para borrar sus archivos (Ej. Previas instalaciones de magisk, módulos, aplicaciones en data/app)
3. Wipe/Borrar particiones System - Vendor - Caches (Suelen sobreescribirse pero nunca está de más)
4. Instalar ROM (Ej. lineage.zip_)_
5. Instalar #gapps y Formatear data (Opcional y omitir si tu rom tiene GApps)
6. Instalar #kernel (Opcional)
7. Instalar #magisk (Opcional)
Adicional Android 12
8. Brevemente, si ve letras raras en el recovery, remueva la contraseña de su sistema antes de ir a este. Buscar nota #recoveryencriptado para información detallada