---
unique-page-id: 10098759
description: 'Comprobación de anuncios de posibles clientes de Facebook para la integración móvil con Marketo: Marketo Docs: Documentación del producto'
title: Comprobación de anuncios de posibles clientes de Facebook para la integración móvil con Marketo
exl-id: 0c381c53-f97a-4e1d-b44d-5ee6521ac990
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# Comprobación de anuncios de posibles clientes de Facebook para la integración móvil con Marketo {#test-facebook-lead-ads-for-mobile-integration-with-marketo}

Después de crear la publicidad de posible cliente, debe probarla.

>[!PREREQUISITES]
>
>Debe [Configuración de la integración de Facebook Lead Ads](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md).

1. En Facebook Power Editor, seleccione una campaña, una publicidad y haga clic en **Editar**.

1. En **Vínculos**, haga clic en **Ver en aplicación móvil** vínculo.

   ![](assets/image2016-5-13-15-3a2-3a38.png)

1. Se enviará una nueva notificación a la cuenta de Facebook a la que podrá acceder desde el dispositivo móvil con la cuenta autorizada. Haga clic en **OK**.

   ![](assets/image2016-3-11-8-3a35-3a7.png)

1. En el dispositivo móvil, pulse **Notificaciones** en la aplicación móvil de Facebook.

   ![](assets/image2016-3-11-8-3a38-3a35.png)

1. En Notificaciones, pulse **Su publicidad está lista para la vista previa**.

   ![](assets/image2016-3-11-8-3a41-3a59.png)

1. Envíe la unidad de prueba de Lead Ad tocando su Llamada a acción y rellenando el formulario que ha creado.

   ![](assets/image2016-3-11-8-3a52-3a20.png)

   >[!NOTE]
   >
   >Este es solo un ejemplo, que utiliza una Llamada a acción Más información . Puede que la llamada a acción de la unidad de publicidad de posibles clientes sea diferente.

1. ¡Aquí es donde sucede la magia! Una vez enviado el formulario, [crear una lista inteligente en Marketo](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) como parte de un programa o en la base de datos de posibles clientes que usa la variable **Formulario de anuncios de posibles clientes de Facebook rellenado** filtro. Inserte el Nombre del formulario de publicidad de posibles clientes del formulario que acaba de enviar.

   ![](assets/image2016-3-11-8-3a59-3a34.png)

1. A continuación, haga clic en la pestaña Posibles clientes para validar que la sincronización funciona correctamente.

   ![](assets/image2016-3-11-15-3a27-3a54.png)

¿Eso es genial o qué?

>[!NOTE]
>
>[Habilitar/deshabilitar los anuncios de posibles clientes de Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)
