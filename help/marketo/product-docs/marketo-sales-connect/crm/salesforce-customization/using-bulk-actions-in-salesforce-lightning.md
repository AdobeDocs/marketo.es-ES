---
unique-page-id: 42762825
description: Uso de acciones masivas en el rayo de Salesforce - Documentos de marketing - Documentación del producto
title: Uso de acciones masivas en Salesforce Lightning
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---


# Uso de acciones masivas en Salesforce Lightning {#using-bulk-actions-in-salesforce-lightning}

Obtenga información sobre cómo realizar acciones masivas, como agregar leads a una campaña, enviar un correo electrónico masivo o enviar leads desde Salesforce a Sales Connect.

>[!PREREQUISITES]
>
>Actualice a la versión más reciente del paquete de Sales Connect e instale los botones de acción masiva en la vista de posibles clientes/contactos. [Haga clic aquí para obtener instrucciones](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf).

>[!NOTE]
>
>Antes de seguir los pasos que se describen a continuación, asegúrese de haber iniciado sesión en su cuenta de Marketing to Sales Connect.

## Correo electrónico masivo {#bulk-email}

1. En Salesforce, haga clic en la ficha **Posibles clientes** y, a continuación, elija la lista de los leads deseados.

   ![](assets/one-6.png)

   >[!NOTE]
   >
   >Si ya está en la lista que va a usar, tendrá que ejecutarla de nuevo seleccionándola en la lista desplegable para asegurarse de que aparecen los botones de acción masiva de MSC. Es un comportamiento de Salesforce que no se puede cambiar.

1. Haga clic en el menú desplegable de flecha (en el extremo derecho de la pantalla) y seleccione **Correo electrónico con MSC**.

   ![](assets/two-6.png)

1. Aparecerá un mensaje de correo electrónico MSC. Incluye las siguientes funciones:

   a. El campo &quot;Para&quot; muestra &quot;Todos los recibos&quot;: corresponde a la lista de leads que ha elegido en la Vista Lista de posibles clientes\
   b. Esta lista está visible en el panel izquierdo llamado &quot;Composición masiva&quot;: aquí puede agregar o quitar destinatarios\
   c. Puede elegir una plantilla o crear su propio correo electrónico\
   d. Puede enviar el correo inmediatamente o programar el envío más tarde

   ![](assets/three-5.png)

## Añadir a Campaña {#add-to-campaign}

1. En Salesforce, haga clic en la ficha **Posibles clientes** y, a continuación, elija la lista de los leads deseados.

   ![](assets/four-4.png)

1. Haga clic en el menú desplegable de flecha (en el extremo derecho de la pantalla) y seleccione **Añadir a la Campaña de MSC**.

   ![](assets/five-4.png)

1. Aparecerá la ventana emergente &quot;Añadir personas a tu Campaña&quot;. Haga clic en **Siguiente** y vaya a través del flujo de campaña típico para déclencheur de una campaña MSC.

   ![](assets/six-1.png)

## Insertar en MarketingTo Sales Connect {#push-to-marketo-sales-connect}

1. En Salesforce, haga clic en la ficha **Posibles clientes** y, a continuación, elija la lista de los leads deseados.

   ![](assets/seven-2.png)

1. Haga clic en el menú desplegable de flecha (en el extremo derecho de la pantalla) y seleccione **Insertar en MSC**.

   ![](assets/eight-2.png)

1. Se abrirá una nueva ficha llamada &quot;Puente de Salesforce&quot;. Haga clic en el botón **Continuar con el grupo →**.

   ![](assets/nine-2.png)

1. Se le enviará a su cuenta de MSC, donde verá un grupo creado con la marca de fecha y hora. Recibirá una notificación una vez finalizada la sincronización y el grupo incluirá los leads sincronizados desde Salesforce.

   ![](assets/ten-1.png)

>[!NOTE]
>
>También puede seguir los mismos pasos para utilizar acciones masivas en la Vista de Lista de contacto.

>[!MORELIKETHIS]
>
>* [Envío de correos electrónicos a través del correo electrónico del grupo](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/sending-emails-via-group-email.md)
>* [Redacción de correos electrónicos masivos con Seleccionar y enviar](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md#sending-emails)

