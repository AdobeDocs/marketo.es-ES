---
unique-page-id: 14352581
description: Errores de limitación - Documentos de marketing - Documentación del producto
title: Errores de limitación
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---


# Errores de limitación {#throttling-errors}

## Límite de archivos alcanzado {#file-limit-reached}

Si envía a través de su propio servidor, tendrá limitaciones para el número de correos electrónicos que puede enviar simultáneamente. Al enviar a través de Sales Connect, puede enviar muchos correos electrónicos, pero intentamos enviarlos todos al mismo tiempo. Si sabe que su servidor va a cortarle 100 correos electrónicos por minuto, sólo tendrá que enviar hasta 100 correos electrónicos a través de la [aplicación Web](https://toutapp.com/login). De lo contrario, los mensajes de correo electrónico pueden aterrizar aquí debido a que los mensajes de correo electrónico están restringidos en el servidor.

## Error de autenticación {#authentication-error}

Esto significa que no hemos podido autenticar la conexión con su servidor SMTP. Lo más probable es que la contraseña haya cambiado recientemente y solo tiene que autenticar sus nuevas credenciales.

Para ello, vaya a la Configuración SMTP, donde debería ver el mismo mensaje de error. Actualice sus credenciales y pulse **Autenticar y Guardar** para ver un mensaje de confirmación.

Ingrese a los Envíos fallidos para intentar reenviar esos correos electrónicos.
