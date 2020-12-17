---
unique-page-id: 4719306
description: Ocultar un campo de Salesforce de la sincronización de marketing - Documentos de marketing - Documentación del producto
title: Ocultar un campo de Salesforce de la sincronización de marketing
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---


# Ocultar un campo de Salesforce de la sincronización de marketing {#hide-a-salesforce-field-from-the-marketo-sync}

>[!NOTE]
>
>**Se requieren permisos de administración**

No todos los campos de Salesforce son útiles para la mercadotecnia. Puede optimizar el rendimiento de la sincronización incluyendo solo los campos que necesite. Así es como se puede ocultar un campo de Marketing.

1. Haga clic en el menú de nombre y seleccione **Configuración**.

   ![](assets/image2015-6-30-15-3a11-3a23.png)

1. Escriba **perfiles** en la barra de búsqueda y haga clic en **Perfiles** en **Administrar usuarios**.

   ![](assets/image2015-6-30-15-3a12-3a46.png)

1. Haga clic en el perfil del usuario de sincronización.

   ![](assets/image2015-6-30-15-3a17-3a38.png)

1. En la sección **Seguridad a nivel de campo**, haga clic en **Vista** al lado del objeto que contiene el campo destinatario.

   ![](assets/image2015-6-30-15-3a24-3a32.png)

1. Haga clic en **Editar**.

   ![](assets/image2015-6-30-15-3a25-3a42.png)

1. Desmarque la casilla **Visible** junto al campo que desee ocultar. Haga clic en **Guardar**.

   ![](assets/image2015-6-30-15-3a27-3a16.png)

   >[!NOTE]
   >
   >Si el campo que oculta en Salesforce ya se ha sincronizado con Marketing, también deberá ocultarlo en Marketing, si no desea utilizarlo.

   ¡Eso es todo! Ya no verá este campo en el Explorador de mercadotecnia una vez finalizada la siguiente sincronización.

   >[!NOTE]
   >
   >**Artículos relacionados**
   >
   >    
   >    
   >    * [Ocultar y mostrar un campo](../../../../../product-docs/administration/field-management/hide-and-unhide-a-field.md)


