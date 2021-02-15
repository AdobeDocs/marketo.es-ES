---
unique-page-id: 2360360
description: Creación de un Webgancho - Documentos de marketing - Documentación del producto
title: Creación de un enlace web
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 0%

---


# Crear un enlace web {#create-a-webhook}

Utilice los enlaces web para aprovechar los servicios web de terceros para enviar mensajes de texto, ampliar los datos personales y mucho más.

>[!AVAILABILITY]
>
>No todos los clientes han adquirido esta funcionalidad. Póngase en contacto con su representante de ventas para obtener más detalles.

1. Vaya a **Administración** y haga clic en **Webhooks**.

   ![](assets/image2014-9-24-14-3a52-3a57.png)

1. Haga clic en **Nuevo Webgancho**.

   ![](assets/image2014-9-24-14-3a53-3a9.png)

1. Asigne un nombre y configure el vínculo Web.

   ![](assets/image2014-9-24-14-3a53-3a19.png)

   >[!NOTE]
   >
   >Esto incluye a menudo la introducción de las credenciales de servicio de terceros como parámetro de URL o en la plantilla de POST.

   * **Dirección URL**: Introduzca la dirección URL que utiliza para POST de la solicitud al servicio Web. Para insertar un token, como la dirección de correo electrónico de la persona (**`{{lead.Email Address}}`**), en la solicitud, haga clic en **Insertar token**.

   * **Plantilla**: Si desea transmitir información en el cuerpo del POST, introduzca la plantilla. Utilice cualquier formato de datos que admita el POST HTTP, incluidos XML, JSON o SOAP. Para insertar un token en la plantilla, haga clic en **Insertar token**.

   * **Codificación** del token de solicitud: Si los valores del token incluyen caracteres especiales (como un símbolo &amp;, &#39;&amp;&#39;), indique el formato de la solicitud (**** JSONor  **Form/Url**).

   * **Tipo** de respuesta: Seleccione el formato de la respuesta que reciba del servicio (**** JSON o  **XML**).

   Haga clic en Crear.

   ![](assets/image2014-9-24-14-3a53-3a35.png)

>[!NOTE]
>
>Obtenga más información en los [webhooks](https://developers.marketo.com/documentation/webhooks/) buceo profundo.
