---
title: "Website Folder en Webkit"
date: 2023-01-22T10:27:00-08:00
draft: false
---

Corriendo Ejemplos de Bootstrap dentro de una WKWebView usando func url(forResource name: String?, withExtension ext: String?, subdirectory subpath: String?) -> URL?

---

Estoy buscando la manera de implementar [Userbase](https://userbase.com) como metodo de autenticación en una aplicación para iOS.

Para lograrlo, quiero desplegar un modal que muestre una pagina web sencilla que se comunice con el API de Userbase. Nada complicado.

Quiero darle una mejor apariencia a mi pantalla de Login usando los ejemplos de [Bootstrap](https://getbootstrap.com/docs/5.3/examples/sign-in/).

Los ejemplos están autocontenidos y hacen referencia a archivos locales.

`<img class="mb-4" src="../assets/brand/bootstrap-logo.svg" alt="" width="72" height="57">`

En lugar de modificar el ejemplo para apuntar a un servidor remoto, creo que es mejor hacer que la `WKWebView` use el directorio completo para cargar la forma de login.

El código es sencillo:

```
        if let url = Bundle.main.url(forResource: "index",
                                     withExtension: "html",
                                     subdirectory: "LOGIN") {
            loginView.loadFileURL(url, allowingReadAccessTo: url)
        } else {
            print("Unable to load login modal")
        }
```  

La estructura del directorio queda prácticamente intacta:

![Folder Structure](https://imagedelivery.net/d-52onWn5g5i2cEgNkzX3g/449d04df-f473-46aa-b578-da28d65a4700/mobile)

El resultado en el simulador es el esperado.

![Simulator Output](https://imagedelivery.net/d-52onWn5g5i2cEgNkzX3g/ab3ce6fb-e2de-4de0-780f-41b35337cb00/mobile)


Referencias:
-   [urls(forResourcesWithExtension:subdirectory:localization:)](https://developer.apple.com/documentation/foundation/bundle/1414688-urls)
