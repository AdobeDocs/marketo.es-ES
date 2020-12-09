---
unique-page-id: 5472348
description: Conversión de plantillas de Página de aterrizaje de forma libre existentes en móviles compatibles - Documentos de marketing - Documentación del producto
title: Conversión de una plantilla de Página de aterrizaje de forma libre existente en compatible con móviles
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---


# Conversión de una plantilla de Página de aterrizaje de forma libre existente en compatible con móviles {#make-an-existing-free-form-landing-page-template-mobile-compatible}

>[!NOTE]
>
>Las plantillas de páginas de aterrizaje creadas antes de la versión [de enero de 2015 deben](../../../../release-notes/2015/release-notes-january-2015.md)actualizarse para que sean compatibles con dispositivos móviles.

Esto se puede hacer en dos lugares: el Editor de plantillas y el Editor de Páginas de aterrizaje.

## Actualizar desde el Editor de plantillas {#upgrade-from-the-template-editor}

1. Vaya a **Design Studio**.

   ![](assets/designstudio-1.png)

1. Seleccione **Plantillas**.

   ![](assets/image2015-1-22-20-3a20-3a2.png)

1. Seleccione una plantilla en la que Compatible con **móviles** sea **No**.

   ![](assets/image2015-1-22-20-3a22-3a24.png)

1. Haga clic en **Editar borrador**.

   ![](assets/image2015-1-22-20-3a25-3a36.png)

1. Haga clic en **Hacer que los móviles sean compatibles**.

   ![](assets/image2015-1-22-20-3a30-3a33.png)

1. Haga clic en **Actualizar**.

   ![](assets/image2015-1-22-20-3a32-3a45.png)

   La plantilla de página de aterrizaje ahora es compatible con móviles.

   >[!NOTE]
   >
   >La actualización debe ser inocua, pero asegúrese de comprobar las discrepancias en las páginas. La actualización creará borradores de cualquier página de aterrizaje que utilice esa plantilla.

   ![](assets/image2015-1-22-20-3a36-3a43.png)

## ¿Qué hace que una plantilla móvil sea compatible? {#what-makes-a-template-mobile-compatible}

¡buenas preguntas! La plantilla debe tener las siguientes etiquetas:

`<pre data-theme="Confluence">Must have <!DOCTYPE HTML> Must have a <HEAD> element Must have a <TITLE> in the <HEAD> element Must have <META CHARSET="UTF-8"> within the <HEAD> element Must have a <BODY> element that contains one (and only one) <DIV class="mktoContent"></DIV></pre>`  Si todo se ve bien, verá este mensaje.

![](assets/image2015-1-22-20-3a41-3a31.png)

Si algo no funciona, aparecerá un mensaje de error, haga clic en Reparar para solucionar el problema y repetir el proceso de validación.

![](assets/image2015-1-22-20-3a43-3a20.png)

Si realiza cambios en la plantilla, haga clic en Acciones de plantilla y seleccione Validar compatibilidad móvil.

## Actualización de una plantilla desde el Editor de Páginas de aterrizaje de formato libre {#upgrading-a-template-from-the-free-form-landing-page-editor}

Cuando edita una página de aterrizaje y hace clic en la ficha móvil, a veces se da cuenta de que la plantilla no se ha actualizado. ¡No teman! Puede actualizarlo aquí mismo.

1. Haga clic en la ficha **Móvil** .

   ![](assets/image2015-1-22-20-3a48-3a19.png)

1. Haga clic en la casilla de verificación y en **Activar**.

   ![](assets/image2015-1-22-20-3a49-3a34.png)

   >[!NOTE]
   >
   >Al activar la versión móvil de una plantilla, se crearán borradores de cualquier página de aterrizaje que la utilice.

¡Increíble! Ahora puede [personalizar la vista](../../../../product-docs/demand-generation/landing-pages/free-form-landing-pages/customize-mobile-view-for-your-free-form-landing-page.md) móvil de todas las páginas de aterrizaje que utilicen esta plantilla.

>[!MORELIKETHIS]
>
>* [Personalización de la Vista móvil para su Página de aterrizaje de forma libre](../../../../product-docs/demand-generation/landing-pages/free-form-landing-pages/customize-mobile-view-for-your-free-form-landing-page.md)

>



