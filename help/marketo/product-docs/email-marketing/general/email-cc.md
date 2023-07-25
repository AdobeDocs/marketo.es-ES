---
unique-page-id: 17727995
description: 'Correo electrónico CC: documentos de Marketo, documentación del producto'
title: Correo electrónico CC
exl-id: 00550e98-916d-4e66-91f8-7394c242a29b
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---

# Correo electrónico CC {#email-cc}

Correo electrónico CC permite que determinados correos electrónicos se envíen a través de Marketo para incluir destinatarios CC.

Esta función está disponible en todos los recursos de correo electrónico de Marketo, independientemente de cómo se envíe el correo electrónico (campaña por lotes o por déclencheur). El destinatario del CC recibirá una copia exacta del correo electrónico enviado a la persona de Marketo elegida. Como tal, cualquier actividad de participación (aperturas, clics, etc.) se registrará en el registro de actividad de la persona de Marketo en la línea &quot;Para&quot; del correo electrónico. Sin embargo, la actividad de envío (envío, envío, devolución, etc.) _que no sea &quot;rebote suave&quot;_ testamento **no** , ya que Marketo no puede distinguir los eventos de envío para la persona de Marketo de los de los destinatarios de CC. Marketo solo permite crear un CC de hasta 100 000 personas a la vez. Si tu lista inteligente supera los 100.000 y es imperativo que todas las personas en ella tengan CC, te recomendamos que separes tu lista.

>[!NOTE]
>
>El correo electrónico CC no se ha diseñado para su uso con pruebas A/B. Puede usarlo de todos modos si lo desea; sin embargo, como técnicamente no es compatible, el soporte técnico de Marketo no podría ayudarle con la resolución de problemas.

## Configuración de correo electrónico CC {#set-up-email-cc}

1. En Mi Marketo, haga clic en **Administrador**.

   ![](assets/one.png)

1. En el árbol, seleccione **Correo electrónico**.

   ![](assets/two.png)

1. Clic **Editar configuración de CC del correo electrónico**.

   ![](assets/three.png)

1. Seleccione hasta 25 campos de posible cliente o empresa de Marketo (de tipo &quot;correo electrónico&quot;) para que estén disponibles para su uso como direcciones CC en los correos electrónicos. Clic **Guardar** cuando termine.

   ![](assets/four.png)

## Uso de Email CC {#using-email-cc}

1. Seleccione el correo electrónico y haga clic en **Editar borrador**.

   ![](assets/five.png)

1. Clic **Configuración de correo electrónico**.

   ![](assets/six.png)

1. Seleccione hasta cinco campos que desee utilizar para copiar personas. En este ejemplo, solo queremos el CC del propietario del posible cliente. Clic **Guardar** cuando termine.

   ![](assets/seven.png)

   ¡Es tan simple como eso! En el ejemplo anterior, cuando envía el correo electrónico, el propietario principal de los destinatarios que elija es CC.

   >[!NOTE]
   >
   >Si una dirección de correo electrónico no válida está en un campo CC, se omitirá.

   Para una identificación rápida, la vista Resumen de correo electrónico muestra si se han seleccionado los campos CC de correo electrónico o cuáles se han seleccionado.

   ![](assets/eight.png)

   Si el correo electrónico está aprobado, pero el administrador de Marketo deshabilita uno o más de los campos CC antes de que se envíe el correo electrónico, **estas personas no recibirán un correo electrónico**. En ese caso, la vista Resumen de correo electrónico atenuará los campos que se deshabilitaron después de la aprobación pero antes del envío:

   ![](assets/removal.png)

   >[!NOTE]
   >
   >También verá el error anterior en la sección Configuración de correo electrónico del borrador del correo electrónico.

## Después del envío {#after-the-send}

* Si un destinatario de CC hace clic en un vínculo rastreado en el correo electrónico, la actividad de clic (como todas las demás actividades de participación) se asocia al destinatario principal del correo electrónico. Además, pueden hacer clic en hasta una página con código de seguimiento web de Marketo (munchkin.js), lo que provoca que se les cookie como destinatario principal.

>[!TIP]
>
>Tiene la opción de [deshabilitar algunos o todos los vínculos de seguimiento](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/disable-tracking-for-an-email-link.md) en un correo electrónico.

* Después de ejecutar una campaña de correo electrónico, la actividad Enviar correo electrónico incluirá una lista de todas las direcciones CC que se incluyeron para cada destinatario del correo. Si se omitieron direcciones CC debido a la cancelación de la suscripción, también se anotará en la actividad.
* Los vínculos de cancelación de suscripción y las páginas funcionan normalmente en los correos electrónicos de CC. Esto permite a los destinatarios de CC cancelar la suscripción correctamente si lo desean (cumpliendo con las regulaciones antispam) y se almacenará un registro de esta acción en la base de datos de Marketo.
* Las personas que figuren como canceladas sus suscripciones en la base de datos de Marketo **no** recibir correos electrónicos a través de CC.
