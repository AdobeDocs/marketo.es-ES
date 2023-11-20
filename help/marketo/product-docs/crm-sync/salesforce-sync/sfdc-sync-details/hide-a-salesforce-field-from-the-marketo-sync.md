---
unique-page-id: 4719306
description: 'Ocultar un campo de Salesforce de la sincronización de Marketo: documentos de Marketo, documentación del producto'
title: Ocultar un campo de Salesforce de la sincronización de Marketo
exl-id: 5d7229f0-43b0-4232-93ed-a9ca52ace401
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 1%

---

# Ocultar un campo de Salesforce de la sincronización de Marketo {#hide-a-salesforce-field-from-the-marketo-sync}

>[!NOTE]
>
>**Permisos de administración necesarios**

No todos los campos de Salesforce son útiles para Marketing. Puede optimizar el rendimiento de la sincronización incluyendo solo los campos que necesite. Así se puede ocultar un campo a un Marketo Engage.

1. Haga clic en el menú de nombre y seleccione **[!UICONTROL Configurar]**.

   ![](assets/image2015-6-30-15-3a11-3a23.png)

1. Introduzca &quot;perfiles&quot; en la barra de búsqueda y haga clic en **[!UICONTROL Perfiles]** bajo **[!UICONTROL Administrar usuarios]**.

   ![](assets/image2015-6-30-15-3a12-3a46.png)

1. Haga clic en el perfil del usuario de sincronización.

   ![](assets/image2015-6-30-15-3a17-3a38.png)

1. En el **[!UICONTROL Seguridad de nivel de campo]** , haga clic en **[!UICONTROL Ver]** después, el objeto que contiene el campo de destino.

   ![](assets/image2015-6-30-15-3a24-3a32.png)

1. Clic **[!UICONTROL Editar]**.

   ![](assets/image2015-6-30-15-3a25-3a42.png)

1. Desmarque la **[!UICONTROL Visible]** junto al campo que desee ocultar. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2015-6-30-15-3a27-3a16.png)

   >[!NOTE]
   >
   >Si el campo que oculta en Salesforce ya se ha sincronizado con Marketo, también debe ocultarlo en Marketo si no desea utilizarlo.

   ¡Eso es todo! Dejará de ver este campo en Marketo una vez finalizada la siguiente sincronización.

   >[!MORELIKETHIS]
   >
   >[Ocultar y mostrar un campo](/help/marketo/product-docs/administration/field-management/hide-and-unhide-a-field.md){target="_blank"}
