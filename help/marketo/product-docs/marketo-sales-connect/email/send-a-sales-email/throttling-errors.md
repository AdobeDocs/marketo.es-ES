---
unique-page-id: 14352581
description: Errores de limitación - Documentos de marketing - Documentación del producto
title: Errores de limitación
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '163'
ht-degree: 0%

---


# Errores de limitación {#throttling-errors}

## Se alcanzó el límite de archivos {#file-limit-reached}

Si envía a través de su propio servidor, tendrá limitaciones para el número de correos electrónicos que puede enviar simultáneamente. Al enviar a través de Sales Connect, puede enviar muchos correos electrónicos, pero intentamos enviarlos todos al mismo tiempo. Así que si sabe que su servidor le va a cortar a 100 correos electrónicos por minuto, sólo tendrá que enviar hasta 100 correos electrónicos a través de la aplicación [](http://toutapp.com/login)web. De lo contrario, los mensajes de correo electrónico pueden aterrizar aquí debido a que los mensajes de correo electrónico están restringidos en el servidor.

## Error de autenticación {#authentication-error}

Esto significa que no hemos podido autenticar la conexión con su servidor SMTP. Lo más probable es que la contraseña haya cambiado recientemente y solo tiene que autenticar sus nuevas credenciales.

Para ello, vaya a la Configuración [SMTP](http://docs.marketo.com/display/docs/assets/external-link-1.jspa) `where you should see the same error message. Update your credentials and hit **Authenticate and Save** to see a confirmation message.`

Ingrese a los Envíos fallidos para intentar reenviar esos correos electrónicos.
