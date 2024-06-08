---
unique-page-id: 2360360
description: Crear un [!DNL Webhook] - Documentos de Marketo - Documentación del producto
title: Crear un [!DNL Webhook]
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
feature: Administration, Webhooks
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# Crear un [!DNL Webhook] {#create-a-webhook}

Uso [!DNL Webhooks] para aprovechar los servicios web de terceros para enviar mensajes de texto, ampliar los datos de personas y mucho más.

>[!AVAILABILITY]
>
>No todos los usuarios de Marketo Engage han adquirido esta funcionalidad. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información.

1. Vaya a la **[!UICONTROL Administrador]** área.

   ![](assets/create-a-webhook-1.png)

1. Clic **[!UICONTROL Webhooks]**.

   ![](assets/create-a-webhook-2.png)

1. Clic **[!UICONTROL Nuevo webhook]**.

   ![](assets/create-a-webhook-3.png)

1. Nombre y configure su [!DNL Webhook].

   ![](assets/create-a-webhook-4.png)

   >[!NOTE]
   >
   >Esto suele incluir la introducción de las credenciales de servicio de terceros como parámetro de URL o en la plantilla de POST.

   * **[!UICONTROL URL]**: introduzca la dirección URL que utiliza en la solicitud al servicio web. Para insertar un token, como la dirección de correo electrónico de la persona (**`{{lead.Email Address}}`**), en su solicitud, haga clic en **[!UICONTROL Insertar token]**.

   * **[!UICONTROL Plantilla]**: Si desea transmitir información en el cuerpo de la solicitud, introduzca a través de la plantilla de carga útil. Plantillas permitidas para los siguientes tipos de solicitud: POST, DELETE, PATCH o PUT. Puede utilizar formatos de datos como JSON o XML. Para insertar un token en la plantilla, haga clic en **[!UICONTROL Insertar token]**.

   * **[!UICONTROL Codificación de token de solicitud]**: Si los valores de token incluyen caracteres especiales (como un signo &amp;), indique el formato de la solicitud (**JSON** o **Formulario/Url**).

   * **[!UICONTROL Tipo de respuesta]**: seleccione el formato de la respuesta que recibe del servicio (**JSON** o **XML**).

   * **[!UICONTROL Tipo de solicitud]**: seleccione el método HTTP que desea utilizar (DELETE, GET, PATCH, POST, PUT).

1. Clic **[!UICONTROL Crear]**.

   ![](assets/create-a-webhook-5.png)

>[!NOTE]
>
>Obtenga más información en la [[!DNL Webhooks]](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/webhooks/webhooks){target="_blank"} buceo profundo.
