---
layout: note
title: "Crea una USB booteable de Linux usando el comando dd"
author: Zetta Founder
date: 2024-04-17
tags: gnu-linux
---

Una de las razones por las que he decidido utilizar este comando para crear mis USBs booteables fue que este se encuentra en cualquier sistema con Linux.

# Sintaxis

La forma sencilla de usar el comando es:

```bash
sudo dd if=rutadela.iso of=/dev/sdX
```

Remplazando la X por la letra que corresponda a nuestra unidad USB.

# Creando la USB booteable

1. Inserta tu USB
2. Ejecuta el comando `lsblk` para obtener la ruta de tu unidad, en mi caso es `sdb`
3. Ahora nos vamos a la ruta de nuestra `.iso` navegando con `cd`, en mi caso esta en la carpeta de descargas, `cd ~/Descargas`
4. Y ejecutaremos el comando `dd`, quedando así finalmente:
    
    ```bash
    sudo dd if=archlinux-2022.01.01-x86_64.iso of=/dev/sdb
    ```
    
5. Una ves finalice podremos usar nuestra USB booteable.

# Pasos en consola

```bash
#ejecutamos el comando lsblk para listar dispositivos

[jpz@hackerz ~]$ lsblk
NAME   MAJ:MIN RM   SIZE RO TYPE MOUNTPOINTS
sda      8:0    0 931.5G  0 disk 
└─sda1   8:1    0 931.5G  0 part /
sdb      8:16   1   1.9G  0 disk 
└─sdb1   8:17   1   1.9G  0 part 

#nos dirigimos a la ruta de nuestra .iso

[jpz@hackerz ~]$ cd ~/Descargas/

#ejecutamos el comando dd para comenzar el booteo

[jpz@hackerz Descargas]$ sudo dd if=archlinux-2022.01.01-x86_64.iso of=/dev/sdb
1770136+0 registros leídos
1770136+0 registros escritos
906309632 bytes (906 MB, 864 MiB) copied, 298.709 s, 3.0 MB/s
[jpz@hackerz Descargas]$ 

#proceso finalizado
```

# Recomendaciones

Existen otros atributos que nos permiten visualizar el progreso de escritura de la imagen en nuestro dispositivo. De hecho distribuciones conocidas como Arch Linux, Majaro, EndeavourOS y MX-Linux tienen recomendaciones de como se debe crear una USB booteable de su `.iso` utilizando el comando `dd`, estás son sus usos recomendados:

```bash
#EndeavourOS
sudo dd bs=4M if=endeavouros.iso of=/dev/sdX conv=fsync oflag=direct status=progress

#MX-Linux
sudo dd bs=4M if=MX-Linux.iso of=/dev/sdX && sync

#Manjaro
sudo dd bs=4M if=manjaro.iso of=/dev/sdX status=progress oflag=sync

#Arch Linux
sudo dd bs=4M if=archlinux.iso of=/dev/sdX status=progress oflag=sync

#Void Linux
sudo dd bs=4M if=void.iso of=/dev/sdX

#Linux Mint (unoffical)
sudo dd if=linuxmint.iso of=/dev/sdX

#Debian (unofficial)
sudo dd bs=4M if=debian.iso of=/dev/sdX status=progress oflag=sync

#Ubuntu (unoficial)
sudo dd if=ubuntu.iso of=/dev/sdX bs=4M && sync
```