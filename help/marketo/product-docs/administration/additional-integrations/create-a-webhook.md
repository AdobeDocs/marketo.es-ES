---
unique-page-id: 2360360
description: Cree un webhook en Administración para llamar a servicios web de terceros para SMS, datos de personas, etc.
title: Crear  [!DNL Webhook]
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
feature: Administration, Webhooks
TQID: https://experienceleague.adobe.com/O4xw1wSvFeTJ2xqZn4Eo7JbrUBQQmKcl7mvLkduFXGc
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2: id: fc9b09fe-b844-4544-887b-e420c3b82065
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 220
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

1. Asigne un nombre a su [!DNL Webhook] y configúrelo.

   ![](assets/create-a-webhook-4.png)

   >[!NOTE]
   >
   >Esto suele incluir la introducción de las credenciales de servicio de terceros como parámetro de URL o en la plantilla POST.

   * **[!UICONTROL URL]**: Escriba la URL que use en su solicitud al servicio web. Para insertar un token, como la dirección de correo electrónico de la persona (**`{{lead.Email Address}}`**), en su solicitud, haga clic en **[!UICONTROL Insertar token]**.

   * **[!UICONTROL Plantilla]**: Si desea transmitir información en el cuerpo de la solicitud, ingrese a través de la plantilla de carga útil. Plantillas permitidas para los siguientes tipos de solicitud: POST, DELETE, PATCH o PUT. Puede utilizar formatos de datos como JSON o XML. Para insertar un token en su plantilla, haga clic en **[!UICONTROL Insertar token]**.

   * **[!UICONTROL Codificación de token de solicitud]**: Si los valores de token incluyen caracteres especiales (como un signo &amp;), indique el formato de su solicitud (**JSON** o **Formulario/URL**).

   * **[!UICONTROL Tipo de respuesta]**: seleccione el formato de la respuesta que recibe del servicio (**JSON** o **XML**).

   * **[!UICONTROL Tipo de solicitud]**: seleccione el método HTTP que desea utilizar (DELETE, GET, PATCH, POST, PUT).

1. Haga clic en **[!UICONTROL Crear]**.

   ![](assets/create-a-webhook-5.png)

>[!NOTE]
>
>Obtenga más información en la profundización de [[!DNL Webhooks]](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/webhooks/webhooks){target="_blank"}.
