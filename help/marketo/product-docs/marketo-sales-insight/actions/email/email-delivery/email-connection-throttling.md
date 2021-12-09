---
description: 'Restricción de la conexión de correo electrónico: Documentos de Marketo: Documentación del producto'
title: Restricción de conexión de correo electrónico
hide: true
hidefromtoc: true
exl-id: 02450a1e-5b30-4057-b204-19fab1a7d6c9
source-git-commit: fda1bf51d4016a61c41be9acba4771db1797a552
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# Restricción de conexión de correo electrónico {#email-connection-throttling}

La integración de la cuenta de Sales Connect para enviar a través de los proveedores de correo electrónico de Exchange o Gmail ofrece una configuración optimizada y optimiza la capacidad de envío de correo electrónico para la comunicación de ventas 1:1. Sin embargo, para mantener los sistemas en buen estado y las cuentas seguras, Gmail y Exchange aplican límites de envío de correo electrónico. These limits are open to be increased or decreased at the providers&#39; discretion.

## Email Connection Throttling (Beta) {#email-connection-throttling-beta}

>[!AVAILABILITY]
>
>Esta función se encuentra actualmente en la versión beta. To join this Beta, please contact your Customer Success Manager.

La limitación de la conexión de correo electrónico permite a los administradores de Conexión de ventas configurar la tasa de envío de correos electrónicos al utilizar Gmail o Exchange como canal de envío, de modo que la tasa a la que se entregan los correos electrónicos al proveedor de canales de envío no supere los límites impuestos.

Cuando se exceden los límites de forma consistente, a veces se puede considerar que el proveedor de canales de envío tiene un comportamiento sospechoso, lo que provoca que los correos electrónicos fallen y, a veces, incluso que se deshabilite una cuenta.

**Notas/Puntos destacados**

* Se habilita automáticamente una vez que un usuario se conecta a Gmail o Exchange
* Se puede personalizar si desea aumentar o reducir la configuración de la recomendación para satisfacer sus necesidades
* Solo restringe los correos electrónicos enviados a través de Gmail o Exchange, no restringe el canal de envío personalizado
* The Email Connection throttling queues up each individual users emails separately as each user has their own connection with their email provider

**Configuración de la restricción de conexión de correo electrónico**

1. Haga clic en el icono del engranaje y seleccione **Configuración**.

   ![](assets/email-connection-throttling-1.png)

1. Under Admin Settings, click **General**.

   ![](assets/email-connection-throttling-2.png)

1. In the Email Connection Throttling card on the right, click the **Enable Email Throttling** slider.

   ![](assets/email-connection-throttling-3.png)

1. In the Email Connection Throttling card on the right, enter the desired batch size of emails that will be sent over to the email channel provider.

   ![](assets/email-connection-throttling-4.png)

1. Establezca la cantidad de tiempo de espera antes de enviar cada lote. En este ejemplo elegimos 25 correos electrónicos cada 45 segundos.

   ![](assets/email-connection-throttling-5.png)

1. Haga clic en **Guardar**.

   ![](assets/email-connection-throttling-6.png)

Con los cambios guardados, todos los usuarios tendrán que enviar sus correos electrónicos en lotes a su cuenta de Gmail o Exchange conectada para su envío.

## Límites del proveedor de correo electrónico {#email-provider-limits}

**Outlook 365**

Empresa/Empresa

* 10,000 per day
* 30 por minuto
* 500 destinatarios por correo electrónico

Más información [se puede encontrar aquí](https://docs.microsoft.com/en-us/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#RecipientLimits).

**Gmail**

* 2.000 por día (500 para juicios y cuentas marcadas)
* 2 correos electrónicos por segundo (límite de API)
* 2000 destinatarios por mensaje (un máximo de 500 para destinatarios externos)

Más información [se puede encontrar aquí](https://support.google.com/a/answer/166852?hl=en).

**Microsoft Exchange Server (2010, 2013)**

El departamento de TI de la organización establece límites, ya que el servidor está alojado por la organización. Contact the network or system admin as applicable for additional information.

>[!MORELIKETHIS]
>
>* [Descripción general del canal de entrega](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/delivery-channel-overview.md)
>* [Email Connection for Gmail Users](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Email Connection for Outlook Users](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)

