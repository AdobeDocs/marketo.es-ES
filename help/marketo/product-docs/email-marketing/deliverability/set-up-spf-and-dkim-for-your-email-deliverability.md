---
unique-page-id: 4720710
description: 'Configuración de SPF y DKIM para la entrega de correo electrónico: Documentos de Marketo: documentación del producto'
title: Configuración de SPF y DKIM para la entregabilidad de correo electrónico
exl-id: a0f88e94-3348-4f48-bbd2-963e2af93dc0
feature: Deliverability
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 4%

---

# Configuración de SPF y DKIM para la entregabilidad de correo electrónico {#set-up-spf-and-dkim-for-your-email-deliverability}

Un método rápido para mejorar tus tasas de entrega de correo electrónico es incorporar **SPF** (Marco de Política del Remitente) y **DKIM** (Domain Keys Identified Mail) en tu configuración de DNS. Con esta adición a las entradas DNS, está diciendo a los destinatarios que ha autorizado a Marketo a enviar correos electrónicos en su nombre. Sin este cambio, su correo electrónico tiene una mayor probabilidad de ser marcado como correo no deseado, ya que el correo electrónico se envió desde su dominio, pero desde una dirección IP con un dominio de Marketo.

>[!CAUTION]
>
>Necesitará al administrador de red para realizar este cambio en el registro DNS.

## Configuración de SPF {#set-up-spf}

**Si NO tiene un registro SPF en su dominio**

Pida al administrador de red que agregue la línea siguiente a las entradas DNS. Reemplace [domain] por el dominio principal de su sitio web (por ejemplo: &quot;company.com&quot;) y [corpIP] con la dirección IP de su servidor de correo electrónico corporativo (por ejemplo, &quot;255.255.255.255&quot;) Si envía correos electrónicos desde varios dominios a través de Marketo, debe agregarlos a cada dominio (en una línea).

`[domain] IN TXT v=spf1 mx ip4:[corpIP] include:mktomail.com ~all`

**Si NO tiene un registro SPF en su dominio**

Si ya tiene un registro SPF en la entrada DNS, agréguele lo siguiente:

include:mktomail.com

## Configuración de DKIM {#set-up-dkim}

**¿Qué es DKIM? ¿Por qué deseo configurar DKIM?**

DKIM es un protocolo de autenticación que utilizan los receptores de correo electrónico para determinar si un mensaje de correo electrónico fue enviado por quién dice que lo envió. DKIM suele mejorar la capacidad de entrega de correos electrónicos a la bandeja de entrada, ya que un destinatario puede estar seguro de que el mensaje no es una falsificación.

**¿Cómo funciona DKIM?**

Después de configurar la clave pública en su registro DNS y activar el dominio de envío en la sección Admin (A), activaremos la firma personalizada de DKIM para sus mensajes salientes, que incluirá una firma digital cifrada con cada correo electrónico que enviemos por usted (B). Los receptores podrán descifrar la firma digital buscando la &quot;clave pública&quot; en el DNS (C) del dominio de envío. Si la clave del correo electrónico corresponde a la clave del registro DNS, es más probable que el servidor de correo receptor acepte el correo electrónico que Marketo envió en su nombre.

![](assets/image2015-1-12-13-3a56-3a55.png)

**¿Cómo configuro DKIM?**

Consulte [Configurar una firma personalizada de DKIM](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* Más información acerca de SPF y su funcionamiento`: http://www.open-spf.org/Introduction/`
>* ¿Está configurado correctamente mi SPF?: `https://www.kitterman.com/spf/validate.html`
>* ¿He utilizado la sintaxis correcta?: `http://www.open-spf.org/SPF_Record_Syntax/`
