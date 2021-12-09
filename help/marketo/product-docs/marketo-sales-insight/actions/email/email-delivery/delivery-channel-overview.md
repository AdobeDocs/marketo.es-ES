---
description: 'Descripción general del canal de entrega: Documentos de Marketo: Documentación del producto'
title: Descripción general del canal de entrega
hide: true
hidefromtoc: true
exl-id: 8dd6fe3e-86ae-4361-bc0a-6488dc1df9fa
source-git-commit: fda1bf51d4016a61c41be9acba4771db1797a552
workflow-type: tm+mt
source-wordcount: '668'
ht-degree: 0%

---

# Descripción general del canal de entrega {#delivery-channel-overview}

Marketo Sales le ofrece varias opciones para enviar correos electrónicos. Este artículo revisará los canales de envío que puede aprovechar, cómo seleccionarlos y cuándo seleccionarlos entre sí.

## Recomendado: Gmail o Exchange mediante conexión de correo electrónico {#recommended-gmail-or-exchange-via-email-connection}

Marketo Sales permite una configuración optimizada y una capacidad de envío mejorada a través de nuestro servicio de conexión de correo electrónico. La conexión de correo electrónico permite a cada usuario conectarse a su [Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md) o [Exchange](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md) cuenta a Marketo Sales para utilizarla como el canal de entrega elegido para todos los correos electrónicos de ventas de Marketo.

La utilización de Gmail o Exchange ofrece algunas ventajas distintas con respecto a otras opciones de canal de envío:

* Se trata de un canal de envío probado con una reputación establecida que ayuda a mantener la capacidad de envío alta.
* Los métodos de autenticación, como SPF y DKIM, ya están configurados y administrados por su equipo de TI, por lo que no hay configuración adicional.
* El envío de correos electrónicos dentro de una red de correo electrónico determinada (es decir, el envío de un correo electrónico como usuario de Exchange a una empresa que recibe correos electrónicos a través de Exchange) puede ayudar a aumentar aún más la capacidad de envío.

Es importante tener en cuenta que estos canales de envío tienen sus propios límites de envío, que Microsoft y Google aplican. Para combatir esto, utilizamos un mecanismo de regulación para ayudar a los usuarios a permanecer dentro de esos límites. Más información sobre [restricción de correo electrónico aquí](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

>[!NOTE]
>
>De forma predeterminada, el complemento O365 siempre utilizará su canal de entrega de intercambio y el complemento Gmail utilizará siempre su canal de entrega de Gmail para enviar correos electrónicos desde los complementos.

**Seguimiento de devoluciones**: Marketo Sales puede detectar devoluciones para usuarios de Exchange Online o Gmail detectando el mensaje de rechazo que se envía a la bandeja de entrada del remitente. Estas notificaciones de devoluciones se resumirán en notificaciones de análisis de plantillas, análisis de campaña y fuente activa para los usuarios. El seguimiento de devoluciones no es compatible con los clientes locales de Exchange.

## Canal de entrega personalizado a través de SMTP {#custom-delivery-channel-via-smtp}

Marketo Sales ofrece la opción adicional de conectar un servidor SMTP de terceros para utilizarlo como canal de envío preferido del equipo de ventas.

La utilización de un proveedor SMTP de terceros es una buena opción para los equipos de ventas en los que el volumen de correo electrónico es la prioridad número uno. Los proveedores SMTP, como Sendgrid y Sparkpost, están optimizados para satisfacer las necesidades de envío masivo de correo electrónico y pueden escalar para satisfacer las necesidades de aquellos que buscan implementar grandes volúmenes de correo electrónico.

Además, los proveedores SMTP de terceros ofrecen una gran cantidad de funciones que ayudan a satisfacer las necesidades de envío de su equipo (como los informes de envío de correo electrónico y las direcciones IP dedicadas), lo que convierte esta opción en una buena opción para aquellos que buscan controles y visibilidad más granulares en torno a su canal de envío de correo electrónico de ventas.

## Servidores de ventas de Marketo (heredados) {#marketo-sales-servers-legacy}

Los servidores de ventas de Marketo solo están disponibles para algunos clientes de ToutApp heredados. Estos clientes verán los servidores de ventas de Marketo disponibles en su configuración de correo electrónico. Todos los clientes no heredados no verán las ventas de Marketo como una opción y deben conectar su cuenta de Gmail o Outlook a las ventas de Marketo para desbloquear un canal de envío.

Los servidores de ventas de Marketo no admiten métodos de autenticación DKIM y SPF, lo que puede reducir la tasa de entrega. Debido a esto, recomendamos que todos los clientes se conecten a Gmail o Outlook para obtener la mejor capacidad de envío.

## Servidores MSC (heredados) {#msc-servers-legacy}

Los servidores MSC solo están disponibles para algunos clientes de ToutApp heredados. Estos clientes verán los servidores MSC disponibles en su configuración de correo electrónico. Todos los clientes no heredados no verán MSC como una opción y deben conectar su cuenta de Gmail o Outlook a Sales Connect para desbloquear un canal de envío.

Los servidores MSC no admiten métodos de autenticación DKIM y SPF, lo que puede reducir la tasa de entrega. Debido a esto, recomendamos que todos los clientes se conecten a Gmail o Outlook para obtener la mejor capacidad de envío.

## Servidores Marketo {#marketo-servers}

Los servidores de correo electrónico de Marketo no se integran con las ventas de Marketo. Los servidores de Marketo están optimizados para su envío masivo y permiten escalar según las necesidades de los especialistas en marketing. Sin embargo, Gmail y Exchange tienen una tasa de éxito más alta para la comunicación de ventas 1:1, por lo que recomendamos utilizar estos servidores para su comunicación de ventas.

>[!MORELIKETHIS]
>
>* [Conexión de correo electrónico para usuarios de Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Conexión de correo electrónico para usuarios de Outlook](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
>* [Configuración de un canal de envío personalizado](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/setting-up-a-custom-delivery-channel.md)
>* [Restricción de conexión de correo electrónico](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)

