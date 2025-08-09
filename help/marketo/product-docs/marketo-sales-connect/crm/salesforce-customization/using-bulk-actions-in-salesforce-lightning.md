---
unique-page-id: 42762825
description: Uso de acciones masivas en Salesforce Lightning - Documentos de Marketo - Documentación del producto
title: Uso de acciones masivas en Salesforce Lightning
exl-id: 72022507-6568-4cc2-b3b5-c1703a1493ad
feature: Marketo Sales Connect
source-git-commit: fe167b4a70a23f129d56ed20ac6c1ed1130049ef
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# Uso de acciones masivas en [!DNL Salesforce Lightning] {#using-bulk-actions-in-salesforce-lightning}

Aprenda a realizar acciones masivas, como agregar posibles clientes a una campaña, enviar un correo electrónico masivo o transferir posibles clientes de [!DNL Salesforce] a [!DNL Sales Connect].

>[!PREREQUISITES]
>
>Actualice a la última versión del paquete [!DNL Sales Connect] e instale los botones de acción masiva en la vista de posibles clientes o contactos.
>* [Instrucciones en inglés](assets/sf-guide-for-lightning-en.pdf)
>* [Instrucciones en japonés](assets/sf-guide-for-lightning-ja.pdf)

>[!NOTE]
>
>Antes de seguir estos pasos, asegúrese de haber iniciado sesión en su cuenta de [!DNL Marketo Sales Connect].

## Correo electrónico masivo {#bulk-email}

1. En [!DNL Salesforce], haga clic en la ficha **[!UICONTROL Posibles clientes]** y, a continuación, elija la lista de posibles clientes que desee.

   ![](assets/one-6.png)

   >[!NOTE]
   >
   >Si ya está en la lista que va a utilizar, tendrá que volver a ejecutarla seleccionándola en la lista desplegable para asegurarse de que se muestran los botones de acción masiva de MSC. Este es el comportamiento de [!DNL Salesforce] que no se puede cambiar.

1. Haga clic en la lista desplegable de flecha (en el extremo derecho de la pantalla) y seleccione **[!UICONTROL Correo electrónico con MSC]**.

   ![](assets/two-6.png)

1. Aparecerá un correo electrónico de MSC. Incluye las siguientes funciones:

   a. El campo &quot;[!UICONTROL A]&quot; muestra &quot;Todos los recibos&quot;; corresponde a la lista de posibles clientes que ha elegido en la vista de lista de posibles clientes
b. Esta lista está visible en el panel izquierdo llamado &quot;Maquetación masiva&quot;. Puede añadir o quitar destinatarios aquí
c. Puede elegir una plantilla o crear su propio correo electrónico
d. Puede enviar el correo electrónico de inmediato o programar su envío más tarde

   ![](assets/three-5.png)

## Agregar a la campaña {#add-to-campaign}

1. En [!DNL Salesforce], haga clic en la ficha **[!UICONTROL Posibles clientes]** y, a continuación, elija la lista de posibles clientes que desee.

   ![](assets/four-4.png)

1. Haga clic en la lista desplegable de flecha (en el extremo derecho de la pantalla) y seleccione **[!UICONTROL Agregar a MSC Campaign]**.

   ![](assets/five-4.png)

1. Aparecerá la ventana emergente &quot;[!UICONTROL Agregar personas a tu campaña]&quot;. Haga clic en **[!UICONTROL Siguiente]** y siga el flujo de campaña habitual para almacenar en déclencheur una campaña de MSC.

   ![](assets/six-1.png)

## Insertar en [!DNL Marketo Sales Connect] {#push-to-marketo-sales-connect}

1. En [!DNL Salesforce], haga clic en la ficha **[!UICONTROL Posibles clientes]** y, a continuación, elija la lista de posibles clientes que desee.

   ![](assets/seven-2.png)

1. Haga clic en la flecha desplegable (en el extremo derecho de la pantalla) y seleccione **[!UICONTROL Insertar en MSC]**.

   ![](assets/eight-2.png)

1. Se abrirá una nueva pestaña llamada &quot;[!DNL Salesforce] Bridge&quot;. Haga clic en el botón **[!UICONTROL Continuar al grupo] →**.

   ![](assets/nine-2.png)

1. Se le enviará a su cuenta MSC, donde verá un grupo creado con una marca de fecha y hora. Recibirá una notificación cuando se complete la sincronización y el grupo incluirá los posibles clientes sincronizados de [!DNL Salesforce].

   ![](assets/ten-1.png)

>[!NOTE]
>
>Puede seguir los mismos pasos para utilizar acciones masivas también en la Vista de lista de contactos.

>[!MORELIKETHIS]
>
>* [Envío de correos electrónicos por correo electrónico de grupo](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/sending-emails-via-group-email.md)
>* [Componer correos electrónicos en lotes con Seleccionar y Enviar](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md#sending-emails)
