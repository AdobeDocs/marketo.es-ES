---
unique-page-id: 4720710
description: Aprenda a configurar SPF y DKIM en su DNS para mejorar la capacidad de envío de correo electrónico. Autorice a Marketo para enviar mensajes en su nombre y reduzca los indicadores de correo no deseado.
title: Configuración de SPF y DKIM para la entregabilidad de correo electrónico
exl-id: a0f88e94-3348-4f48-bbd2-963e2af93dc0
feature: Deliverability
TQID: https://experienceleague.adobe.com/ZZvIOz7gmqXEht3xw1Pj1tabkQqjvGokF0BgOjdNzjs
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 434
ht-degree: 89%

---

# Configuración de SPF y DKIM para la entregabilidad de correo electrónico {#set-up-spf-and-dkim-for-your-email-deliverability}

Un método rápido para mejorar sus tasas de entrega de correo electrónico es incorporar **SPF** (Marco de directivas de remitente) y **DKIM** en su configuración de DNS. Con esta adición a las entradas DNS, está diciendo a los destinatarios que ha autorizado a Marketo a enviar correos electrónicos en su nombre. Sin este cambio, su correo electrónico tiene mayor probabilidad de ser marcado como spam, ya que el correo electrónico se envió desde su dominio, pero desde una dirección IP con un dominio de Marketo.

>[!CAUTION]
>
>Necesitará que su administrador de red realice este cambio en el registro DNS.

## Configurar SPF {#set-up-spf}

**Si NO TIENE un registro SPF en su dominio**

Pida al administrador de red que añada la línea siguiente a las entradas de DNS. Sustituya [domain] por el dominio principal de su sitio web (por ejemplo: “company.com”) y [corpIP] con la dirección IP de su servidor de correo electrónico corporativo (por ejemplo, &quot;255.255.255.255&quot;). Si envía correos electrónicos desde varios dominios a través de Marketo, debe añadirlos a cada dominio (en una línea).

`[domain] IN TXT v=spf1 mx ip4:[corpIP] include:mktomail.com ~all`

**Si TIENE un registro SPF en su dominio**

Si ya tiene un registro SPF existente en la entrada de DNS, añádale lo siguiente:

include:mktomail.com

## Configurar DKIM {#set-up-dkim}

**¿Qué es DKIM? ¿Por qué me interesa configurar DKIM?**

DKIM es un protocolo de autenticación que utilizan los receptores de correo electrónico para determinar si un mensaje de correo electrónico fue enviado por quien dice que lo ha enviado. DKIM suele mejorar la entregabilidad de correos electrónicos a la bandeja de entrada, ya que el receptor puede estar seguro de que el mensaje no es una falsificación.

**¿Cómo funciona DKIM?**

Después de configurar la clave pública en su registro DNS y de activar el dominio de envío en la sección de administración (A), activaremos la firma DKIM personalizada para sus mensajes salientes, que incluirá una firma digital cifrada con cada correo electrónico que enviemos por usted (B). Los receptores podrán descifrar la firma digital consultando la “clave pública” en el DNS (C) del dominio de envío. Si la clave del correo electrónico se corresponde con la clave del registro DNS, es más probable que el servidor receptor de correo acepte el correo electrónico que envía Marketo en su nombre.

![](assets/image2015-1-12-13-3a56-3a55.png)

**¿Cómo configuro DKIM?**

Consulte [Configurar una firma DKIM personalizada](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* Más información acerca de SPF y su funcionamiento`: http://www.open-spf.org/Introduction/`
>* ¿Está configurado correctamente mi SPF?: `https://www.kitterman.com/spf/validate.html`
>* ¿He utilizado la sintaxis correcta?: `http://www.open-spf.org/SPF_Record_Syntax/`
