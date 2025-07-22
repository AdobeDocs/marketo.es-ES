---
unique-page-id: 2359663
description: Definir un valor de campo de formulario oculto - Documentos de Marketo - Documentación del producto
title: Establecer un valor de campo de formulario oculto
exl-id: acec7de1-8567-42c0-a6ce-a91b0bf69f41
feature: Forms
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 3%

---

# Establecer un valor de campo de formulario oculto {#set-a-hidden-form-field-value}

Los campos ocultos generalmente se rellenan dinámicamente. No se muestran a la persona que rellena el formulario. A continuación se indica cómo establecer el valor.

>[!PREREQUISITES]
>
>[Establecer un campo de formulario como oculto](/help/marketo/product-docs/demand-generation/forms/form-fields/set-a-form-field-as-hidden.md)

## Seleccione el campo {#select-the-field}

1. En el formulario, selecciona el campo oculto y haz clic en **[!UICONTROL Editar]** para **[!UICONTROL Rellenar automáticamente]**.

   ![](assets/autofill.png)

## Utilizar valor predeterminado {#use-default-value}

Si selecciona Usar **[!UICONTROL valor predeterminado]**, puede codificar un valor específico para que se utilice siempre cuando se envíe este formulario. Escriba el **[!UICONTROL Valor predeterminado]** y haga clic en **[!UICONTROL Guardar]**.

![](assets/image2014-9-15-13-3a5-3a27.png)

## URL Parameter {#url-parameter}

Si desea capturar los parámetros de URL (cadenas de consulta) de la página en la que se encuentra la persona al rellenar el formulario, puede usar **[!UICONTROL parámetros de URL]** para rellenar el campo oculto.

>[!NOTE]
>
>Los parámetros son un poco técnicos, ¿no? Sin embargo, una vez que los tienes, son poderosos. Esta [página de Wikipedia sobre cadenas de consulta](https://en.wikipedia.org/wiki/Query_string) es de alguna manera útil.

1. Seleccione **[!UICONTROL Parámetro de dirección URL]** para **[!UICONTROL Obtener tipo de valor]**.

   ![](assets/image2014-9-15-13-3a6-3a48.png)

1. Escriba el **[!UICONTROL Nombre del parámetro]** y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2014-9-15-13-3a7-3a35.png)

>[!TIP]
>
>Puede escribir un **[!UICONTROL Valor predeterminado]** en caso de que no se encuentre el parámetro de la dirección URL.

## Valor de cookie {#cookie-value}

Si está almacenando datos en cookies, puede usar **[!UICONTROL Valor de la cookie]** para recoger datos cuando se envíe el formulario.

1. Seleccione **[!UICONTROL Valor de cookie]** para **[!UICONTROL Obtener valor de]**.

   ![](assets/image2014-9-15-13-3a8-3a21.png)

1. Escriba la cookie **[!UICONTROL Nombre de parámetro]** que desee y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2014-9-15-13-3a8-3a43.png)

   >[!TIP]
   >
   >Puede escribir un **[!UICONTROL valor predeterminado]** en caso de que no se encuentre el parámetro o la cookie.

## Parámetro de referencia {#referrer-parameter}

Si desea capturar datos de la página de la que salió el visitante antes de rellenar el formulario, puede usar **[!UICONTROL Parámetro de referente]**.

1. Establezca **[!UICONTROL Obtener valor de]** en **[!UICONTROL Parámetro de referente]**.

   ![](assets/image2014-9-15-13-3a9-3a31.png)

1. Escriba el **[!UICONTROL Nombre del parámetro]** que desee arrebatar de la dirección URL del referente y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2014-9-15-13-3a9-3a56.png)

   >[!TIP]
   >
   >Puede escribir un **[!UICONTROL Valor predeterminado]** en caso de que no se encuentre el parámetro de referente.

1. Haga clic en **[!UICONTROL Finalizar]**.

   ![](assets/image2014-9-15-13-3a10-3a26.png)

1. Haga clic en **[!UICONTROL Aprobar y cerrar]**.

   ![](assets/image2014-9-15-13-3a10-3a43.png)
