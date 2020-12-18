---
unique-page-id: 2359644
description: Mostrar formulario HTML personalizado para personas conocidas - Documentos de marketing - Documentación del producto
title: Mostrar formulario HTML personalizado para personas conocidas
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---


# Mostrar formulario HTML personalizado para personas conocidas {#show-custom-html-form-for-known-people}

Si un visitante recibe una cookie (una persona conocida que proporcionó una dirección de correo electrónico en el pasado), ¿por qué molestarse con el formulario? Simplemente déles el botón de descarga. Así es como.

1. Vaya a **Marketing** **Actividades**.

   ![](assets/login-marketing-activities-5.png)

1. En **Marketing** **Actividades**, seleccione el formulario y haga clic en **Editar** **Formulario**.

   ![](assets/image2014-9-15-12-3a24-3a6.png)

1. En **Formulario** **Configuración**, haga clic en **Configuración**.

   ![](assets/image2014-9-15-12-3a24-3a36.png)

1. Definir si **Visitante conocido** **muestra**: a **Personalizado** **HTML**.

   ![](assets/image2014-9-15-12-3a24-3a59.png)

1. Haga clic en ![—](assets/image2014-9-25-14-3a1-3a26.png) para editar el **HTML** **personalizado** que se mostrará a personas conocidas.

   ![](assets/image2014-9-15-12-3a25-3a38.png)

1. Hay contenido predeterminado, pero no dude en cambiarlo.

   ![](assets/image2014-9-15-12-3a25-3a49.png)

   Testigos disponibles:

   | Token | Descripción |
   |---|---|
   | `{{lead.FirstName}}` | Esto mostrará el nombre de la persona. |
   | `{{lead.LastName}}` | Esto mostrará el apellido de la persona. |
   | `{{form.Button:default=Download}}` | Se mostrará el botón de formulario. Reemplace el área después de `=` para cambiar el texto del botón. |
   | `{{form.NotYou:default=Not you?}}` | Esto mostrará un vínculo en caso de que la persona sea otra. Reemplace el área después de `=` para cambiar el texto del vínculo. |

   >[!CAUTION]
   >
   >Sólo se pueden usar los cuatro tokens anteriores. Ningún otro token funcionará aquí.

1. Haga clic en **Finalizar**.

   ![](assets/image2014-9-15-12-3a27-3a25.png)

1. Haga clic en **Aprobar y cerrar**.

   >[!NOTE]
   >
   >El formulario debe aprobarse para utilizarse en páginas de aterrizaje.

   ![](assets/image2014-9-15-12-3a27-3a53.png)

   >[!NOTE]
   >
   >**Recordatorio**
   >
   >
   >Recuerde [aprobar el borrador de página de aterrizaje](../../../../product-docs/demand-generation/landing-pages/understanding-landing-pages/approve-unapprove-or-delete-a-landing-page.md) creado por los cambios del formulario.

   ![](assets/image2014-9-15-12-3a28-3a12.png)

   >[!TIP]
   >
   >Puede dirigir el clic del botón al recurso configurando la página de seguimiento del formulario en la dirección URL del archivo.

¡Un pedazo de torta! Echa un vistazo a lo que una persona vería si regresara al mismo formulario: