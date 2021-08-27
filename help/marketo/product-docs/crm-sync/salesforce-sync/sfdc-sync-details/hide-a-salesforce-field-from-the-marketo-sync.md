---
unique-page-id: 4719306
description: Ocultar un campo de Salesforce de la sincronización de Marketo - Marketo Docs - Documentación del producto
title: Ocultar un campo de Salesforce de la sincronización de Marketo
exl-id: 5d7229f0-43b0-4232-93ed-a9ca52ace401
source-git-commit: 7376804bda915d7ff25cdc50cb78a6686bd36882
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 0%

---

# Ocultar un campo de Salesforce de la sincronización de Marketo {#hide-a-salesforce-field-from-the-marketo-sync}

>[!NOTE]
>
>**Se requieren permisos de administrador**

No todos los campos de Salesforce son útiles para Marketing. Puede optimizar el rendimiento de la sincronización incluyendo solo los campos que necesite. Así puede ocultar un campo de Marketo.

1. Haga clic en el menú de su nombre y seleccione **Configuración**.

   ![](assets/image2015-6-30-15-3a11-3a23.png)

1. Introduzca **profiles** en la barra de búsqueda y haga clic en **Perfiles** en **Administrar usuarios**.

   ![](assets/image2015-6-30-15-3a12-3a46.png)

1. Haga clic en el perfil del usuario de sincronización.

   ![](assets/image2015-6-30-15-3a17-3a38.png)

1. En la sección **Field-Level Security**, haga clic en **View** junto al objeto que contiene el campo de destino.

   ![](assets/image2015-6-30-15-3a24-3a32.png)

1. Haga clic en **Editar**.

   ![](assets/image2015-6-30-15-3a25-3a42.png)

1. Desmarque la casilla **Visible** situada junto al campo que desee ocultar. Haga clic en **Guardar**.

   ![](assets/image2015-6-30-15-3a27-3a16.png)

   >[!NOTE]
   >
   >Si el campo que oculta en Salesforce ya se ha sincronizado con Marketo, también deberá ocultarlo en Marketo si no desea utilizarlo.

   ¡Eso es todo! Ya no verá este campo en Marketo una vez finalizada la siguiente sincronización.

   >[!MORELIKETHIS]
   >
   >[Ocultar y mostrar un campo](/help/marketo/product-docs/administration/field-management/hide-and-unhide-a-field.md)
