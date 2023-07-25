---
unique-page-id: 1147352
description: 'Enviar un correo electrónico de muestra: documentos de Marketo, documentación del producto'
title: Enviar correo electrónico de muestra
exl-id: b8f845e8-5c5e-463d-9d60-9c8103cec5ac
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

# Enviar correo electrónico de muestra {#send-a-sample-email}

Enviar muestras de un correo electrónico es rápido y sencillo. Para enviar un correo electrónico de contenido dinámico, consulte [Vista previa de un correo electrónico con contenido dinámico](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/preview-an-email-with-dynamic-content.md).

>[!NOTE]
>
>Debe tener el **Base de datos de Access - Ejecutar acciones de flujo único** permiso para enviar correos electrónicos de ejemplo.

## Enviar correo electrónico de muestra {#send-a-sample-email-1}

1. Busque y seleccione su correo electrónico. Haga clic en **Acciones de correo electrónico** y seleccione. **Enviar muestra**.\
   ![](assets/one-281-29.jpg)

   >[!NOTE]
   >
   >Mis tokens resuelven el valor apropiado para el programa del correo electrónico.

1. Introduzca una o varias direcciones de correo electrónico para la entrega. Para varias direcciones de correo electrónico, utilice comas para separarlas. Clic **Enviar** cuando termine.

   ![](assets/two.png)

   >[!IMPORTANT]
   >
   >Si introduce varias direcciones de correo electrónico, todos serán visibles para cada destinatario. El primero que introduzca será el destinatario principal y cada dirección de correo electrónico posterior será un destinatario de CC.

   >[!TIP]
   >
   >Si desea resolver tokens como una persona específica, elija dicha persona en la **lista desplegable de personas** en el paso 2.

## Enviar un correo electrónico de muestra durante la edición {#send-a-sample-email-while-editing}

1. Busque el correo electrónico, selecciónelo y haga clic en **Editar borrador** pestaña.

   ![](assets/three-281-29.jpg)

1. Clic **Acciones de correo electrónico**, seleccione **Enviar muestra**.

   ![](assets/four.png)

1. Introduzca una dirección de correo electrónico para la entrega y haga clic en **Enviar**.

   ![](assets/two.png)

   >[!NOTE]
   >
   >El campo déclencheur solo es aplicable a los que utilizan [script de correo electrónico](https://developers.marketo.com/documentation/velocity-script/).

## Enviar un correo electrónico de muestra basado en un segmento {#send-a-sample-email-based-on-a-segment}

>[!PREREQUISITES]
>
>[Aplicación de la segmentación a su correo electrónico](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/using-dynamic-content-in-an-email.md).

1. Busque el correo electrónico, selecciónelo y haga clic en **Editar borrador** pestaña.

   ![](assets/three-281-29.jpg)

1. Clic **Previsualizar**.

   ![](assets/1.png)

1. Haga clic en **Ver por** y seleccione. **Segmentación**.

   ![](assets/2.png)

1. Aparecerá una lista desplegable con las segmentaciones disponibles. Haga clic en él y seleccione el que desee.

   ![](assets/3.png)

1. Utilice las flechas para desplazarse por las opciones (en este caso, cambiamos dinámicamente la línea de asunto).

   ![](assets/4.png)

1. Clic **Enviar muestra** para recibir un correo electrónico de prueba del segmento en acción.

   ![](assets/5.png)

   >[!TIP]
   >
   >También puede enviar un correo electrónico de ejemplo basado en un segmento en el modo de edición del correo electrónico. Haga clic en **Acciones de correo electrónico** menú desplegable, seleccione **Enviar muestra** y, a continuación, elija el segmento.

Es muy importante muestrear el contenido antes de lanzar una campaña. Medir dos veces, cortar una vez!
