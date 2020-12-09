---
unique-page-id: 2359424
description: Alertar al representante de ventas - Documentos de marketing - Documentación del producto
title: Alertar al representante de ventas
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 0%

---


# Alertar al representante de ventas {#alert-the-sales-rep}

## Misión: Alertar al representante de ventas cuando una persona rellene un formulario en el sitio web {#mission-alert-the-sales-rep-when-a-person-fills-out-a-form-on-your-web-site}

Para enviar automáticamente correos electrónicos de alerta a los representantes de ventas, todo lo que necesita es un correo electrónico de alerta y una campaña por correo electrónico. Así es como hacerlo.

>[!NOTE]
>
>**FYI**
>
>Marketo ahora está estandarizando el idioma en todas las suscripciones, por lo que puede ver posibles clientes/posibles clientes en su suscripción y persona/personas en docs.marketo.com. Estos términos significan lo mismo; no afecta a las instrucciones del artículo. También hay otros cambios. [Más información](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

>[!PREREQUISITES]
>
>* [página de aterrizaje con un formulario](landing-page-with-a-form.md)

>



## Paso 1: Crear un correo electrónico de alerta {#step-create-an-alert-email}

1. Vaya al área Actividades **de** marketing.

   ![](assets/one-5.png)

1. Seleccione **Mi Programa** que ha creado en la [Página de aterrizaje con una ganancia rápida de formulario](landing-page-with-a-form.md) y, a continuación, en **Nuevo** , haga clic en **Nuevo recurso** local.

   ![](assets/two-6.png)

1. Haga clic en **Correo electrónico**.

   ![](assets/three-5.png)

1. **Asigne un nombre** al correo electrónico &quot;Mi alerta de correo electrónico&quot;, seleccione una plantilla y haga clic en **Crear**.

   ![](assets/four-4.png)

1. Introduzca el **Nombre**, **De correo electrónico**, **Respuesta** y **Asunto** que desea que vea su equipo de ventas.

   ![](assets/five-5.png)

1. Haga clic con el doble para editar el texto del correo electrónico.

   ![](assets/six-5.png)

1. Escriba el contenido del correo electrónico.

   ![](assets/seven-6.png)

1. Coloque el cursor donde desee insertar la información de contacto de la persona y haga clic en el icono **Insertar token** .

   ![](assets/eight-4.png)

1. Busque y seleccione el `{{SP_Send_Alert_Info}}` token **y haga clic en** Insertar ****.

   ![](assets/image2014-9-24-13-3a10-3a0.png)

   >[!NOTE]
   >
   >{{SP_Send_Alert_Info}} es un token especial para los mensajes de correo electrónico de alerta. Consulte [Uso del testigo](../../product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md) Enviar información de alerta para obtener más información.

1. Haga clic en **Guardar**.

   ![](assets/ten-5.png)

1. Cierre la ficha o ventana del editor de correo electrónico.

   ![](assets/eleven-5.png)

1. En Acciones **de** correo electrónico, haga clic en **Aprobar**.

   ![](assets/twelve-4.png)

## Paso 2: Crear una Campaña de desencadenador de alertas {#step-create-an-alert-trigger-campaign}

1. Seleccione **Mi Programa** creado anteriormente y, a continuación, en **Nuevo **haga clic en **Nueva Campaña** inteligente.

   ![](assets/image2014-9-24-13-3a14-3a17.png)

1. **Asigne un nombre** a la campaña &quot;Mi Campaña de alerta&quot; y haga clic en **Crear**.

   ![](assets/image2014-9-24-13-3a14-3a28.png)

1. En la ficha Lista **** inteligente, busque y arrastre el activador **Rellenar formulario** al lienzo.

   ![](assets/image2014-9-24-13-3a14-3a43.png)

1. Seleccione el formulario que hemos creado anteriormente.

   ![](assets/image2014-9-24-13-3a14-3a58.png)

1. En la ficha **Flujo** , busque y arrastre la acción **Enviar alerta** al lienzo.

   ![](assets/image2014-9-24-13-3a15-3a10.png)

1. Seleccione **Mi correo electrónico** de alerta creado anteriormente y deje **Enviar a** como propietario **de** ventas.

   ![](assets/eighteen-1.png)

1. Escriba su dirección de correo electrónico en el campo **A otros correos electrónicos** .

   ![](assets/nineteen-2.png)

1. Vaya a la ficha **Programar** y haga clic en el botón **Activar **Ver.

   ![](assets/twenty-2.png)

   >[!TIP]
   >
   >
   >Configure las reglas **de** cualificación en **cada vez** (editando la Campaña inteligente) para permitir que la misma persona active las alertas varias veces.

1. Haga clic en **Activar** en la pantalla de confirmación.

   ![](assets/twenty-one-1.png)

## Paso 3: ¡Pruébelo! {#step-test-it-out}

1. Seleccione la página de aterrizaje y haga clic en **Vista Página** aprobada.

   ![](assets/image2014-9-24-13-3a17-3a8.png)

   >[!NOTE]
   >
   >**Recordatorio**
   >
   >
   >No te olvides de aprobar páginas de aterrizaje; no se activan hasta que se aprueban.

1. Complete el formulario y haga clic en **Enviar**.

   ![](assets/image2014-9-24-13-3a17-3a41.png)

1. Deberías recibir tu correo electrónico en breve. Una vez que haya comprobado que todo funciona como debería, elimine su dirección de correo electrónico del flujo Enviar alerta (consulte el paso 2.7 anterior).

   >[!NOTE]
   >
   >Haga clic en la ficha Información de **persona** en Marketo para ver la información de contacto.

## Misión finalizada {#mission-complete}

<br> 

[◄ Misión 7: Personalice un correo electrónico](personalize-an-email.md) [de Misión 9: Actualizar datos de posibles clientes ►](update-person-data.md)