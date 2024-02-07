---
description: Notificación - Conexión De Websocket - Documentos De Marketo - Documentación Del Producto
title: Notificación - Conexión de Websocket
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: 94afeacfdecf71e6985daccc31dd67e3d19953ac
workflow-type: tm+mt
source-wordcount: '114'
ht-degree: 0%

---

# Notificación: Conexión de Websocket {#notification-websocket-connection}

Este artículo es para usuarios de Marketo Engage que recibieron la siguiente notificación en su instancia de Marketo: `"We were unable to establish a websocket connection to <some-server.adobe.net>. We are ending support of the servers you are connected to now on March 3, 2024. Please work with your IT team to allowlist required Marketo Engage and Adobe domains and ports to prevent access disruptions."`

Si usted o su organización utilizan una configuración restrictiva del servidor de seguridad o del servidor proxy, es posible que usted o el administrador de la red tengan que realizar una lista de permitidos de ciertos dominios e intervalos de direcciones IP para garantizar que Adobe Marketo Engage funciona según lo esperado.

La compatibilidad con Marketo no está configurada para ayudar a implementar los protocolos siguientes. Si necesita ayuda, comparta este artículo con su equipo de TI. Si restringen el acceso a la web mediante una lista de permitidos, pídale que agregue los siguientes dominios (incluido el asterisco) para permitir todos los recursos y sockets web de Marketo:

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`
