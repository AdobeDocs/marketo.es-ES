---
unique-page-id: 2359644
description: Mostrar formulario HTML personalizado para personas conocidas - Documentos de Marketo - Documentación del producto
title: Mostrar formulario HTML personalizado para personas conocidas
exl-id: 668216ea-7c2b-4204-81a5-56547c3baf1d
feature: Forms
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 1%

---

# Mostrar formulario HTML personalizado para personas conocidas {#show-custom-html-form-for-known-people}

Si un visitante ha proporcionado su nombre completo y dirección de correo electrónico en el pasado y no desea que obtenga todo el formulario, aprenda a mostrarle un HTML personalizado (por ejemplo, solo un botón de descarga).

1. Vaya a **[!UICONTROL Actividades de marketing]**.

   ![](assets/login-marketing-activities-5.png)

1. En **[!UICONTROL Actividades de marketing]**, seleccione el formulario y haga clic en **[!UICONTROL Editar formulario]**.

   ![](assets/image2014-9-15-12-3a24-3a6.png)

1. En **[!UICONTROL Configuración de formulario]**, haga clic en **[!UICONTROL Configuración]**.

   ![](assets/image2014-9-15-12-3a24-3a36.png)

1. Definir Si **[!UICONTROL Visitante conocido, Mostrar]**: como **[!UICONTROL HTML personalizado]**.

   ![](assets/image2014-9-15-12-3a24-3a59.png)

1. Haga clic en ![—](assets/image2014-9-25-14-3a1-3a26.png) para editar **[!UICONTROL HTML personalizado]** que se mostrará a las personas conocidas.

   ![](assets/image2014-9-15-12-3a25-3a38.png)

1. Hay contenido predeterminado, pero no dude en cambiarlo.

   ![](assets/image2014-9-15-12-3a25-3a49.png)

   Tokens disponibles:

   | Token | Descripción |
   |---|---|
   | `{{lead.FirstName}}` | Se mostrará el nombre de la persona. |
   | `{{lead.LastName}}` | Se mostrará el apellido de la persona. |
   | `{{form.Button:default=Download}}` | Se mostrará el botón del formulario. Reemplace el área después de `=` para cambiar el texto del botón. |
   | `{{form.NotYou:default=Not you?}}` | Se mostrará un vínculo en caso de que la persona sea otra. Reemplace el área después de `=` para cambiar el texto del vínculo. |

   >[!CAUTION]
   >
   >Solo se pueden utilizar los cuatro tokens anteriores. Aquí no funcionará ningún otro token.

1. Haga clic en **[!UICONTROL Finalizar]**.

   ![](assets/image2014-9-15-12-3a27-3a25.png)

1. Haga clic en **[!UICONTROL Aprobar y cerrar]**.

   >[!NOTE]
   >
   >El formulario debe aprobarse para poder utilizarse en páginas de aterrizaje.

   ![](assets/image2014-9-15-12-3a27-3a53.png)

   >[!NOTE]
   >
   >Recuerde [aprobar los cambios del borrador de la página de aterrizaje](/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/approve-unapprove-or-delete-a-landing-page.md) creado por el formulario.

   ¡Pedazo de torta! Vea lo que una persona vería si volviera al mismo formulario:

   ![](assets/image2014-9-15-12-3a28-3a12.png)

   >[!TIP]
   >
   >Puede dirigir el clic del botón al recurso estableciendo la página de seguimiento del formulario en la dirección URL del archivo.
