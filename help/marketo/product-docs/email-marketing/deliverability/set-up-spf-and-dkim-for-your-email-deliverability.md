---
unique-page-id: 4720710
description: 'Configuración de SPF y DKIM para su capacidad de entrega por correo electrónico: Marketo Docs: documentación del producto'
title: Configuración de SPF y DKIM para su capacidad de entrega por correo electrónico
exl-id: a0f88e94-3348-4f48-bbd2-963e2af93dc0
source-git-commit: de32becbfe74c2a88c53de8af8be4ee022782114
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# Configuración de SPF y DKIM para su capacidad de entrega por correo electrónico {#set-up-spf-and-dkim-for-your-email-deliverability}

Un método rápido para mejorar las tasas de envío de correo electrónico es incorporar **SPF** (Marco de Política del Remitente) y **DKIM** (Correo identificado de claves de dominio) en la configuración DNS. Con esta adición a las entradas DNS, se indica a los destinatarios que ha autorizado a Marketo a enviar correos electrónicos en su nombre. Sin este cambio, su correo electrónico tiene una mayor probabilidad de ser marcado como correo no deseado, ya que el correo electrónico fue dirigido desde su dominio, pero enviado desde una dirección IP con un dominio de Marketo.

>[!CAUTION]
>
>Necesitará su administrador de red para realizar este cambio en su registro DNS.

## Configuración de SPF {#set-up-spf}

**Si NO tiene un registro SPF en su dominio**

Solicite al administrador de red que agregue la línea siguiente a sus entradas DNS. Reemplazar [domain] con el dominio principal de su sitio web (por ejemplo, &quot;company.com&quot;) y [corpIP] con la dirección IP de su servidor de correo electrónico corporativo (por ejemplo, &quot;255.255.255.255&quot;). Si envía correos electrónicos de varios dominios a través de Marketo, debe agregarlos a cada dominio (en una línea).

`[domain] IN TXT v=spf1 mx ip4:[corpIP] include:mktomail.com ~all`

**Si NO tiene un registro SPF en su dominio**

Si ya tiene un registro SPF en la entrada DNS, agregue lo siguiente:

include:mktomail.com

## Configuración de DKIM {#set-up-dkim}

**¿Qué es DKIM? ¿Por qué quiero configurar DKIM?**

DKIM es un protocolo de autenticación que utilizan los receptores de correo electrónico para determinar si un mensaje de correo electrónico fue enviado por el que dice que lo enviaron. A menudo, DKIM mejora la entrega de correos electrónicos a la bandeja de entrada, ya que un receptor puede estar seguro de que el mensaje no es una falsificación.

**¿Cómo actúa DKIM?**

Después de configurar la clave pública en el registro DNS y activar el dominio de envío en la sección de administración (A), activaremos la firma DKIM personalizada para sus mensajes salientes, que incluirá una firma digital cifrada con cada correo electrónico que enviemos por usted (B). Los receptores podrán descifrar la firma digital buscando la &quot;clave pública&quot; en el DNS (C) de su dominio de envío. Si la clave del correo electrónico corresponde a la clave del registro DNS, es más probable que el servidor de correo receptor acepte el correo electrónico que Marketo envió en su nombre.

![](assets/image2015-1-12-13-3a56-3a55.png)

**¿Cómo configuro DKIM?**

Consulte [Configuración de una firma DKIM personalizada](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md).

>[!MORELIKETHIS]
>
>* [Más información sobre SPF y cómo funciona](http://www.open-spf.org/Introduction/)
>* [Herramientas de entrega de correo electrónico de Marketo](https://www.marketo.com/software/email-marketing/email-deliverability/)
>* [¿Mi SPF está configurado correctamente?](https://www.kitterman.com/spf/validate.html)
>* [¿He usado la sintaxis correcta?](http://www.open-spf.org/SPF_Record_Syntax/)

