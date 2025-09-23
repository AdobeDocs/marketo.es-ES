---
unique-page-id: 14352407
description: 'Resumen del canal de entrega: documentos de Marketo, documentación del producto'
title: Información general sobre el canal de entrega
exl-id: 432bad1e-4eaf-4be8-b856-be364c44816e
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 1%

---

# Información general sobre el canal de entrega {#delivery-channel-overview}

Marketo [!DNL Sales Connect] le ofrece varias opciones para enviar correos electrónicos. Este artículo revisa los canales de envío que puede aprovechar, cómo seleccionarlos y cuándo elegir uno sobre otro.

## Recomendado: Gmail o [!DNL Exchange] mediante conexión de correo electrónico {#recommended-gmail-or-exchange-via-email-connection}

[!DNL Sales Connect] permite una configuración optimizada y una capacidad de envío mejorada a través de nuestro servicio de conexión de correo electrónico. La [!UICONTROL conexión de correo electrónico] permite que cada usuario se conecte a su cuenta de [Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md) o [Exchange](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md) a [!DNL Sales Connect] para que se utilice como el canal de entrega elegido para todos los correos electrónicos de [!DNL Sales Connect].

El uso de Gmail o [!DNL Exchange] presenta algunas ventajas distintas con respecto a otras opciones de canales de envío:

* Se trata de un canal de envío probado con una reputación establecida que ayuda a mantener la capacidad de envío alta.
* Los métodos de autenticación como SPF y DKIM ya están configurados y administrados por su equipo de TI, por lo que no hay ninguna configuración adicional.
* El envío de correos electrónicos dentro de una red de correo electrónico determinada (por ejemplo, el envío de un correo electrónico como usuario de [!DNL Exchange] a una compañía que recibe correos electrónicos a través de [!DNL Exchange]) puede ayudar a aumentar aún más la capacidad de envío.

Es importante tener en cuenta que estos canales de envío tienen sus propios límites de envío, que Microsoft y Google aplican. Para combatir esto, utilizamos un mecanismo de limitación para ayudar a los usuarios a mantenerse dentro de esos límites. Obtenga más información acerca de la limitación de [correo electrónico aquí](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

>[!NOTE]
>
>De forma predeterminada, el complemento O365 siempre utilizará su canal de entrega de Exchange y el complemento de Gmail siempre utilizará su canal de entrega de Gmail para enviar correos electrónicos desde los complementos.

**Seguimiento de devoluciones**: MSC puede detectar devoluciones para [!DNL Exchange Online] o usuarios de Gmail al detectar el mensaje de devolución que se envía a la bandeja de entrada del remitente. Estas notificaciones de rechazo se resumirán en notificaciones de análisis de plantilla, análisis de campaña y fuentes en directo para los usuarios. No se admite el seguimiento de devoluciones para [!DNL Exchange] clientes locales.

## Canal de entrega personalizado a través de SMTP {#custom-delivery-channel-via-smtp}

[!DNL Sales Connect] ofrece la opción adicional de conectar un servidor SMTP de terceros para utilizarlo como el canal de entrega preferido de su equipo de ventas.

La utilización de un proveedor SMTP de terceros es una excelente opción para los equipos de ventas en los que el volumen de correo electrónico es la prioridad número uno. Los proveedores SMTP como [!DNL Sendgrid] y [!DNL Sparkpost] están optimizados para satisfacer las necesidades de envío masivo de correo electrónico y se pueden escalar para satisfacer las necesidades de aquellos que buscan implementar grandes volúmenes de correo electrónico.

Además, los proveedores SMTP de terceros ofrecen una plétora de funciones para ayudar a satisfacer las necesidades de envío de su equipo (como informes de envío de correo electrónico y direcciones IP dedicadas), lo que lo convierte en una excelente opción para aquellos que buscan controles más granulares y visibilidad alrededor de su canal de envío de correo electrónico de ventas.

## Servidores MSC (heredados) {#msc-servers-legacy}

Los servidores MSC solo están disponibles para algunos clientes heredados de ToutApp. Estos clientes verán los servidores MSC disponibles en su configuración de correo electrónico. Todos los clientes no heredados no verán MSC como una opción y deben conectar su cuenta de Gmail o [!DNL Outlook] a [!DNL Sales Connect] para desbloquear un canal de entrega.

Los servidores MSC no admiten los métodos de autenticación DKIM y SPF, lo que puede reducir la tasa de entrega. Debido a esto, recomendamos que todos los clientes se conecten a Gmail o [!DNL Outlook] para obtener la mejor entrega.

## Servidores Marketo {#marketo-servers}

Los servidores de correo electrónico de Marketo no se integran con [!DNL Sales Connect]. Los servidores Marketo están optimizados para la entrega masiva, lo que les permite ampliarse según las necesidades de los especialistas en marketing. Sin embargo, Gmail y [!DNL Exchange] tienen una tasa de éxito mayor para la comunicación de ventas de 1:1, por lo que recomendamos utilizar estos servidores para la comunicación de ventas.

>[!MORELIKETHIS]
>
>* [Conexión de correo electrónico para usuarios de Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Conexión de correo electrónico para [!DNL Outlook] Usuarios](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
>* [Configuración de un canal de entrega personalizado](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/setting-up-a-custom-delivery-channel.md)
>* [Restricción de conexión de correo electrónico](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)
