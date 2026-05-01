---
unique-page-id: 4719306
description: Obtenga información sobre cómo ocultar un campo de Salesforce de la sincronización de Marketo para optimizar el rendimiento. Utilice la seguridad a nivel de campo en el perfil de usuario de sincronización para excluir los campos innecesarios.
title: Ocultar un campo de Salesforce de la sincronización de Marketo
exl-id: 5d7229f0-43b0-4232-93ed-a9ca52ace401
feature: Salesforce Integration
source-git-commit: f4ac42384a47d4b5e1ca139f1580ab475c58f543
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 11%

---

# Ocultar un campo [!DNL Salesforce] de la sincronización de Marketo {#hide-a-salesforce-field-from-the-marketo-sync}

>[!NOTE]
>
>**Se requieren permisos de administrador**

No todos los campos de Salesforce son útiles para Marketing. Puede optimizar el rendimiento de la sincronización incluyendo solo los campos que necesite. Así se puede ocultar un campo de Marketo Engage.

1. Haz clic en el menú de tu nombre y selecciona **[!UICONTROL Configuración]**.

   ![](assets/image2015-6-30-15-3a11-3a23.png)

1. Escriba &quot;perfiles&quot; en la barra de búsqueda y haga clic en **[!UICONTROL Perfiles]** en **[!UICONTROL Administrar usuarios]**.

   ![](assets/image2015-6-30-15-3a12-3a46.png)

1. Haga clic en el perfil del usuario de sincronización.

   ![](assets/image2015-6-30-15-3a17-3a38.png)

1. En la sección **[!UICONTROL Seguridad de nivel de campo]**, haga clic en **[!UICONTROL Ver]** junto al objeto que contiene el campo de destino.

   ![](assets/image2015-6-30-15-3a24-3a32.png)

1. Haga clic en **[!UICONTROL Editar]**.

   ![](assets/image2015-6-30-15-3a25-3a42.png)

1. Desmarque la casilla **[!UICONTROL Visible]** que está junto al campo que desea ocultar. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2015-6-30-15-3a27-3a16.png)

   >[!NOTE]
   >
   >Si el campo que oculta en [!DNL Salesforce] ya se ha sincronizado con Marketo, también deberá ocultarlo en Marketo si no desea utilizarlo.

   Este campo ya no aparece en Marketo una vez finalizada la siguiente sincronización.

   >[!MORELIKETHIS]
   >
   >[Ocultar y mostrar un campo](/help/marketo/product-docs/administration/field-management/hide-and-unhide-a-field.md){target="_blank"}
