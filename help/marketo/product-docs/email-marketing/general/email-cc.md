---
unique-page-id: 17727995
description: 'Correo electrónico CC: documentos de Marketo, documentación del producto'
title: Correo electrónico CC
exl-id: 00550e98-916d-4e66-91f8-7394c242a29b
feature: Email Editor
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 0%

---

# Correo electrónico CC {#email-cc}

Correo electrónico CC permite que determinados correos electrónicos se envíen a través de Marketo para incluir destinatarios CC.

Esta función está disponible en todos los recursos de correo electrónico de Marketo, independientemente de cómo se envíe el correo electrónico (campaña por lotes o por déclencheur). El destinatario del CC recibirá una copia exacta del correo electrónico enviado a la persona de Marketo elegida. Como tal, cualquier actividad de participación (aperturas, clics, etc.) se registrará en el registro de actividad de la persona de Marketo en la línea &quot;Para&quot; del correo electrónico. Sin embargo, la actividad de entrega (enviada, entregada, rechazada de forma grave, etc.) _distinta de la &quot;devolución de mensajes no entregados&quot;_ **no se registrará**, ya que Marketo no puede distinguir los eventos de entrega para la persona de Marketo de los destinatarios de CC. Marketo solo permite crear un CC de hasta 100 000 personas a la vez. Si tu lista inteligente supera los 100.000 y es imperativo que todas las personas en ella tengan CC, te recomendamos que separes tu lista.

>[!NOTE]
>
>El correo electrónico CC no se ha diseñado para su uso con pruebas A/B. Puede usarlo de todos modos si lo desea; sin embargo, como técnicamente no es compatible, el soporte técnico de Marketo no podría ayudarle con la resolución de problemas.

## Configuración de correo electrónico CC {#set-up-email-cc}

1. En Mi Marketo, haga clic en **[!UICONTROL Administrador]**.

   ![](assets/one.png)

1. En el árbol, seleccione **[!UICONTROL Correo electrónico]**.

   ![](assets/two.png)

1. Haga clic en **[!UICONTROL Editar configuración de CC del correo electrónico]**.

   ![](assets/three.png)

1. Seleccione hasta 25 campos de posible cliente o empresa de Marketo (de tipo &quot;correo electrónico&quot;) para que estén disponibles para su uso como direcciones CC en los correos electrónicos. Haga clic en **Guardar** cuando termine.

   ![](assets/four.png)

## Uso de Email CC {#using-email-cc}

1. Seleccione su correo electrónico y haga clic en **[!UICONTROL Editar borrador]**.

   ![](assets/five.png)

1. Haga clic en **[!UICONTROL Configuración de correo electrónico]**.

   ![](assets/six.png)

1. Seleccione los campos que desee utilizar para crear correspondencia personalizada. _Hay un límite de cinco por correo electrónico_. En este ejemplo, solo queremos el CC del propietario del posible cliente. Haga clic en **Guardar** cuando haya terminado.

   ![](assets/seven.png)

   ¡Es tan simple como eso! En el ejemplo anterior, cuando envía el correo electrónico, el propietario principal de los destinatarios que elija es CC.

   >[!NOTE]
   >
   >Si una dirección de correo electrónico no válida está en un campo CC, se omitirá.

   Para una identificación rápida, la vista Resumen de correo electrónico muestra si se han seleccionado los campos CC de correo electrónico o cuáles se han seleccionado.

   ![](assets/eight.png)

   Si el correo electrónico se aprueba, pero el administrador de Marketo deshabilita uno o más de los campos CC antes de que se envíe el correo electrónico, **esas personas no recibirán un correo electrónico**. En ese caso, la vista Resumen de correo electrónico atenuará los campos que se deshabilitaron después de la aprobación pero antes del envío:

   ![](assets/removal.png)

   >[!NOTE]
   >
   >También verá el error anterior en la sección Configuración de correo electrónico del borrador del correo electrónico.

## Después del envío {#after-the-send}

* Si un destinatario de CC hace clic en un vínculo rastreado en el correo electrónico, la actividad de clic (como todas las demás actividades de participación) se asocia al destinatario principal del correo electrónico. Además, pueden hacer clic en hasta una página con código de seguimiento web de Marketo (munchkin.js), lo que provoca que se les cookie como destinatario principal.

>[!TIP]
>
>Tiene la opción de [deshabilitar algunos o todos los vínculos de seguimiento](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/disable-tracking-for-an-email-link.md) en un mensaje de correo electrónico.

* Después de ejecutar una campaña de correo electrónico, la actividad Enviar correo electrónico incluirá una lista de todas las direcciones CC que se incluyeron para cada destinatario del correo. Si se omitieron direcciones CC debido a la cancelación de la suscripción, también se anotará en la actividad.
* Los vínculos de cancelación de suscripción y las páginas funcionan normalmente en los correos electrónicos de CC. Esto permite a los destinatarios de CC cancelar la suscripción correctamente si lo desean (cumpliendo con las regulaciones antispam) y se almacenará un registro de esta acción en la base de datos de Marketo.
* Las personas que figuren como canceladas sus suscripciones en la base de datos de Marketo **no** recibirán correos electrónicos a través de CC.
