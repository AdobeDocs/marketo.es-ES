---
unique-page-id: 4720710
description: Configure SPF y DKIM para su capacidad de entrega por correo electrónico - Documentos de marketing - Documentación del producto
title: Configure SPF y DKIM para su capacidad de entrega por correo electrónico
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 0%

---


# Configure SPF y DKIM para su capacidad de entrega por correo electrónico {#set-up-spf-and-dkim-for-your-email-deliverability}

Un método rápido para mejorar las tasas de envío de correo electrónico es incorporar **SPF** (Entorno de directivas de remitentes) y **DKIM** (Correo identificado con claves de dominio) en la configuración de DNS. Con esta adición a sus entradas DNS, le está diciendo a los destinatarios que ha autorizado a Marketing a enviar correos electrónicos en su nombre. Sin este cambio, el correo electrónico tiene una mayor probabilidad de ser marcado como correo no deseado, ya que el correo electrónico se dirigió desde su dominio, pero se envió desde una dirección IP con un dominio de marketing.

>[!CAUTION]
>
>Necesitará el administrador de red para realizar este cambio en el registro DNS.

## Configurar SPF {#set-up-spf}

**Si NO tiene un registro SPF en su dominio**

Pida al administrador de red que agregue la línea siguiente a sus entradas DNS. Reemplazar [dominio] por el dominio principal de su sitio web (por ejemplo: &quot;compañía.com&quot;) y [corpIP] con la dirección IP de su servidor de correo electrónico corporativo (por ejemplo: &quot;255.255.255.255&quot;). Si envía correos electrónicos desde varios dominios a través de Marketing, debe agregarlos a cada dominio (en una línea).
[dominio] EN TXT v=spf1 mx ip4:[corpIP] include:mktomail.com ~all\
Si NO tiene un registro SPF en su dominio

Si ya tiene un registro SPF en la entrada DNS, agregue lo siguiente:

include:mktomail.com

## Configurar DKIM {#set-up-dkim}

### ¿Qué es DKIM? ¿Por qué quiero configurar DKIM? {#what-is-dkim-why-do-i-want-to-set-up-dkim}

DKIM es un protocolo de autenticación que utilizan los receptores de correo electrónico para determinar si un mensaje de correo electrónico ha sido enviado por quien dice que fue enviado. DKIM a menudo mejora la entrega de correos electrónicos a la bandeja de entrada, ya que un receptor puede estar seguro de que el mensaje no es una falsificación.

¿Cómo actúa DKIM?

Después de configurar la clave pública en el registro DNS y activar el dominio de envío en la sección Administración (A), activaremos la firma DKIM personalizada para sus mensajes salientes, que incluirá una firma digital cifrada con cada correo electrónico que enviemos por usted (B). Los receptores podrán descifrar la firma digital buscando la &quot;clave pública&quot; en el DNS (C) de su dominio de envío. Si la clave del correo electrónico corresponde con la clave del registro DNS, es más probable que el servidor de correo receptor acepte el mensaje de correo electrónico de marketing enviado en su nombre.

![](assets/image2015-1-12-13-3a56-3a55.png)

¿Cómo configuro DKIM?

Consulte [Configuración de una firma](set-up-a-custom-dkim-signature.md)DKIM personalizada.

>[!MORELIKETHIS]
>
>* [Más información sobre SPF y cómo funciona](http://www.open-spf.org/Introduction/)
>* [Herramientas de entrega de correo electrónico del comerciante](https://www.marketo.com/software/email-marketing/email-deliverability/)
>* [¿Mi SPF está configurado correctamente?](http://www.kitterman.com/spf/validate.html)
>* [¿He usado la sintaxis correcta?](http://www.open-spf.org/SPF_Record_Syntax/)

>



