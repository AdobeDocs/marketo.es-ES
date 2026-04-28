---
unique-page-id: 2360360
description: Cree un webhook en Administración para llamar a servicios web de terceros para SMS, datos de personas, etc.
title: Crear  [!DNL Webhook]
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
feature: Administration, Webhooks
source-git-commit: 40f06a5391f2f7263bea0c5b8cefc1f3a607c68c
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 0%

---

# Crear un(a) [!DNL Webhook] {#create-a-webhook}

Use [!DNL Webhooks] para aprovechar los servicios web de terceros y enviar mensajes de texto, expandir datos personales y mucho más.

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/create-a-webhook-1.png)

1. Haga clic en **[!UICONTROL Webhooks]**.

   ![](assets/create-a-webhook-2.png)

1. Haga clic en **[!UICONTROL Nuevo webhook]**.

   ![](assets/create-a-webhook-3.png)

1. Name and configure your [!DNL Webhook].

   ![](assets/create-a-webhook-4.png)

   >[!NOTE]
   >
   >Esto suele incluir la introducción de las credenciales de servicio de terceros como parámetro de URL o en la plantilla POST.

   * **[!UICONTROL URL]**: Escriba la URL que use en su solicitud al servicio web. Para insertar un token, como la dirección de correo electrónico de la persona (**`{{lead.Email Address}}`**), en su solicitud, haga clic en **[!UICONTROL Insertar token]**.

   * **[!UICONTROL Template]**: If you want to transmit information in the body of the request, enter via the payload template. Plantillas permitidas para los siguientes tipos de solicitud: POST, DELETE, PATCH o PUT. You may use data formats such as JSON or XML. Para insertar un token en su plantilla, haga clic en **[!UICONTROL Insertar token]**.

   * **[!UICONTROL Codificación de token de solicitud]**: Si los valores de token incluyen caracteres especiales (como un signo &amp;), indique el formato de su solicitud (**JSON** o **Formulario/URL**).

   * **[!UICONTROL Tipo de respuesta]**: seleccione el formato de la respuesta que recibe del servicio (**JSON** o **XML**).

   * **[!UICONTROL Request Type]**: Select the HTTP method to use (DELETE, GET, PATCH, POST, PUT).

1. Haga clic en **[!UICONTROL Crear]**.

   ![](assets/create-a-webhook-5.png)

>[!NOTE]
>
>Obtenga más información en la profundización de [[!DNL Webhooks]](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/webhooks/webhooks){target="_blank"}.
