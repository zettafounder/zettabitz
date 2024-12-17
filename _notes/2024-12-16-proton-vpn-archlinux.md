---
layout: note
title: "Activar Proton VPN en Arch Linux"
author: Zetta Founder
date: 2024-12-16
tags: gnu-linux
---
Hay un cliente oficial para Ubuntu, Debia y Fedora y aunque hay versiones AUR y Flatpak estás no son recomendadas en la propia web de Proton VPN y nos dejan 2 opciones para utilizar Proton VPN en otros sistemas Linux: OpenVPN y WireGuard.

En este caso quiero activar Proton VPN en Arch Linux, para ello seguí estos pasos:

1. Instalación de WireGuard, para ello instale el paquete wireguard-tools como se menciona en su página web [WireGuard.com](https://www.wireguard.com/install/).
2. Descargue el archivo de configuración de la VPN en account.protonvpn.com, en la sección de descargas en la parte de WireGuard configuration.
3. Movi el archivo descargado "loquesea.conf" a: /etc/wireguard/
4. **Active la VPN** con el comando: sudo wg-quick up eos

En el camino tuve un error que hablaba de un DNS o algo así, lo solucione ejecutando este comando: systemctl start systemd-resolved.service

Para **desactivar la VPN**: sudo wg-quick down eos

> "eos" es el nombre de mi archivo de configuración descargado, este puede tener cualquier nombre en mi caso se llama: eos.conf, pero a la hora de ejecutar el comando debemos omitir la extención ".conf".

Eso es todo, ya tengo la VPN de proton activa en mi Arch Linux.

Referencias:
- [WireGuard.com](https://www.wireguard.com)
- [ProtonVPN.com: How to manually configure WireGuard on Linux](https://protonvpn.com/support/wireguard-linux#cli)