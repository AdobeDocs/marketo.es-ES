---
unique-page-id: 42762825
description: Uso de acciones masivas en Salesforce Lightning - Documentos de Marketo - Documentación del producto
title: Uso de acciones masivas en Salesforce Lightning
exl-id: 72022507-6568-4cc2-b3b5-c1703a1493ad
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Uso de acciones masivas en Salesforce Lightning {#using-bulk-actions-in-salesforce-lightning}

Aprenda a realizar acciones masivas, como añadir posibles clientes a una campaña, enviar un correo electrónico masivo o transferir posibles clientes de Salesforce a Sales Connect.

>[!PREREQUISITES]
>
>Actualice a la última versión del paquete de Sales Connect e instale los botones de acción por lotes en la vista de cliente potencial/contacto. [Haga clic aquí para obtener instrucciones](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf).

>[!NOTE]
>
>Antes de seguir estos pasos, asegúrese de haber iniciado sesión en su cuenta de Marketo Sales Connect.

## Correo electrónico masivo {#bulk-email}

1. En Salesforce, haga clic en **Posibles clientes** y, a continuación, elija la lista de posibles clientes que desee.

   ![](assets/one-6.png)

   >[!NOTE]
   >
   >Si ya está en la lista que va a utilizar, tendrá que volver a ejecutarla seleccionándola en la lista desplegable para asegurarse de que se muestran los botones de acción masiva de MSC. Este es un comportamiento de Salesforce que no se puede cambiar.

1. Haga clic en la lista desplegable de flecha (en el extremo derecho de la pantalla) y seleccione **Correo electrónico con MSC**.

   ![](assets/two-6.png)

1. Aparecerá un correo electrónico de MSC. Incluye las siguientes funciones:

   a. El campo &quot;A&quot; muestra &quot;Todos los recibos&quot;; corresponde a la lista de posibles clientes que ha elegido en la vista de lista de posibles clientes\
   b. Esta lista está visible en el panel izquierdo llamado &quot;Maquetación masiva&quot;. Puede añadir o quitar destinatarios aquí\
   c. Puede elegir una plantilla o crear su propio correo electrónico\
   d. Puede enviar el correo electrónico de inmediato o programar su envío más tarde

   ![](assets/three-5.png)

## Agregar a la campaña  {#add-to-campaign}

1. En Salesforce, haga clic en **Posibles clientes** y, a continuación, elija la lista de posibles clientes que desee.

   ![](assets/four-4.png)

1. Haga clic en la lista desplegable de flecha (en el extremo derecho de la pantalla) y seleccione **Añadir a la campaña de MSC**.

   ![](assets/five-4.png)

1. Aparecerá la ventana emergente &quot;Agregar personas a su campaña&quot;. Clic **Siguiente** y siga el flujo de campaña típico para almacenar en déclencheur una campaña de MSC.

   ![](assets/six-1.png)

## Insertar en Marketo Sales Connect {#push-to-marketo-sales-connect}

1. En Salesforce, haga clic en **Posibles clientes** y, a continuación, elija la lista de posibles clientes que desee.

   ![](assets/seven-2.png)

1. Haga clic en la lista desplegable de flecha (en el extremo derecho de la pantalla) y seleccione **Insertar en MSC**.

   ![](assets/eight-2.png)

1. Se abrirá una nueva pestaña llamada &quot;Salesforce Bridge&quot;. Haga clic en **Pasar al → de grupo** botón.

   ![](assets/nine-2.png)

1. Se le enviará a su cuenta MSC, donde verá un grupo creado con una marca de fecha y hora. Recibirá una notificación una vez que se complete la sincronización y el grupo incluirá los posibles clientes sincronizados desde Salesforce.

   ![](assets/ten-1.png)

>[!NOTE]
>
>Puede seguir los mismos pasos para utilizar acciones masivas también en la Vista de lista de contactos.

>[!MORELIKETHIS]
>
>* [Envío de correos electrónicos mediante correo electrónico de grupo](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/sending-emails-via-group-email.md)
>* [Redacción de correos electrónicos masivos con selección y envío](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md#sending-emails)
