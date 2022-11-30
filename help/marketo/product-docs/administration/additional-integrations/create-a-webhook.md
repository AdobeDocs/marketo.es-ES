---
unique-page-id: 2360360
description: 'Creación de un vínculo web: Documentos de Marketo: Documentación del producto'
title: Creación de un vínculo web
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
source-git-commit: 5f509a7aa27692e54bf129b94c657aff0f645f2b
workflow-type: tm+mt
source-wordcount: '210'
ht-degree: 0%

---

# Creación de un vínculo web {#create-a-webhook}

Utilice los enlaces web para aprovechar los servicios web de terceros para enviar mensajes de texto, expandir datos de personas y mucho más.

>[!AVAILABILITY]
>
>No todos los clientes han adquirido esta funcionalidad. Póngase en contacto con su representante de ventas para obtener más información.

1. Vaya a la **Administrador** .

   ![](assets/create-a-webhook-1.png)

1. Haga clic en **Enlaces web**.

   ![](assets/create-a-webhook-2.png)

1. Haga clic en **Nuevo Weblock**.

   ![](assets/create-a-webhook-3.png)

1. Asigne un nombre al vínculo web y configúrelo.

   ![](assets/create-a-webhook-4.png)

   >[!NOTE]
   >
   >Esto incluye a menudo la introducción de las credenciales del servicio de terceros como parámetro de URL o en la plantilla de POST.

   * **URL**: Introduzca la URL que utiliza en la solicitud al servicio web. Para insertar un token, como la dirección de correo electrónico de la persona (**`{{lead.Email Address}}`**), en la solicitud, haga clic en **Insertar token**.

   * **Plantilla**: Si desea transmitir información en el cuerpo del POST, introduzca la plantilla. Utilice cualquier formato de datos compatible con el POST HTTP, incluidos XML, JSON o SOAP. Para insertar un token en la plantilla, haga clic en **Insertar token**.

   * **Codificación del token de solicitud**: Si los valores de token incluyen caracteres especiales (como el símbolo &amp;), indique el formato de la solicitud (**JSON** o **Formulario/Url**).

   * **Tipo de respuesta**: Seleccione el formato de la respuesta que reciba del servicio (**JSON** o **XML**).

   * **Tipo de solicitud**: Seleccione el método HTTP que desea utilizar (DELETE, GET, PATCH, POST, PUT).

1. Haga clic en **Crear**.

   ![](assets/create-a-webhook-5.png)

>[!NOTE]
>
>Obtenga más información en la [webhooks](https://developers.marketo.com/documentation/webhooks/) buceo profundo.
