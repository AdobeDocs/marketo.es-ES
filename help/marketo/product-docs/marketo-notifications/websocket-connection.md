---
description: Detalles de notificación para los usuarios de Marketo Engage que recibieron la notificación No se pudo establecer una conexión con Websocket
title: Notificación - Conexión de Websocket
hide: true
exl-id: 00c754f8-3850-4209-803d-5cdb108dc6dc
TQID: https://experienceleague.adobe.com/NpcRnxQPi03CF8z77Urrfs2P2phkuRbh2pd5J1UquFk
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 123
ht-degree: 30%

---

# Notificación: conexión de Websocket {#notification-websocket-connection}

Este documento es para usuarios de Marketo Engage que recibieron la siguiente notificación en su instancia de Marketo: `"We were unable to establish a websocket connection to <some-server.adobe.net>. We are ending support of the servers you are currently connected to. Please work with your IT Team to allowlist required Marketo Engage and Adobe domains and ports to prevent access disruptions."`

Si usted o su organización utilizan una configuración restrictiva del servidor de seguridad o del servidor proxy, es posible que usted o el administrador de la red tengan que realizar una lista de permitidos de ciertos dominios e intervalos de direcciones IP para garantizar que Adobe Marketo Engage funciona según lo esperado.

La compatibilidad con Marketo no está configurada para ayudar a implementar los protocolos siguientes. Si necesita ayuda, comparta este documento con su equipo de TI. Si restringen el acceso a la web mediante una lista de permitidos, pídale que agregue los siguientes dominios (incluido el asterisco) para permitir todos los recursos y sockets web de Marketo:

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`
