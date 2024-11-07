---
layout: note
title: "Elimina el bloatware de tu Android sin ser root"
date: 2022-01-07
---

Elimina las Apps que trae tu android "por defecto" sin root. Esto gracias a una herramienta que utilizan los desarrolladores.

Acabas de comprar un terminal Android y al encenderlo te das cuenta que viene con muchas aplicaciones que tu no vas a utilizar nunca. Este conjunto de aplicaciones que vienen pre-instaladas es conocido como **"bloatware"**.

**Razones por las que los usuarios de Android desean eliminar el bloatware de su terminal:**
- Consume memoria que se podría aprovechar mejor.
- Vuelve el dispositivo lento innecesariamente.
- Buscan ahorrar espacio con menos actualizaciones.

**Ventajas de eliminar el bloatware de tu dispositivo:**
- Ahorra espacio en tu dispositivo.
- Te evita hacer actualizaciones de aplicaciones que no utilizas.
- Se agiliza tu dispositivo al disminuir el uso de memoria RAM.

## Pasos para eliminar el bloatware de tu dispositivo Android sin root

### Paso 1. Habilitar la Depuración USB en nuestro Android

Para habilitar la **Depuración por USB** primero deberemos de habilitar las **Opciones de Desarrollador** para ello iremos a Ajustes → Acerca del teléfono y dar 5 taps hasta que nos salga un aviso de que las **Opciones de Desarrollador** ya han sido habilitadas.

### Paso 2. Descargar las herramientas SDK de Android

Puedes descargar estas herramientas en la pagina oficial, [developer.android.com](https://developer.android.com/studio/releases/platform-tools).
Lo siguiente sera descomprimir el archivo descargado y mover la carpeta que nos quedo en el directorio raíz de nuestro disco duro.

### Paso 3. Eliminar apps innecesarias

1. Primero, activa la depuración USB del teléfono y conéctalo al ordenador.
2. Ahora, abre una ventana de comandos **CMD** en el ordenador.
3. Para comprobar que el teléfono se ha conectado correctamente, ejecuta el comando `adb devices`. Debe aparecer el número identificativo del dispositivo en la ventana de comandos.
4. En el ordenador, introduce la instrucción `adb shell`.
5. Para eliminar una aplicación en concreto, introduce el comando `pm uninstall -k --user 0 nombredelpaquete`. Por ejemplo `pm uninstall -k --user 0 com.samsung.calculator`.
6. Repite el paso anterior con todas las apps que quieras desinstalar.

> Nota: Puedes apoyarte de la aplicación App Inspector para identificar el nombre del paquete de la app que deseas desinstalar.