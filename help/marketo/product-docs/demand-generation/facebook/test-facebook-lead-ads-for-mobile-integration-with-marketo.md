---
unique-page-id: 10098759
description: Obtenga información sobre cómo probar la integración móvil de Facebook Lead Ads con Marketo. Verifique correctamente los envíos de anuncios de posibles clientes desde la sincronización móvil.
title: Prueba de anuncios de clientes potenciales de Facebook para la integración móvil con Marketo
exl-id: 0c381c53-f97a-4e1d-b44d-5ee6521ac990
feature: Integrations
source-git-commit: d20c398cd1f5ed2646f56995c35a57630c3f2e95
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 4%

---

# Probar [!DNL Facebook] anuncios de posibles clientes para la integración móvil con Marketo {#test-facebook-lead-ads-for-mobile-integration-with-marketo}

Después de crear el anuncio de posible cliente, debe probarlo.

>[!PREREQUISITES]
>
>Debe [configurar la integración de [!UICONTROL Anuncios destacados de Facebook]](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md).

1. En [!UICONTROL Facebook Power Editor], seleccione una campaña y un anuncio y haga clic en **[!UICONTROL Editar]**.

1. En **[!UICONTROL Vínculos]**, haga clic en el vínculo **[!UICONTROL Ver en aplicación móvil]**.

   ![](assets/image2016-5-13-15-3a2-3a38.png)

1. Se enviará una nueva notificación a la cuenta de [!DNL Facebook] a la que podrá acceder desde el dispositivo móvil con la cuenta autorizada. Haga clic en **[!UICONTROL Aceptar]**.

   ![](assets/image2016-3-11-8-3a35-3a7.png)

1. En tu dispositivo móvil, pulsa **[!UICONTROL Notificaciones]** en la aplicación móvil [!DNL Facebook].

   ![](assets/image2016-3-11-8-3a38-3a35.png)

1. En Notificaciones, pulsa **[!UICONTROL Tu anuncio está listo para la vista previa]**.

   ![](assets/image2016-3-11-8-3a41-3a59.png)

1. Envíe su prueba de unidad de publicidad de posibles clientes tocando su Call to action y rellenando el formulario que ha creado.

   ![](assets/image2016-3-11-8-3a52-3a20.png)

   >[!NOTE]
   >
   >Este es un ejemplo que utiliza una Call to action Más información. El Call to action de la unidad de anuncios de posibles clientes puede ser diferente.

1. Después de enviar el formulario, [cree una lista inteligente en Marketo](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) como parte de un programa o en la base de datos de posibles clientes que usa el filtro **[!UICONTROL Formulario de anuncios de posibles clientes rellenado en Facebook]**. Inserte el nombre del formulario de anuncio de posibles clientes del formulario que ha enviado.

   ![](assets/image2016-3-11-8-3a59-3a34.png)

1. Ahora haga clic en la pestaña Posibles clientes para validar que la sincronización funciona correctamente.

   ![](assets/image2016-3-11-15-3a27-3a54.png)

>[!NOTE]
>
>[Configurar [!UICONTROL Anuncios Principales De Facebook]](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)
