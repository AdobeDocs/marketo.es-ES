---
description: Notificación - Conexión De Websocket - Documentos De Marketo - Documentación Del Producto
title: Notificación - Conexión de Websocket
hide: true
hidefromtoc: true
exl-id: 00c754f8-3850-4209-803d-5cdb108dc6dc
source-git-commit: eb3e7983f7521d025dff1f5d79b8caeaeb0f622c
workflow-type: tm+mt
source-wordcount: '114'
ht-degree: 0%

---

# Notificación: Conexión de Websocket {#notification-websocket-connection}

Este documento es para usuarios de Marketo Engage que recibieron la siguiente notificación en su instancia de Marketo: `"We were unable to establish a websocket connection to <some-server.adobe.net>. We are ending support of the servers you are currently connected to. Please work with your IT Team to allowlist required Marketo Engage and Adobe domains and ports to prevent access disruptions."`

Si usted o su organización utilizan una configuración restrictiva del servidor de seguridad o del servidor proxy, es posible que usted o el administrador de la red tengan que realizar una lista de permitidos de ciertos dominios e intervalos de direcciones IP para garantizar que Adobe Marketo Engage funciona según lo esperado.

La compatibilidad con Marketo no está configurada para ayudar a implementar los protocolos siguientes. Si necesita ayuda, comparta este documento con su equipo de TI. Si restringen el acceso a la web mediante una lista de permitidos, pídale que agregue los siguientes dominios (incluido el asterisco) para permitir todos los recursos y sockets web de Marketo:

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`
