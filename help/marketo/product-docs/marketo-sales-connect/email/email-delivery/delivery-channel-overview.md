---
unique-page-id: 14352407
description: Información general sobre el Canal de envío - Documentos de marketing - Documentación del producto
title: Información general del Canal de envío
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 0%

---


# Información general del Canal de envío {#delivery-channel-overview}

Desglosaremos los tres canales diferentes que puede aprovechar, cómo seleccionarlos, cuándo seleccionarlos entre sí y los matices que los rodean.

>[!NOTE]
>
>Esta información sólo es relevante si envía sus correos electrónicos desde la [aplicación Web](https://toutapp.com/login). Si utiliza Sales Connect en Gmail o Outlook, los correos electrónicos se enviarán a través de esos servidores de correo electrónico.

## Servidores de correo electrónico MSC (predeterminado) {#msc-email-servers-default}

De forma predeterminada, este método se seleccionará para el envío de los mensajes de correo electrónico. Los servidores de correo electrónico MSC son una opción buena para los usuarios que no utilizan Gmail ni Outlook. Además, como son nuestros servidores, podemos tomar cualquier mensaje de error relacionado con devoluciones o envíos fallidos y mostrarlo en la sección &quot;Envíos fallidos&quot; de la ficha Conversaciones.

Otra ventaja de utilizar los servidores MSC es que, al utilizar una [Identidad de correo electrónico](/help/marketo/product-docs/marketo-sales-connect/getting-started/email-settings/add-identity.md), el destinatario verá la dirección de correo electrónico de la identidad que ha creado.

Al utilizar servidores MSC, es posible que sus destinatarios vean una etiqueta &quot;a través de toutapp.com&quot;. Este es el cliente de correo electrónico que les informa de que el correo electrónico se ha enviado mediante Sales Connect.

Para obtener más información, consulte este [artículo de ayuda de Gmail](https://support.google.com/mail/answer/1311182?hl=en).

>[!NOTE]
>
>Nuestros servidores MSC no tienen un [registro DMARC](https://dmarc.org/) disponible. No se pueden incluir en la lista blanca de sus propios servidores.

## Gmail Server {#gmail-server}

Si el proveedor de correo electrónico de la compañía es Gmail, puede aprovechar la cuenta existente para enviar los correos electrónicos de Sales Connect. Esta es una opción buena si desea evitar la información &quot;a través de toutapp.com&quot; y si prefiere confiar en la reputación del dominio y la capacidad de entrega de su compañía. Una ventaja adicional de usar un servidor de Gmail es que cualquier cosa que envíe desde la aplicación web se agregará automáticamente a la carpeta de Gmail enviada.

Solo podemos conectarnos correctamente con una sola cuenta de Gmail (una dirección de correo electrónico) que envíe sus correos electrónicos de Sales Connect. Esto significa que si utiliza varias identidades de correo electrónico, solo la dirección de la cuenta a la que estamos conectados aparecerá al consultar los detalles.

En la aplicación web, su identidad aparecerá como la creó (arriba). Sin embargo, el envío a través de servidores Gmail mostrará la dirección de la cuenta conectada.

>[!NOTE]
>
>Como Sales Connect no administra directamente los servidores de Gmail, no registramos eventos de correo electrónico devueltos en la aplicación web.

## Servidor SMTP personalizado {#custom-smtp-server}

¿Pagar por su propio servidor? ¿Usar un entorno de Microsoft Exchange? Ésta es una opción para usted. Consulte [estas instrucciones](http://docs.marketo.com/x/zYTS) para obtener información sobre cómo configurar. Al igual que los servidores Gmail, puesto que Sales Connect no administra directamente el servidor, no registramos eventos de correo electrónico devueltos en la aplicación web.
