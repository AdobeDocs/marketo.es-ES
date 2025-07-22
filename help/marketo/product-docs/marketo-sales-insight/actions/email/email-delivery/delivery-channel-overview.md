---
description: 'Resumen del canal de entrega: documentos de Marketo, documentación del producto'
title: Resumen del canal de entrega
exl-id: 8dd6fe3e-86ae-4361-bc0a-6488dc1df9fa
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 0%

---

# Resumen del canal de entrega {#delivery-channel-overview}

Marketo Sales le ofrece varias opciones para enviar correos electrónicos. Este artículo revisa los canales de envío que puede aprovechar, cómo seleccionarlos y cuándo elegir uno sobre otro.

## Recomendado: Gmail o Exchange mediante una conexión de correo electrónico {#recommended-gmail-or-exchange-via-email-connection}

Marketo Sales permite una configuración optimizada y una capacidad de envío mejorada a través de nuestro servicio de conexión de correo electrónico. La conexión de correo electrónico permite a cada usuario conectarse a su cuenta de [Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md) o [[!DNL Exchange]](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md) con Marketo Sales para utilizarla como el canal de entrega elegido para todos los correos electrónicos de Marketo Sales.

El uso de Gmail o [!DNL Exchange] presenta algunas ventajas distintas con respecto a otras opciones de canales de envío:

* Se trata de un canal de envío probado con una reputación establecida que ayuda a mantener la capacidad de envío alta.
* Los métodos de autenticación como SPF y DKIM ya están configurados y administrados por su equipo de TI, por lo que no hay ninguna configuración adicional.
* El envío de correos electrónicos dentro de una red de correo electrónico determinada (por ejemplo, el envío de un correo electrónico como usuario de [!DNL Exchange] a una compañía que recibe correos electrónicos a través de [!DNL Exchange]) puede ayudar a aumentar aún más la capacidad de envío.

Es importante tener en cuenta que estos canales de envío tienen sus propios límites de envío, que Microsoft y Google aplican. Para combatir esto, utilizamos un mecanismo de limitación para ayudar a los usuarios a mantenerse dentro de esos límites. Obtenga más información acerca de la limitación de [correo electrónico aquí](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

>[!NOTE]
>
>De forma predeterminada, el complemento O365 siempre utilizará su canal de entrega de Exchange y el complemento de Gmail siempre utilizará su canal de entrega de Gmail para enviar correos electrónicos desde los complementos.

**Seguimiento de devoluciones**: Marketo Sales puede detectar devoluciones para usuarios de Exchange Online o Gmail detectando el mensaje de devolución enviado a la bandeja de entrada del remitente. Estas notificaciones de rechazo se resumirán en notificaciones de análisis de plantilla, análisis de campaña y fuentes en directo para los usuarios. El seguimiento de devoluciones no es compatible con los clientes locales de Exchange.

## Canal de entrega personalizado a través de SMTP {#custom-delivery-channel-via-smtp}

Marketo Sales ofrece la opción adicional de conectar un servidor SMTP de terceros para utilizarlo como canal de envío preferido de su equipo de ventas.

La utilización de un proveedor SMTP de terceros es una excelente opción para los equipos de ventas en los que el volumen de correo electrónico es la prioridad número uno. Los proveedores SMTP como Sendgrid y Sparkpost están optimizados para satisfacer las necesidades de envío masivo de correo electrónico y pueden ampliarse para satisfacer las necesidades de aquellos que buscan implementar grandes volúmenes de correo electrónico.

Además, los proveedores SMTP de terceros ofrecen una plétora de funciones para ayudar a satisfacer las necesidades de envío de su equipo (como informes de envío de correo electrónico y direcciones IP dedicadas), lo que lo convierte en una excelente opción para aquellos que buscan controles más granulares y visibilidad alrededor de su canal de envío de correo electrónico de ventas.

## Servidores de ventas Marketo (heredados) {#marketo-sales-servers-legacy}

Los servidores de ventas de Marketo solo están disponibles para algunos clientes heredados de ToutApp. Estos clientes verán los servidores de ventas de Marketo disponibles en su configuración de correo electrónico. Todos los clientes que no sean clientes heredados no verán Marketo Sales como una opción y deberán conectar su cuenta de Gmail o [!DNL Outlook] a Marketo Sales para desbloquear un canal de entrega.

Los servidores de ventas de Marketo no admiten los métodos de autenticación DKIM y SPF, lo que puede reducir la tasa de entrega. Debido a esto, recomendamos que todos los clientes se conecten a Gmail o [!DNL Outlook] para obtener la mejor entrega.

## Servidores MSC (heredados) {#msc-servers-legacy}

Los servidores MSC solo están disponibles para algunos clientes heredados de ToutApp. Estos clientes verán los servidores MSC disponibles en su configuración de correo electrónico. Todos los clientes no heredados no verán MSC como una opción y deben conectar su cuenta de Gmail o Outlook a Sales Connect para desbloquear un canal de envío.

Los servidores MSC no admiten los métodos de autenticación DKIM y SPF, lo que puede reducir la tasa de entrega. Debido a esto, recomendamos que todos los clientes se conecten a Gmail o [!DNL Outlook] para obtener la mejor entrega.

## Servidores Marketo {#marketo-servers}

Los servidores de correo electrónico de Marketo no se integran con Marketo Sales. Los servidores Marketo están optimizados para la entrega masiva, lo que les permite ampliarse según las necesidades de los especialistas en marketing. Sin embargo, Gmail y [!DNL Exchange] tienen una tasa de éxito mayor para la comunicación de ventas de 1:1, por lo que recomendamos utilizar estos servidores para la comunicación de ventas.

>[!MORELIKETHIS]
>
>* [Conexión de correo electrónico para usuarios de Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Conexión de correo electrónico para [!DNL Outlook] Usuarios](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
>* [Configuración de un canal de entrega personalizado](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/setting-up-a-custom-delivery-channel.md)
>* [Restricción de conexión de correo electrónico](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)
