---
unique-page-id: 5472348
description: Hacer compatible una plantilla de página de aterrizaje de forma libre existente con dispositivos móviles - Documentos de Marketo - Documentación del producto
title: Hacer compatible una plantilla de página de destino de forma libre existente con dispositivos móviles
exl-id: 942456a5-3f3e-4a71-aecc-4cc6bf6237b3
feature: Landing Pages
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 3%

---

# Hacer compatible una plantilla de página de aterrizaje de forma libre existente [!UICONTROL móvil] {#make-an-existing-free-form-landing-page-template-mobile-compatible}

Esto se puede hacer en dos lugares, el Editor de plantillas y el Editor de páginas de aterrizaje.

## Actualización desde el Editor de plantillas {#upgrade-from-the-template-editor}

1. Vaya a **[!UICONTROL Design Studio]**.

   ![](assets/designstudio-1.png)

1. Seleccione **[!UICONTROL Plantillas]**.

   ![](assets/image2015-1-22-20-3a20-3a2.png)

1. Seleccione una plantilla donde **[!UICONTROL Compatible con dispositivos móviles]** sea **[!UICONTROL No]**.

   ![](assets/image2015-1-22-20-3a22-3a24.png)

1. Haga clic en **[!UICONTROL Editar borrador]**.

   ![](assets/image2015-1-22-20-3a25-3a36.png)

1. Haga clic en **[!UICONTROL Hacer compatible el móvil]**.

   ![](assets/image2015-1-22-20-3a30-3a33.png)

1. Haga clic en **[!UICONTROL Actualizar]**.

   ![](assets/image2015-1-22-20-3a32-3a45.png)

   La plantilla de la página de aterrizaje ahora es compatible con dispositivos móviles.

   >[!NOTE]
   >
   >La actualización debe ser inofensiva, pero asegúrese de comprobar las páginas para detectar cualquier discrepancia. La actualización creará borradores de cualquier página de aterrizaje que utilice esa plantilla.

   ![](assets/image2015-1-22-20-3a36-3a43.png)

## ¿Qué hace que una plantilla [!UICONTROL móvil sea compatible]? {#what-makes-a-template-mobile-compatible}

¡Grandes preguntas! La plantilla debe tener las etiquetas siguientes:

`Must have <!DOCTYPE HTML> Must have a <HEAD> element Must have a <TITLE> in the <HEAD> element Must have <META CHARSET="UTF-8"> within the <HEAD> element Must have a <BODY> element that contains one (and only one) <DIV class="mktoContent"></DIV>`

Si todo se ve bien, verá este mensaje.

![](assets/image2015-1-22-20-3a41-3a31.png)

Si algo está mal, aparecerá un mensaje de error, haga clic en reparar para solucionar el problema y repita el proceso de validación.

![](assets/image2015-1-22-20-3a43-3a20.png)

Si realiza cambios en la plantilla, haga clic en [!UICONTROL Acciones de plantilla] y seleccione [!UICONTROL Validar compatibilidad móvil].

## Actualización de una plantilla desde el editor de páginas de aterrizaje de forma libre {#upgrading-a-template-from-the-free-form-landing-page-editor}

Cuando está editando una página de aterrizaje y hace clic en la pestaña móvil, a veces observa que la plantilla no se ha actualizado. ¡No temas! Puede actualizarlo justo allí.

1. Haga clic en la ficha **[!UICONTROL Móvil]**.

   ![](assets/image2015-1-22-20-3a48-3a19.png)

1. Haga clic en la casilla y luego en **[!UICONTROL Activar]**.

   ![](assets/image2015-1-22-20-3a49-3a34.png)

   >[!NOTE]
   >
   >Al activar la versión móvil de una plantilla, se crearán borradores de todas las páginas de aterrizaje que la utilicen.

¡Fantástico! Ahora puedes [personalizar la vista móvil](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/customize-mobile-view-for-your-free-form-landing-page.md) de todas tus páginas de aterrizaje que usen esta plantilla.
