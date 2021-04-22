---
unique-page-id: 2360360
description: 'Creación de un vínculo web: Documentos de Marketo: Documentación del producto'
title: Creación de un vínculo web
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 0%

---

# Creación de un enlace web {#create-a-webhook}

Utilice los enlaces web para aprovechar los servicios web de terceros para enviar mensajes de texto, expandir datos de personas y mucho más.

>[!AVAILABILITY]
>
>No todos los clientes han adquirido esta funcionalidad. Póngase en contacto con su representante de ventas para obtener más información.

1. Vaya a **Admin** y haga clic en **Webhooks**.

   ![](assets/image2014-9-24-14-3a52-3a57.png)

1. Haga clic en **Nuevo vínculo web**.

   ![](assets/image2014-9-24-14-3a53-3a9.png)

1. Asigne un nombre al vínculo web y configúrelo.

   ![](assets/image2014-9-24-14-3a53-3a19.png)

   >[!NOTE]
   >
   >Esto incluye a menudo la introducción de las credenciales del servicio de terceros como parámetro de URL o en la plantilla de POST.

   * **URL**: Introduzca la URL que utiliza para almacenar la solicitud en el POST del servicio web. Para insertar un token, como la dirección de correo electrónico de la persona (**`{{lead.Email Address}}`**), en la solicitud, haga clic en **Insertar token**.

   * **Plantilla**: Si desea transmitir información en el cuerpo del POST, introduzca la plantilla. Utilice cualquier formato de datos compatible con el POST HTTP, incluidos XML, JSON o SOAP. Para insertar un token en la plantilla, haga clic en **Insertar token**.

   * **Codificación** del token de solicitud: Si los valores de token incluyen caracteres especiales (como un signo &amp;, &quot;&amp;&quot;), indique el formato de la solicitud (**** JSONo  **Formulario/Url**).

   * **Tipo** de respuesta: Seleccione el formato de la respuesta que recibe del servicio (**** JSONo  **XML**).

   Haga clic en Crear.

   ![](assets/image2014-9-24-14-3a53-3a35.png)

>[!NOTE]
>
>Obtenga más información en el análisis profundo de [webhooks](https://developers.marketo.com/documentation/webhooks/).
