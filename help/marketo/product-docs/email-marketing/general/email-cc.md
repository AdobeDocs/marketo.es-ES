---
unique-page-id: 17727995
description: Email CC - Marketo Docs - Documentación del producto
title: Correo electrónico CC
exl-id: 00550e98-916d-4e66-91f8-7394c242a29b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---

# Correo electrónico CC {#email-cc}

Email CC permite enviar correos electrónicos especificados a través de Marketo para incluir destinatarios CC.

Esta función está disponible en todos los recursos de correo electrónico de Marketo, independientemente de cómo se envíe el correo electrónico (campaña por lotes o de déclencheur). El destinatario de CC recibirá una copia exacta del correo electrónico enviado a la persona de Marketo elegida. Como tal, cualquier actividad de participación (aperturas, clics, etc.) se registrará en el registro de actividades de la persona de Marketo en la línea &quot;Para&quot; del correo electrónico. Sin embargo, la actividad de entrega (enviada, entregada, rechazada grave, etc.) _distinto de &quot;bounce suave&quot;_ will **not** , ya que Marketo no puede distinguir los eventos de envío para la persona de Marketo de los de los destinatarios de CC. Marketo sólo contará con un máximo de 100.000 personas a la vez. Si tu lista inteligente supera los 100.000 y es imperativo que todas las personas que estén en ella tengan CC&#39;d, te recomendamos que rompas tu lista.

>[!NOTE]
>
>El correo electrónico CC no estaba diseñado para utilizarse con pruebas A/B. Puede usarlo de todas formas si lo desea, pero como técnicamente no es compatible, el servicio de asistencia técnica de Marketo no podría ayudarle en la resolución de problemas.

## Configurar correo electrónico CC {#set-up-email-cc}

1. En Mi Marketo, haga clic en **Administrador**.

   ![](assets/one.png)

1. En el árbol, seleccione **Correo electrónico**.

   ![](assets/two.png)

1. Haga clic en **Editar configuración de correo electrónico CC**.

   ![](assets/three.png)

1. Seleccione hasta 25 campos de empresa o posible cliente de Marketo (de tipo &quot;correo electrónico&quot;) para que estén disponibles para su uso como direcciones CC dentro de los correos electrónicos. Haga clic en **Guardar** cuando haya terminado.

   ![](assets/four.png)

## Uso de Email CC {#using-email-cc}

1. Seleccione el correo electrónico y haga clic en **Editar borrador**.

   ![](assets/five.png)

1. Haga clic en **Configuración de correo electrónico**.

   ![](assets/six.png)

1. Seleccione hasta cinco campos que quiera usar con personas de CC. En este ejemplo, solo queremos el CC del propietario del posible cliente. Haga clic en **Guardar** cuando haya terminado.

   ![](assets/seven.png)

   ¡Es tan simple como eso! En el ejemplo anterior, al enviar el correo electrónico, el propietario del posible cliente de los destinatarios que ha elegido será CC&#39;d.

   >[!NOTE]
   >
   >Si una dirección de correo electrónico no válida está en un campo CC, se omitirá.

   Para una identificación rápida, la vista Resumen de correo electrónico le muestra si se seleccionaron los campos CC de correo electrónico.

   ![](assets/eight.png)

   Si el correo electrónico está aprobado, pero el administrador de Marketo desactiva uno o más de los campos CC antes de que se envíe el correo electrónico, **esas personas no recibirán un correo electrónico**. En ese escenario, la vista Resumen de correo electrónico mostrará en gris los campos deshabilitados después de la aprobación pero previamente al envío:

   ![](assets/removal.png)

   >[!NOTE]
   >
   >También verá el error anterior en la sección Configuración de correo electrónico del borrador de correo electrónico.

## Después del envío {#after-the-send}

* Si un destinatario de CC hace clic en un vínculo rastreado en el correo electrónico, la actividad de clic (como cualquier otra actividad de participación) se asociará con el destinatario principal del correo electrónico. Además, pueden hacer clic en una página con el código de seguimiento web de Marketo (munchkin.js), lo que provoca que se les codifique como destinatario principal.

>[!TIP]
>
>Tiene la opción de [desactivación de algunos vínculos o de todos los vínculos de seguimiento](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/disable-tracking-for-an-email-link.md) en un correo electrónico.

* Después de ejecutar una campaña de correo electrónico, la actividad Enviar correo electrónico incluye una lista de todas las direcciones CC incluidas para cada destinatario del correo. Si se omitieron direcciones CC debido a la cancelación de la suscripción, también se indicará en la actividad.
* Los vínculos y las páginas de cancelación de suscripción funcionan normalmente en los correos electrónicos CC. Esto permite a los destinatarios de CC cancelar la suscripción correctamente si lo desean (cumpliendo con las regulaciones antispam), y se almacenará un registro de esta acción en la base de datos de Marketo.
* Las personas que aparezcan como canceladas la suscripción en la base de datos de Marketo **not** recibir correos electrónicos a través de CC.
