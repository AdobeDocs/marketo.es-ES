---
unique-page-id: 1147352
description: 'Envío de un correo electrónico de muestra: Documentos de Marketo: Documentación del producto'
title: Enviar un correo electrónico de ejemplo
exl-id: b8f845e8-5c5e-463d-9d60-9c8103cec5ac
source-git-commit: 1586b71ec9f9c4f8abc4fd9a3277d5a5f5b88080
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

# Enviar un correo electrónico de ejemplo {#send-a-sample-email}

Es rápido y fácil enviar muestras de un correo electrónico. Para enviar un correo electrónico de contenido dinámico, consulte [Vista previa de un correo electrónico con contenido dinámico](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/preview-an-email-with-dynamic-content.md).

>[!NOTE]
>
>Debe tener la variable **Acceso a Base de Datos: Ejecutar Acciones de Flujo Único** permiso para enviar correos electrónicos de ejemplo.

## Enviar un correo electrónico de ejemplo {#send-a-sample-email-1}

1. Busque y seleccione su correo electrónico. Haga clic en el **Acciones de correo electrónico** y seleccione **Enviar muestra**.\
   ![](assets/one-281-29.jpg)

   >[!NOTE]
   >
   >Mis tokens se resuelven en el valor apropiado para el programa del correo electrónico.

1. Introduzca una o varias direcciones de correo electrónico para la entrega. Para varias direcciones de correo electrónico, utilice comas para separarlas. Haga clic en **Enviar** cuando haya terminado.

   ![](assets/two.png)

   >[!IMPORTANT]
   >
   >Si introduce varias direcciones de correo electrónico, todas ellas serán visibles para cada destinatario. El primero introducido será el destinatario principal y cada dirección de correo electrónico posterior será un destinatario CC.

   >[!TIP]
   >
   >Si desea resolver los tokens como una persona específica, elija a esa persona en la variable **lista desplegable de personas** en el paso 2.

## Enviar un correo electrónico de ejemplo al editar {#send-a-sample-email-while-editing}

1. Busque su correo electrónico, selecciónelo y haga clic en el botón **Editar borrador** pestaña .

   ![](assets/three-281-29.jpg)

1. Haga clic en **Acciones de correo electrónico**, seleccione **Enviar muestra**.

   ![](assets/four.png)

1. Introduzca una dirección de correo electrónico para la entrega y haga clic en **Enviar**.

   ![](assets/two.png)

   >[!NOTE]
   >
   >El campo de déclencheur solo es aplicable a los que utilizan [secuencia de comandos de correo electrónico](https://developers.marketo.com/documentation/velocity-script/).

## Envío de un correo electrónico de muestra basado en un segmento {#send-a-sample-email-based-on-a-segment}

>[!PREREQUISITES]
>
>[Aplicar segmentación al correo electrónico](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/using-dynamic-content-in-an-email.md).

1. Busque su correo electrónico, selecciónelo y haga clic en el botón **Editar borrador** pestaña .

   ![](assets/three-281-29.jpg)

1. Haga clic en **Vista previa**.

   ![](assets/1.png)

1. Haga clic en el **Ver por** y seleccione **Segmentación**.

   ![](assets/2.png)

1. Aparece un menú desplegable con las segmentaciones disponibles. Haga clic en él y seleccione el que desee.

   ![](assets/3.png)

1. Utilice las flechas para desplazarse por sus opciones (en este caso cambiamos dinámicamente la línea de asunto).

   ![](assets/4.png)

1. Haga clic en **Enviar muestra** para recibir un correo electrónico de prueba del segmento en acción.

   ![](assets/5.png)

   >[!TIP]
   >
   >También puede enviar un correo electrónico de ejemplo basado en un segmento en el modo de edición del correo electrónico. Haga clic en el **Acciones de correo electrónico** desplegable, seleccione **Enviar muestra** y, a continuación, elija su segmento.

Muestreo del contenido antes de lanzar una campaña es muy importante. ¡Medir dos veces, cortar una vez!
