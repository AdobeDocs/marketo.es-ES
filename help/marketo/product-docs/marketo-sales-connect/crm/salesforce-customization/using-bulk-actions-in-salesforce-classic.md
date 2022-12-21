---
unique-page-id: 42762794
description: Uso de acciones masivas en Salesforce Classic - Marketo Docs - Documentación del producto
title: Uso de acciones masivas en Salesforce Classic
exl-id: f676ba65-6bc9-41e5-aa70-0f10bceedab7
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# Uso de acciones masivas en Salesforce Classic {#using-bulk-actions-in-salesforce-classic}

Aprenda a realizar acciones masivas, como agregar posibles clientes a una campaña, enviar un correo electrónico masivo o enviar posibles clientes desde Salesforce a Sales Connect.

>[!PREREQUISITES]
>
>Actualice a la última versión del paquete de conexión de ventas e instale los botones de acción masiva en la vista de contacto/posible cliente. [Haga clic aquí para obtener instrucciones](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf).

>[!NOTE]
>
>Antes de seguir los pasos descritos, asegúrese de haber iniciado sesión en su cuenta de Marketo Sales Connect.

## Correo electrónico masivo {#bulk-email}

1. En Salesforce, haga clic en la **Posibles clientes** y, a continuación, la pestaña **Ir** botón.

   ![](assets/one-5.png)

1. Elija los posibles clientes que desee y haga clic en la **Correo electrónico con MSC (Classic)** botón.

   ![](assets/two-5.png)

1. Aparecerá un correo electrónico MSC. Incluye las siguientes funciones:

   a. El campo &quot;A&quot; muestra &quot;Todas las recepciones&quot;, que corresponde a la lista de posibles clientes que ha elegido en la vista de la lista de posibles clientes\
   b. Esta lista está visible en el panel izquierdo llamado &quot;Composición masiva&quot; : aquí puede añadir o eliminar destinatarios\
   c. Puede elegir una plantilla o crear su propio correo electrónico\
   d. Puede obtener una vista previa de los campos dinámicos que se rellenarán en el correo electrónico\
   e. Puede enviar el correo electrónico inmediatamente o programarlo para enviarlo más tarde

   ![](assets/three-4.png)

## Agregar a la campaña  {#add-to-campaign}

1. En Salesforce, haga clic en la **Posibles clientes** y, a continuación, la pestaña **Ir** botón.

   ![](assets/four-3.png)

1. Elija los posibles clientes que desee y haga clic en la **Agregar a MSC Campaign (Classic)** botón.

   ![](assets/five-3.png)

1. Aparecerá la ventana emergente &quot;Añadir personas a la campaña&quot;. Haga clic en **Siguiente** y revise el flujo de campaña típico para almacenar en déclencheur una campaña de MSC.

   ![](assets/six.png)

## Insertar en Marketo Sales Connect {#push-to-marketo-sales-connect}

1. En Salesforce, haga clic en la **Posibles clientes** y, a continuación, la pestaña **Ir** botón.

   ![](assets/seven-1.png)

1. Elija los posibles clientes que desee y haga clic en la **Insertar en MSC (Classic)** botón.

   ![](assets/eight-1.png)

1. Se abrirá una nueva pestaña denominada &quot;Salesforce Bridge&quot;. Haga clic en el **Continúe con Grupo →** botón.

   ![](assets/nine-1.png)

1. Se le enviará a su cuenta de MSC, donde verá un grupo creado con una marca de fecha y hora. Recibirá una notificación una vez finalizada la sincronización y el grupo incluirá los posibles clientes sincronizados con Salesforce.

   ![](assets/ten.png)

>[!NOTE]
>
>También puede seguir los mismos pasos para utilizar acciones masivas en la Vista de lista de contactos.

>[!MORELIKETHIS]
>
>* [Envío de correos electrónicos a través del correo electrónico del grupo](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/sending-emails-via-group-email.md)
>* [Redacción de correos electrónicos masivos con Select y Send](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md#sending-emails)

