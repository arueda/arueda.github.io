---
title: "Publicar en Cloudflare sitio hecho en Hugo"
date: 2023-01-22T14:08:00-08:00
draft: false
---

Error: "/opt/buildhome/repo/themes/ananke/layouts/partials/func/GetFeaturedImage.html:39:1": 
parse failed: template: partials/func/GetFeaturedImage.html:39: function "return" not defined

---

Cloudflare me reportó este error al intentar desplegar mi sitio.
La solución es sencilla: Definir una variable de entorno con la versión de Hugo a utilizar.

En mi caso la versión 110 solucionó mi problema.
`HUGO_VERSION`: 0.110.0


Referencia:
[Cloudflare: Deploy a Hugo Site](https://developers.cloudflare.com/pages/framework-guides/deploy-a-hugo-site/)
