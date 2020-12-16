---
unique-page-id: 2360360
description: Creación de un Webgancho - Documentos de marketing - Documentación del producto
title: Creación de un enlace web
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 0%

---


# Creación de un enlace web {#create-a-webhook}

Utilice los enlaces web para aprovechar los servicios web de terceros para enviar mensajes de texto, ampliar los datos personales y mucho más.

>[!NOTE]
>
>**Disponibilidad**
>
>No todos los clientes han adquirido esta funcionalidad. Póngase en contacto con su representante de ventas para obtener más detalles.

1. Vaya a **Administración **y haga clic en **Webhooks**.

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

   * **Codificación** del token de solicitud: Si los valores del token incluyen caracteres especiales (como un símbolo &amp;, &#39;&amp;&#39;), indique el formato de la solicitud (**JSON** o **Formulario/Url**).

   * **Tipo** de respuesta: Seleccione el formato de la respuesta que reciba del servicio (**JSON** o **XML**).

   Haga clic en Crear.

   ![](assets/image2014-9-24-14-3a53-3a35.png)

>[!NOTE]
>
>**Buceo profundo**
>
>Aprenda más en el [webhooks](http://developers.marketo.com/documentation/webhooks/) de buceo profundo.

