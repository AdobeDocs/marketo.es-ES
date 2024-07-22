---
unique-page-id: 10617431
description: 'Definición de la audiencia de los mensajes en la aplicación: documentos de Marketo, documentación del producto'
title: Establezca La Audiencia De Mensajes En La Aplicación
exl-id: 696ae5b6-7063-41bc-bcef-27879182ff1e
feature: Mobile Marketing
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# Establezca La Audiencia De Mensajes En La Aplicación {#set-your-in-app-message-audience}

El primer paso es decidir quién debe recibir el mensaje en la aplicación. Debe configurar la lista inteligente.

1. Haga clic en **Editar lista inteligente**.

   ![](assets/image2016-5-9-15-3a15-3a7.png)

1. En la lista inteligente, el déclencheur Tiene actividad de aplicación móvil se rellena automáticamente. Haga clic en la lista desplegable y seleccione la aplicación en la que desee colocar el mensaje.

   ![](assets/image2016-5-9-15-3a18-3a10.png)

   >[!NOTE]
   >
   >Actualmente, no se admiten varios valores para el campo Aplicación móvil para programas de mensajes en la aplicación.

1. **Apertura de aplicación** es la configuración de acción predeterminada, pero puede seleccionar cualquier evento personalizado que ya haya configurado.

   ![](assets/image2016-5-9-15-3a20-3a23.png)

   >[!NOTE]
   >
   >El déclencheur predeterminado (Apertura de aplicación) y los déclencheur personalizados que el desarrollador haya agregado al código se muestran automáticamente en el selector de acciones. Si falta un evento personalizado, póngase en contacto con el desarrollador para asegurarse de que ha añadido los eventos personalizados a la aplicación. Tenga en cuenta que el proceso de codificación y aprobación de eventos personalizados puede tardar algún tiempo en completarse. Consulte [este artículo](/help/marketo/product-docs/mobile-marketing/admin/before-you-create-push-notifications-and-in-app-messages.md) para obtener más información.

1. Las restricciones están disponibles para el déclencheur **Tiene actividad de aplicación móvil** si las necesita.

   ![](assets/image2016-5-9-15-3a22-3a27.png)

1. Puede añadir filtros a la lista inteligente para limitar quién recibe el mensaje en la aplicación. En este ejemplo, con el filtro **Fecha de adquisición**, solo las personas adquiridas el 9 de junio de 2016 recibirán el mensaje en la aplicación.

   ![](assets/image2016-5-9-15-3a26-3a2.png)

1. Vuelva al Panel de control de Campaign de mensajes en la aplicación. Defina el límite de visualización en la lista desplegable.

   ![](assets/image2016-5-9-15-3a30-3a35.png)

   >[!NOTE]
   >
   >El límite de visualización predeterminado es **Una vez por sesión**. Si desea que el mensaje deje de mostrarse después de que el destinatario responda, seleccione **Cada vez hasta que se pulse**. Si debería mostrarse cada vez, independientemente de lo que haga el destinatario, elija **Cada vez**.

   ![](assets/image2016-5-9-15-3a32-3a6.png)

¡Buen trabajo! Ya tienes tu audiencia configurada. Ha obtenido la barra azul y la marca de verificación verde.

¡Hora de [seleccionar su mensaje en la aplicación](/help/marketo/product-docs/mobile-marketing/in-app-messages/sending-your-in-app-message/select-your-in-app-message.md)!
