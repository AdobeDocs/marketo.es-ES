---
unique-page-id: 2359663
description: Definir un valor de campo de formulario oculto - Documentos de Marketo - Documentación del producto
title: Establecer un valor de campo de formulario oculto
exl-id: acec7de1-8567-42c0-a6ce-a91b0bf69f41
feature: Forms
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---

# Establecer un valor de campo de formulario oculto {#set-a-hidden-form-field-value}

Los campos ocultos generalmente se rellenan dinámicamente. No se muestran a la persona que rellena el formulario. A continuación se indica cómo establecer el valor.

>[!PREREQUISITES]
>
>[Definir un campo de formulario como oculto](/help/marketo/product-docs/demand-generation/forms/form-fields/set-a-form-field-as-hidden.md)

## Seleccione el campo {#select-the-field}

1. En el formulario, seleccione el campo oculto y haga clic en **Editar** para **Relleno automático**.

   ![](assets/autofill.png)

## Utilizar valor predeterminado {#use-default-value}

Al seleccionar Utilizar valor predeterminado, puede codificar un valor específico para que se utilice siempre cuando se envíe este formulario. Introduzca el valor predeterminado y haga clic en Guardar.

![](assets/image2014-9-15-13-3a5-3a27.png)

## Parámetro URL {#url-parameter}

Si desea capturar los parámetros de URL (cadenas de consulta) de la página en la que se encuentra la persona al rellenar el formulario, puede utilizar **Parámetros de URL** para rellenar el campo oculto.

>[!NOTE]
>
>Los parámetros son un poco técnicos, ¿no? Sin embargo, una vez que los tienes, son poderosos. Esta [Página de Wikipedia sobre cadenas de consulta](https://en.wikipedia.org/wiki/Query_string) es de alguna manera útil.

1. Seleccionar **Parámetro URL** para **Obtener tipo de valor**.

   ![](assets/image2014-9-15-13-3a6-3a48.png)

1. Introduzca el **Nombre de parámetro** y haga clic en **Guardar**.

   ![](assets/image2014-9-15-13-3a7-3a35.png)

>[!TIP]
>
>Puede introducir un Valor predeterminado en caso de que no se encuentre el parámetro de URL.

## Valor de cookie {#cookie-value}

Si almacena datos en cookies, puede utilizar **Valor de cookie** para recoger datos cuando se envía el formulario.

1. Seleccionar **Valor de cookie** para **Obtener valor de**.

   ![](assets/image2014-9-15-13-3a8-3a21.png)

1. Introduzca el nombre de parámetro de la cookie que desee y haga clic en **Guardar**.

   ![](assets/image2014-9-15-13-3a8-3a43.png)

   >[!TIP]
   >
   >Puede introducir un Valor predeterminado en caso de que no se encuentre el parámetro o la cookie.

## Parámetro de referente {#referrer-parameter}

Si desea capturar datos de la página de la que proviene el visitante antes de rellenar el formulario, puede utilizar **Parámetro de referente**.

1. Establecer **Obtener valor de** hasta **Parámetro de referente**.

   ![](assets/image2014-9-15-13-3a9-3a31.png)

1. Introduzca el **Nombre de parámetro** que desee extraer de la dirección URL de referencia y haga clic en **Guardar**.

   ![](assets/image2014-9-15-13-3a9-3a56.png)

   >[!TIP]
   >
   >Puede introducir un **Valor predeterminado** en caso de que no se encuentre el parámetro referrer.

1. Clic **Finalizar**.

   ![](assets/image2014-9-15-13-3a10-3a26.png)

1. Clic **Aprobar y cerrar**.

   ![](assets/image2014-9-15-13-3a10-3a43.png)
