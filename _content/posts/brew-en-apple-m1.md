---
title: "Homebrew en Apple M1"
date: 2022-02-25T07:54:47-08:00
draft: false
---

Error:  

*Cannot install in Homebrew on ARM processor in Intel default prefix*

Solución: Ejecutar la instalación por defecto para que el script se encargue de poner home brew en la carpeta correcta.  

`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`

---

Hace poco cambié mi MacBook Air Intel por una M1. Me interesaba conocer el desempeño de los nuevos procesadores y corroborar el ahorro de energía.

Este post no es para hablar de los beneficios o desventajas de los nuevos equipos Apple. Más bien quiero documentar algo que ocurrió al querer instalar [Hugo](https://gohugo.io) mediante [Homebrew](https://brew.sh)

Solicité a Homebrew la instalación de Hugo:
`brew install hugo`

Inmediatamente recibí el siguiente mensaje de error:

> Error: Cannot install in Homebrew on ARM processor in Intel default prefix (/usr/local)!  
> Please create a new installation in /opt/homebrew using one of the  
> "Alternative Installs" from:  
>  https://docs.brew.sh/Installation  
> You can migrate your previously installed formula list with:  
>  brew bundle dump 

La nueva mac es una clon de la anterior, restauré la información usando las herramientas de Mac OS y homebrew quedó configurado de la misma manera. El detalle es que las Mac con M1 necesitan que homebrew quede instalado en otro folder.

La solución fue instalar brew de nuevo tal como se muestra en la pagina de inicio:  

`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`

Adicionalmente realicé la migración de mi instalación anterior ejecutando:
`brew bundle dump`

Puse brew en el path siguiendo las instrucciones sugeridas.
Instalé Hugo.  

`brew install hugo`

Éxito:
> 🍺  /opt/homebrew/Cellar/hugo/0.92.2: 48 files, 54.3MB
