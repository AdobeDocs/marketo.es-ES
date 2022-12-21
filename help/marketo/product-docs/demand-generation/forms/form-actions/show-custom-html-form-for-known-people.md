---
unique-page-id: 2359644
description: Mostrar formulario de HTML personalizado para personas conocidas - Documentos de Marketo - Documentación del producto
title: Mostrar formulario de HTML personalizado para personas conocidas
exl-id: 668216ea-7c2b-4204-81a5-56547c3baf1d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---

# Mostrar formulario de HTML personalizado para personas conocidas {#show-custom-html-form-for-known-people}

Si se coordina a un visitante (persona conocida que proporcionó una dirección de correo electrónico en el pasado), ¿por qué molestarse con el formulario? Simplemente déles el botón de descarga. Así es como.

1. Vaya a **Actividades de marketing**.

   ![](assets/login-marketing-activities-5.png)

1. En **Actividades de marketing**, seleccione el formulario y haga clic en **Editar formulario**.

   ![](assets/image2014-9-15-12-3a24-3a6.png)

1. En **Configuración de formulario**, haga clic en **Configuración**.

   ![](assets/image2014-9-15-12-3a24-3a36.png)

1. Establezca Si **Visitante conocido, mostrar**: a **HTML personalizado**.

   ![](assets/image2014-9-15-12-3a24-3a59.png)

1. Haga clic en el ![—](assets/image2014-9-25-14-3a1-3a26.png) para editar el **HTML personalizado** que se mostrará a personas conocidas.

   ![](assets/image2014-9-15-12-3a25-3a38.png)

1. Hay contenido predeterminado, pero no dude en cambiarlo.

   ![](assets/image2014-9-15-12-3a25-3a49.png)

   Tokens disponibles:

   | Token | Descripción |
   |---|---|
   | `{{lead.FirstName}}` | Se mostrará el nombre de la persona. |
   | `{{lead.LastName}}` | Se mostrará el apellido de la persona. |
   | `{{form.Button:default=Download}}` | Se mostrará el botón del formulario. Reemplace el área después de la variable `=` para cambiar el texto del botón. |
   | `{{form.NotYou:default=Not you?}}` | Se mostrará un vínculo en caso de que la persona sea otra. Reemplace el área después de la variable `=` para cambiar el texto del vínculo. |

   >[!CAUTION]
   >
   >Solo se pueden utilizar los cuatro tokens anteriores. Cualquier otro token no funcionará aquí.

1. Haga clic en **Finalizar**.

   ![](assets/image2014-9-15-12-3a27-3a25.png)

1. Haga clic en **Aprobar y cerrar**.

   >[!NOTE]
   >
   >El formulario debe aprobarse para utilizarse en páginas de aterrizaje.

   ![](assets/image2014-9-15-12-3a27-3a53.png)

   >[!NOTE]
   >
   >Recuerde [aprobar el borrador de la página de aterrizaje](/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/approve-unapprove-or-delete-a-landing-page.md) creado por los cambios del formulario.

   ¡Un trozo de tarta! Eche un vistazo a lo que una persona vería si regresara al mismo formulario:

   ![](assets/image2014-9-15-12-3a28-3a12.png)

   >[!TIP]
   >
   >Puede dirigir el clic del botón al recurso configurando la página de seguimiento del formulario en la dirección URL del archivo.
