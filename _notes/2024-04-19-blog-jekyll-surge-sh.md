---
layout: note
title: "Crear un blog con Jekyll y montarlo en Surge.sh"
author: Jesús Peralta
date: 2024-04-19
tags: programacion
---

## Instalar Surge.

1. Instalar las dependencias node.js y npm.

```bash
sudo pacman -S nodejs npm
```

1. Instalar surge.

```bash
sudo npm install --global surge
```

## Instalar Jekyll.

1. Instalar ruby.

```bash
sudo pacman -S ruby
```

1. Instalar jekyll.

```bash
gem install jekyll bundler

```

1. Añadir directorio de gemas al PATH (añadir a .bashrc).

```bash
export PATH=/home/jpz/.local/share/gem/ruby/3.0.0/bin:$PATH
```

## Crear el blog.

1. Crear directorio del proyecto.

```bash
jekyll new jpztec.surge.sh
```

1. Configurar gema "webrick".

```bash
cd jpztec.surge.sh
nano Gemfile
# Añadir linea:
gem "webrick"
# Cerrar y guardar (Ctrl+S)
```

1. Instalar gemas del proyecto

```bash
bundle install

```

1. Compilar el blog y ejecutar el servidor local.

```bash
bundle exec jekyll serve
```

o

```bash
bundle exec jekyll serve --livereload # Para ver en tiempo real los cambios.
```

## Ver blog (local).

Entrar desde el navegador a: **localhost:4000**

## Subir el blog a [surge.sh](http://surge.sh/)

1. Construir sitio (generar HTML, CSS, etc...).

```bash
bundle exec jekyll build
```

1. Subir blog generado ubicado en "_site" a [surge.sh](http://surge.sh/).

```bash
surge _site
# Iniciar sesión o registrarse en surge.sh y subir.
```

## Referencias

- [Surge.sh - Getting started with Surge](https://surge.sh/help/getting-started-with-surge).
- [Surge.sh - Deploying a Jekyll project](https://surge.sh/help/deploying-a-jekyll-project).
- [Jekyllrb.com - Quickstart](https://jekyllrb.com/docs/).
- [Jekyllrb.com - Command Line Usage](https://jekyllrb.com/docs/usage/).
- [Jekyllrb.com - Rendering Process](https://jekyllrb.com/docs/rendering-process/).