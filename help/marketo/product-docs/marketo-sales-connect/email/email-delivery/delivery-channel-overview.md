---
unique-page-id: 14352407
description: 'Resumen del canal de entrega: documentos de Marketo, documentación del producto'
title: Resumen del canal de entrega
exl-id: 432bad1e-4eaf-4be8-b856-be364c44816e
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---

# Resumen del canal de entrega {#delivery-channel-overview}

Marketo Sales Connect le ofrece varias opciones para enviar correos electrónicos. Este artículo revisa los canales de envío que puede aprovechar, cómo seleccionarlos y cuándo elegir uno sobre otro.

## Recomendado: Gmail o Exchange mediante una conexión de correo electrónico {#recommended-gmail-or-exchange-via-email-connection}

Sales Connect permite una configuración optimizada y una capacidad de envío mejorada mediante nuestro servicio de conexión de correo electrónico. La conexión de correo electrónico permite a cada usuario conectarse a su [Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md) o [Exchange](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md) cuenta de a Sales Connect para que se utilice como canal de entrega preferido para todos los correos electrónicos de Sales Connect.

El uso de Gmail o Exchange tiene algunas ventajas destacables sobre otras opciones de canales de envío:

* Se trata de un canal de envío probado con una reputación establecida que ayuda a mantener la capacidad de envío alta.
* Los métodos de autenticación como SPF y DKIM ya están configurados y administrados por su equipo de TI, por lo que no hay ninguna configuración adicional.
* El envío de correos electrónicos dentro de una red de correo electrónico determinada (por ejemplo, enviar un correo electrónico como usuario de Exchange a una empresa que recibe correos electrónicos a través de Exchange) puede ayudar a aumentar aún más la capacidad de envío.

Es importante tener en cuenta que estos canales de envío tienen sus propios límites de envío que aplican Microsoft y Google. Para combatir esto, utilizamos un mecanismo de limitación para ayudar a los usuarios a mantenerse dentro de esos límites. Más información sobre [restricción de correo electrónico aquí](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

>[!NOTE]
>
>De forma predeterminada, el complemento O365 siempre utilizará su canal de entrega de Exchange y el complemento de Gmail siempre utilizará su canal de entrega de Gmail para enviar correos electrónicos desde los complementos.

**Seguimiento de devoluciones**: MSC puede detectar devoluciones para los usuarios de Exchange Online o Gmail detectando el mensaje de devolución enviado a la bandeja de entrada del remitente. Estas notificaciones de rechazo se resumirán en notificaciones de análisis de plantilla, análisis de campaña y fuentes en directo para los usuarios. El seguimiento de devoluciones no es compatible con los clientes locales de Exchange.

## Canal de entrega personalizado a través de SMTP {#custom-delivery-channel-via-smtp}

Sales Connect ofrece la opción adicional de conectar un servidor SMTP de terceros para utilizarlo como el canal de envío preferido de su equipo de ventas.

La utilización de un proveedor SMTP de terceros es una buena opción para los equipos de ventas en los que el volumen de correo electrónico es la prioridad número uno. Los proveedores SMTP como Sendgrid y Sparkpost están optimizados para satisfacer las necesidades de envío masivo de correo electrónico y pueden ampliarse para satisfacer las necesidades de aquellos que buscan implementar grandes volúmenes de correo electrónico.

Además, los proveedores SMTP de terceros ofrecen una plétora de funciones para ayudar a satisfacer las necesidades de envío de su equipo (como informes de envío de correo electrónico y direcciones IP dedicadas), lo que lo convierte en una buena opción para aquellos que buscan controles más granulares y visibilidad alrededor de su canal de envío de correo electrónico de ventas.

## Servidores MSC (heredados) {#msc-servers-legacy}

Los servidores MSC solo están disponibles para algunos clientes heredados de ToutApp. Estos clientes verán los servidores MSC disponibles en su configuración de correo electrónico. Todos los clientes no heredados no verán MSC como una opción y deben conectar su cuenta de Gmail o Outlook a Sales Connect para desbloquear un canal de envío.

Los servidores MSC no admiten los métodos de autenticación DKIM y SPF, lo que puede reducir la tasa de entrega. Debido a esto, recomendamos que todos los clientes se conecten a Gmail o Outlook para obtener la mejor entrega.

## Servidores Marketo {#marketo-servers}

Los servidores de correo electrónico de Marketo no se integran con Sales Connect. Los servidores Marketo están optimizados para la entrega masiva, lo que les permite ampliarse según las necesidades de los especialistas en marketing. Sin embargo, Gmail y Exchange tienen una tasa de éxito más alta para la comunicación de ventas 1:1, por lo que recomendamos utilizar estos servidores para su comunicación de ventas.

>[!MORELIKETHIS]
>
>* [Conexión de correo electrónico para usuarios de Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Conexión de correo electrónico para usuarios de Outlook](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
>* [Configuración de un canal de entrega personalizado](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/setting-up-a-custom-delivery-channel.md)
>* [Restricción de conexión de correo electrónico](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)
