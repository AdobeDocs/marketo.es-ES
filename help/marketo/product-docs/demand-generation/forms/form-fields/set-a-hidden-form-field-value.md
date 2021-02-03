---
unique-page-id: 2359663
description: Definir un valor de campo de formulario oculto - Documentos de marketing - Documentación del producto
title: Definir un valor de campo de formulario oculto
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---


# Definir un valor de campo de formulario oculto {#set-a-hidden-form-field-value}

Los campos ocultos suelen rellenarse dinámicamente. No se muestran a la persona que rellena el formulario. Así es como se establece el valor.

>[!PREREQUISITES]
>
>[Definir un campo de formulario como oculto](/help/marketo/product-docs/demand-generation/forms/form-fields/set-a-form-field-as-hidden.md)

## Seleccione el campo {#select-the-field}

1. En el formulario, seleccione el campo oculto y haga clic en **Editar** para **Rellenar automáticamente**.

   ![](assets/autofill.png)

## Usar valor predeterminado {#use-default-value}

Si selecciona Usar valor predeterminado, puede codificar un valor específico para utilizarlo siempre cuando se envíe este formulario. Introduzca el valor predeterminado y haga clic en Guardar.

![](assets/image2014-9-15-13-3a5-3a27.png)

## Parámetro de URL {#url-parameter}

Si desea capturar los parámetros de URL (cadenas de Consulta) de la página en la que se encuentra la persona al rellenar el formulario, puede utilizar **parámetros de URL** para rellenar el campo oculto.

>[!NOTE]
>
>Los parámetros son algo técnicos, ¿no es así? Una vez que los consigues, son poderosos. Esta [página de Wikipedia en cadenas de Consulta](https://en.wikipedia.org/wiki/Query_string) es de alguna manera útil.

1. Seleccione **Parámetro de URL** para **Obtener tipo de valor**.

   ![](assets/image2014-9-15-13-3a6-3a48.png)

1. Introduzca el **Nombre de parámetro** y haga clic en **Guardar**.

   ![](assets/image2014-9-15-13-3a7-3a35.png)

>[!TIP]
>
>Puede introducir un valor predeterminado en caso de que no se encuentre el parámetro de URL.

## Valor de cookie {#cookie-value}

Si está almacenando datos en cookies, puede utilizar **Valor de la cookie** para recoger datos cuando se envía el formulario.

1. Seleccione **Valor de la cookie** para **Obtener valor de**.

   ![](assets/image2014-9-15-13-3a8-3a21.png)

1. Escriba el nombre del parámetro de cookie que desee y haga clic en **Guardar**.

   ![](assets/image2014-9-15-13-3a8-3a43.png)

   >[!TIP]
   >
   >Puede introducir un valor predeterminado en caso de que no se encuentre el parámetro o la cookie.

## Parámetro de remitente del reenvío {#referrer-parameter}

Si desea capturar datos de la página de la que proviene el visitante antes de rellenar el formulario, puede utilizar **Parámetro de Remitente del reenvío**.

1. Establezca **Obtener valor de** en **Parámetro de Remitente del reenvío**.

   ![](assets/image2014-9-15-13-3a9-3a31.png)

1. Introduzca el **Nombre de parámetro** que desea extraer de la URL de remitente del reenvío y haga clic en **Guardar**.

   ![](assets/image2014-9-15-13-3a9-3a56.png)

   >[!TIP]
   >
   >Puede introducir un **Valor predeterminado** en caso de que no se encuentre el parámetro de remitente del reenvío.

1. Haga clic en **Finalizar**.

   ![](assets/image2014-9-15-13-3a10-3a26.png)

1. Haga clic en **Aprobar y cerrar**.

   ![](assets/image2014-9-15-13-3a10-3a43.png)
