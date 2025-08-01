---
solution: Marketo Engage
product: marketo
title: Añadir CSS personalizadas al contenido del correo electrónico
description: Aprenda a añadir CSS personalizado al contenido del correo electrónico directamente en el Designer de correo electrónico en Marketo Engage.
level: Intermediate
feature: Email Designer
exl-id: c191b44a-47ab-41f8-aa95-9268e359e5db
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 4%

---

# Añadir CSS personalizadas al contenido del correo electrónico {#custom-css}

Añada su propio CSS personalizado directamente en el Designer de correo electrónico de Marketo Engage para un estilo avanzado y específico.

## Definir CSS personalizado {#define-custom-css}

1. Asegúrese de que haya algún contenido definido en el Designer de correo electrónico añadiendo al menos un componente.

1. Seleccione **[!UICONTROL Cuerpo]**, ya sea en el **[!UICONTROL árbol de navegación]** de la izquierda o en el panel derecho. **[!UICONTROL Estilos CSS]** se muestra a la derecha.

   ![](assets/custom-css-1.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >La sección **[!UICONTROL estilos CSS]** solo está disponible cuando el contenido está presente en el editor.

1. Haga clic en el botón **[!UICONTROL + Agregar CSS]** personalizado.

   >[!NOTE]
   >
   >El botón **[!UICONTROL Agregar CSS personalizado]** solo está disponible cuando se selecciona **[!UICONTROL Cuerpo]**. Sin embargo, puede aplicar estilos CSS personalizados a todos los componentes del contenido.

1. Introduzca su código CSS en el área de texto dedicada que aparece. Asegúrese de que CSS personalizado [ sea válido y siga la sintaxis correcta ](#use-valid-css). Haga clic en **Guardar** cuando termine.

   ![](assets/custom-css-2.png)

   >[!NOTE]
   >
   >No se puede agregar CSS personalizado al contenido al usar una [plantilla con contenido bloqueado](/help/marketo/product-docs/email-marketing/email-designer/content-locking.md). La etiqueta del botón cambia a **[!UICONTROL Ver CSS personalizado]** y cualquier CSS personalizado que se muestre será de solo lectura.

1. Asegúrese de que CSS se aplique al contenido. Si no es así, consulte la sección [Solución de problemas](#troubleshooting).

   ![](assets/custom-css-3.png)

   >[!NOTE]
   >
   >Si elimina todo el contenido, la sección desaparece y ya no se aplica el CSS personalizado definido anteriormente. Vuelva a agregar contenido para que vuelva a aparecer la sección **[!UICONTROL estilos CSS]**. Se vuelve a aplicar el CSS personalizado.

## Uso de CSS válido {#using-valid-css}

Puede introducir cualquier cadena CSS válida en el área de texto **[!UICONTROL Agregar CSS]** personalizado. El CSS con el formato correcto se aplica inmediatamente al contenido.

>[!CAUTION]
>
>Usted es responsable de la seguridad de su CSS personalizado. Asegúrese de que CSS no introduzca vulnerabilidades ni conflictos con el contenido existente.
>
>Evite utilizar CSS que pudiera romper involuntariamente el diseño o la funcionalidad del contenido.

+++ Ejemplos de CSS válido

A continuación se muestran ejemplos de CSS válido.

```css
.acr-component[data-component-id="form"] {
  display: flex;
  justify-content: center;
  background: none;
}

.acr-Form {
  width: 100%;
  padding: 20px 100px;
  border-spacing: 0px 8px;
  box-sizing: border-box;
  margin: 0;
}

.acr-Form .spectrum-FieldLabel {
  width: 20%;
}

.acr-Form.spectrum-Form--labelsAbove .spectrum-FieldLabel,
.acr-Form [data-form-item="checkbox"] .spectrum-FieldLabel {
  width: auto;
}

.acr-Form .spectrum-Textfield {
  width: 100%;
}

#acr-form-error,
#acr-form-confirmation {
  width: 100%;
  padding: var(--spectrum-global-dimension-static-size-500);
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: center;
  gap: var(--spectrum-global-dimension-static-size-200);
}

.spectrum-Form-item.is-required .spectrum-FieldLabel:after{
  content: '*';
  font-size: 1.25rem;
  margin-left: 5px;
  position: absolute;
}

/* Error field placeholder */
.spectrum-HelpText {
  display: none !important;
}

.spectrum-HelpText.is-invalid,
.is-invalid ~ .spectrum-HelpText {
  display: flex !important;
}
```

```css
@media only screen and (min-width: 600px) {
  .acr-paragraph-1 {
    width: 100% !important;
  }
}
```

+++


+++ Ejemplos de CSS no válido

Si se introduce un CSS no válido, se muestra un mensaje de error que indica que el CSS no se puede guardar. A continuación se muestran ejemplos de CSS no válido.

No se acepta el uso de etiquetas `<style>`:

```html
<style type="text/css">
  .acr-Form {
    width: 100%;
    padding: 20px 100px;
    border-spacing: 0px 8px;
    box-sizing: border-box;
    margin: 0;
  }
</style>
```

No se acepta sintaxis no válida como llaves que faltan:

```css
body {
  background: red;
```

+++

## Implementación técnica {#implementation}

Su CSS personalizado se agrega al final de la sección `<head>` como parte de una etiqueta `<style>` con el atributo `data-name="global-custom"`, como en el ejemplo siguiente. Esto garantiza que los estilos personalizados se apliquen globalmente al contenido.

+++ Ver muestra

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="content-version" content="3.3.31">
    <meta name="x-apple-disable-message-reformatting">
    <meta name="viewport" content="width=device-width,initial-scale=1.0">
    <style data-name="default" type="text/css">
      td { padding: 0; }
      th { font-weight: normal; }
    </style>
    <style data-name="grid" type="text/css">
      .acr-grid-table { width: 100%; }
    </style>
    <style data-name="acr-theme" type="text/css" data-theme="default" data-variant="0">
      body { margin: 0; font-family: Arial; }
    </style>
    <style data-name="media-default-max-width-500px" type="text/css">
      @media screen and (max-width: 500px) {
        body { width: 100% !important; }
      }
    </style>
    <style data-name="global-custom" type="text/css">
      /* Add you custom CSS here */
    </style>
  </head>
  <body>
    <!-- Minimal content -->
  </body>
</html>
```

+++


El panel **[!UICONTROL Configuración]** de Designer de correo electrónico no interpreta ni valida la CSS personalizada. Es totalmente independiente y solo se puede modificar mediante la opción **[!UICONTROL Agregar CSS personalizado]**.

### Protecciones: contenido importado {#guardrails}

Si desea utilizar CSS personalizado con contenido importado en el Designer de correo electrónico, tenga en cuenta lo siguiente:

* Si [importa contenido externo de HTML](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#import-html), incluido CSS, a menos que convierta ese contenido, estará en **[!UICONTROL modo de compatibilidad]**, donde la sección **[!UICONTROL estilos CSS]** no está disponible.

* Si al importar contenido creado con Email Designer se incluye CSS aplicado a través de la opción **[!UICONTROL Agregar CSS personalizado]**, el CSS aplicado anteriormente será visible y editable desde la misma opción.

## Resolución de problemas {#troubleshooting}

Si no se aplica el CSS personalizado, pruebe las sugerencias siguientes.

* Asegúrese de que el CSS sea válido y esté libre de errores de sintaxis (como llaves que faltan, nombres de propiedad incorrectos). [Descubra cómo](#use-valid-css)

* Asegúrese de que su CSS se esté agregando a la etiqueta `<style>` con el atributo `data-name="global-custom"`.

* Compruebe si la etiqueta de estilo `global-custom` tiene el atributo `data-disabled` establecido en `true`. Si es así, no se aplica el CSS personalizado.

+++ Por ejemplo:

  ```html
  <style data-name="global-custom" type="text/css" data-disabled="true"> body: { color: red; } </style>
  ```

+++

* Asegúrese de que otras reglas CSS no anulen su CSS.

   * Utilice las herramientas para desarrolladores del navegador para inspeccionar el contenido y verificar que el CSS está dirigido a los selectores correctos.

   * Considere agregar `!important` a sus declaraciones para asegurarse de que tengan prioridad.

+++ Por ejemplo:

     ```css
     .acr-Form {
       background: red !important;
     }
     ```

+++

>[!NOTE]
>
>La compatibilidad con Marketo Engage no está configurada para ayudar a solucionar problemas con CSS personalizado. Para obtener ayuda sobre CSS, consulte con un desarrollador web.
