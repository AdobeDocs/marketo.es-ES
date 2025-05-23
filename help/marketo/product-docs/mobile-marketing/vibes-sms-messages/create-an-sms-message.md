---
description: 'Creación de un mensaje SMS: documentos de Marketo, documentación del producto'
title: Creación de un mensaje SMS
feature: Mobile Marketing
exl-id: 94749ea4-2fe3-4d90-9b31-35700ddd1670
source-git-commit: dae00c6877e638ae60305122f3f3e17b3c922e10
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# Creación de un mensaje SMS {#create-an-sms-message}

A continuación se muestra cómo crear un mensaje SMS.

>[!AVAILABILITY]
>
>Esta función está disponible como complemento para su cuenta de Adobe Marketo Engage. Para que se pueda aprovisionar correctamente, debe adquirirse a través del Adobe. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información. La integración nativa de Marketo Vibes SMS está disponible en Estados Unidos y Canadá. Para otros países, se puede utilizar una conexión a través de Webhooks de Marketo poniéndose en contacto directamente con Vibes[&#128279;](https://www.vibes.com/talk-to-sales).

>[!PREREQUISITES]
>
>[Agregar vibraciones como servicio de LaunchPoint](/help/marketo/product-docs/mobile-marketing/admin/add-vibes-as-a-launchpoint-service.md){target="_blank"}

1. Vaya a **[!UICONTROL Actividades de marketing]**.

   ![](assets/create-an-sms-message-1.png)

1. Haga clic con el botón derecho en el programa deseado y seleccione **[!UICONTROL Nuevo recurso local]**.

   ![](assets/create-an-sms-message-2.png)

1. Seleccionar **mensaje SMS**.

   ![](assets/create-an-sms-message-3.png)

1. Escriba un nombre y una descripción opcional para el nuevo mensaje SMS y haga clic en **Crear**.

   ![](assets/create-an-sms-message-4.png)

1. En el editor, haga clic dentro de la burbuja azul y empiece a introducir texto.

   ![](assets/create-an-sms-message-5.png)

   >[!NOTE]
   >
   >El límite de caracteres de un mensaje SMS es de 160 caracteres con el conjunto de caracteres ASCII estándar. Si supera los 160 caracteres, el mensaje se dividirá en función del recuento total de caracteres.

1. Para agregar un token a tu mensaje, escribe un saludo rápido y haz clic en **Token**.

   ![](assets/create-an-sms-message-6.png)

   >[!NOTE]
   >
   >Si se añade un token, el mensaje puede superar el límite de caracteres. A continuación, el mensaje se dividiría, lo que crearía un mensaje adicional.

   >[!IMPORTANT]
   >
   >Cumplimiento de SMS: todos los mensajes SMS salientes deben incluir el nombre de la marca o la descripción del programa. Las instrucciones HELP y STOP deben proporcionarse al menos una vez al mes por suscriptor para programas de mensajes recurrentes.

1. Seleccione el **token** deseado, escriba un **valor predeterminado** opcional y haga clic en **Crear**.

   ![](assets/create-an-sms-message-7.png)

1. Para agregar un vínculo, selecciona en qué parte del mensaje deseas que aparezca y haz clic en **Vínculo**.

   ![](assets/create-an-sms-message-8.png)

1. Seleccione un tipo de vínculo. La página de aterrizaje de Marketo es la predeterminada. Si va con él, haga clic en el menú desplegable Landing Page y seleccione la página deseada. Haga clic en **Insertar** cuando haya terminado.

   ![](assets/create-an-sms-message-9.png)

   >[!NOTE]
   >
   >Los dos vínculos de seguimiento están seleccionados de forma predeterminada. Desmarcar solo Incluir mkt_tok seguirá permitiendo el seguimiento del vínculo, pero después de redireccionar, la URL de destino no incluirá el parámetro de cadena de consulta mkt_tok. Este parámetro lo utilizan las páginas de aterrizaje de Marketo y Munchkin para garantizar un seguimiento adecuado de las actividades de la persona (como cuando una persona decide excluirse).

1. Si desea usar una dirección URL externa en su lugar, seleccione **Dirección URL externa**, ingrese/pegue la dirección URL y haga clic en **Insertar**.

   ![](assets/create-an-sms-message-10.png)

   >[!NOTE]
   >
   >Si se mantiene seleccionada la opción &quot;Rastrear vínculo&quot;, Marketo modifica automáticamente la dirección URL con fines de seguimiento. Si opta por deshabilitar el seguimiento, la dirección URL se mostrará en el mensaje sin cambios (por ejemplo, `www.adobe.com`).

   >[!CAUTION]
   >
   >Se recomienda _no_ usar acortadores de URL (por ejemplo, Bitly), ya que los operadores pueden marcar su mensaje como correo no deseado.

1. El vínculo se muestra en el mensaje.

   ![](assets/create-an-sms-message-11.png)

   >[!NOTE]
   >
   >Marketo muestra una vista previa de vínculo del dominio de seguimiento marcado. Si desactiva la casilla de verificación del vínculo mkt_tok, se cambia el vínculo.

Si inserta más de 160 caracteres, el editor divide el SMS en secciones. Hay un límite general de 900 caracteres por mensaje. Si supera ese límite, el mensaje se truncará tras la entrega.
